# chatgpt-14-05-2026-debug-login-smartlearn.md

## Objetivo
Resolver problemas relacionados con el login, registro y autenticación en la aplicación móvil Smart Learn, específicamente la comunicación entre Android (Retrofit/OkHttp) y el backend en Spring Boot.

---

## Contexto
Se revisaron múltiples clases del proyecto Smart Learn tanto del lado Android como Spring Boot relacionadas con:
- API REST usando Retrofit.
- Login biométrico y manual.
- Persistencia local con SharedPreferences.
- Configuración de Retrofit y OkHttp.
- Flujo de navegación de actividades.
- Configuración del Manifest.
- Respuesta de login mediante JWT/token.
- Logs completos de Android Studio.

El usuario estaba teniendo:
- Error 401 en login.
- Error `Too many follow-up requests: 21` durante registro.
- Problemas aparentes de autenticación y posibles redirecciones infinitas.

---

## Ideas clave
- El login sí estaba llegando correctamente al backend.
- El endpoint `/smartlearn/api/usuario/login` respondía con HTTP 401 cuando las credenciales eran incorrectas.
- El error `Too many follow-up requests: 21` normalmente ocurre por:
  - Redirecciones infinitas.
  - Problemas de seguridad Spring Security.
  - Reenvíos automáticos de OkHttp.
  - Interceptors mal configurados.
- El interceptor de autenticación estaba agregando headers correctamente.
- Retrofit y OkHttp estaban configurados correctamente a nivel general.
- El backend Spring Boot sí estaba respondiendo.
- El problema parecía estar relacionado con estado interno de autenticación/sesión o comportamiento del backend.
- Después de acceder desde navegador y probar nuevamente con un usuario válido, el sistema comenzó a funcionar normalmente.

---

## Decisiones
- Mantener Retrofit con:
  - `AuthInterceptor`
  - `HttpLoggingInterceptor`
  - `GsonConverterFactory`
- Mantener `usesCleartextTraffic="true"` mientras se usa HTTP sin HTTPS.
- Continuar usando SharedPreferences para:
  - Token.
  - Estado de sesión.
  - ID de usuario.
- Validar que el login manual siga usando:
  - `nombreCuenta`
  - `contrasena`
- No modificar más el flujo actual debido a que el problema quedó resuelto.

---

## Trabajo realizado
### Código revisado Android
Se revisaron:
- `ApiService`
- `RetrofitClient`
- `LoginLogic`
- `PreferencesManager`
- `MainActivity`
- `CargaActivity`
- `SmartLearnApp`
- `AndroidManifest.xml`
- `LoginResponse`

### Código revisado Spring Boot
Se revisaron:
- `LoginRequest`
- `LoginResponse`

### Análisis realizado
- Verificación de rutas Retrofit.
- Comparación de atributos enviados en JSON.
- Revisión de logs HTTP completos.
- Revisión de headers enviados:
  - `X-Client-Type`
  - `User-Agent`
  - Token JWT.
- Revisión del comportamiento de OkHttp.
- Revisión del flujo de navegación Android.
- Verificación de persistencia de sesión.
- Análisis del error:
  - `ProtocolException: Too many follow-up requests: 21`

### Hallazgos importantes
- El login incorrecto devolvía correctamente HTTP 401.
- El usuario no registrado realmente no existía en base de datos.
- Solo uno de los intentos de registro sí se guardó.
- Después de acceder desde navegador y usar un usuario válido, el sistema comenzó a responder normalmente.

---

## Problemas/dudas
### Problemas encontrados
- Error 401 durante autenticación.
- Error de follow-up requests infinitos.
- Inconsistencia aparente entre registros realizados desde Android y registros persistidos realmente.

### Posibles causas identificadas
- Estado temporal del backend.
- Configuración Spring Security.
- Redirecciones automáticas.
- Sesiones/cookies.
- Posible comportamiento inesperado del servidor tras múltiples intentos.

### Dudas pendientes
- Confirmar exactamente qué originó el problema inicial.
- Verificar si existe alguna redirección oculta en Spring Security.
- Confirmar que no existan filtros duplicados o conflictos de autenticación.

---

## Conclusiones
- El sistema actualmente quedó funcionando correctamente.
- Retrofit, OkHttp y el flujo general de login parecen estar bien configurados.
- El problema probablemente estuvo relacionado con:
  - estado temporal del backend,
  - autenticación,
  - o comportamiento interno de Spring Security.
- Sería recomendable posteriormente:
  - agregar logs más detallados del lado backend,
  - revisar filtros de seguridad,
  - y validar respuestas HTTP en endpoints de registro y login.
- También sería útil implementar:
  - manejo explícito de errores 401/403,
  - refresh de token,
  - y trazabilidad más detallada en autenticación.
