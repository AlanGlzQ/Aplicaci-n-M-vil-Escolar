# CampusCucei

CampusCucei es una app móvil hecha con **React Native + Expo** pensada para estudiantes de CUCEI.  
Permite iniciar sesión con código y NIP, consultar información académica y acceder a recursos externos como el directorio y videos informativos.

> Nota: Esta app consume servicios externos que **no son de mi autoría**.  
> El código de la app sí es propio, pero el backend y algunas páginas embebidas pertenecen a terceros.

---

## 🚀 Funcionalidades

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

## 🧱 Stack tecnológico

- [React Native](https://reactnative.dev/)
- [Expo](https://expo.dev/)
- [react-native-webview](https://github.com/react-native-webview/react-native-webview)
- [AsyncStorage](https://github.com/react-native-async-storage/async-storage)
- React Navigation

---

## 📦 Instalación y ejecución

1. Clona este repositorio:

   ```bash
   git clone https://github.com/<TU_USUARIO>/<TU_REPO>.git
   cd <TU_REPO>

2. Instala dependencias
  npm install
  # o
  yarn install

3. Inicia el proyecto con Expo
  npx expo start

4. Escanea el QR con la app de Expo Go en tu teléfono, o ejecútalo en un emulador.
