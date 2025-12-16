# CampusCucei

CampusCucei es una app móvil hecha con **React Native + Expo** pensada para estudiantes de CUCEI.  
Permite iniciar sesión con código y NIP, consultar información académica y acceder a recursos externos como el directorio y videos informativos.

> Nota: Esta app consume servicios externos que **no son de mi autoría**.  
> El código de la app sí es propio, pero el backend y algunas páginas embebidas pertenecen a terceros.

---

##  Funcionalidades

- Pantalla de **login** con código y NIP.
- Uso de un **backend externo** para autenticación y datos académicos.
- Visualización de:
  - Información del alumno.
  - Información académica (kárdex, materias, etc., según lo que devuelva el backend).
- **Directorio** embebido en un `WebView`.
- Sección de **videos** (contenido hosteado externamente en otro repositorio de mi propiedad).
- **Mapa interactivo del campus CUCEI**:
  - Muestra un mapa del campus.
  - Incluye hotspots en edificios/módulos.
  - Cada hotspot abre un modal con galería de fotos y descripción del lugar.
  - Bloquea la orientación en **horizontal** mientras el mapa está abierto para mejor visualización.
- **Modo demo** opcional para poder probar la app sin usar el backend real.

---

##  Stack tecnológico

- [React Native](https://reactnative.dev/)
- [Expo](https://expo.dev/)
- [react-native-webview](https://github.com/react-native-webview/react-native-webview)
- [AsyncStorage](https://github.com/react-native-async-storage/async-storage)
- React Navigation

---
## Estructura del proyecto

Actualmente el proyecto está organizado en pantallas principales:

- `App.js`: punto de entrada de la app.
- `Loggin.js`: pantalla de inicio de sesión.
- `Menu.js`: menú principal / navegación.
- `KardexAlumno.js`: consulta de información académica.
- `Directorio.js`: directorio embebido en WebView.
- `Video.js`: pantalla para videos informativos.
- `MapaLite.js`: mapa interactivo del campus.
- `PerfilAlumno.js`: información del perfil del alumno.
- `Principal.js`: pantalla principal/inicial tras el login.
- `config.js`: configuración de URLs/endpoints externos.
- `mapa_2024.jpg`: recurso de mapa usado en la pantalla de mapa.

##  Instalación y ejecución

1. Clona este repositorio:

   ```bash
   git clone https://github.com/AlanGlzQ/Aplicaci-n-M-vil-Escolar.git
   cd Aplicaci-n-M-vil-Escolar

2. Instala dependencias
  npm install
  # o
  yarn install

3. Inicia el proyecto con Expo
  npx expo start

4. Escanea el QR con la app de Expo Go en tu teléfono, o ejecútalo en un emulador.

##  Demo en video

Puedes ver una demostración completa de la aplicación aquí:

 [![Demo CampusCucei](campus_thumbnail.png)](https://drive.google.com/file/d/1BUcxZBWQS5o8fPSMrI4n87ukulmyjMwg/view?usp=sharing)

## Estado del proyecto

Este proyecto fue desarrollado como proyecto escolar/personal y no está pensado
como aplicación de producción. El backend y algunos recursos externos pueden cambiar
o dejar de estar disponibles con el tiempo.

El código del frontend (esta app) es de mi autoría.
