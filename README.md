# EPS · App móvil

App móvil para gestionar **citas médicas** en una EPS, hecha con **React Native + Expo**. Muestra una experiencia distinta según el rol: paciente, doctor o administrador.

Backend: [EpsLaravel](https://github.com/CristianGarcia7/EpsLaravel)

## 📱 Funcionalidades

**Paciente**
- Registro, inicio de sesión y recuperación de contraseña
- Solicitar citas eligiendo doctor, horario y consultorio
- Ver el estado de sus citas

**Doctor**
- Ver, aprobar, rechazar y completar citas
- Gestionar sus horarios
- Ver su consultorio asignado

**Administrador**
- Dashboard con contadores
- Gestión de usuarios, doctores, pacientes, especialidades, consultorios y citas

**General**
- 🔔 Notificaciones push (`expo-notifications`) cuando cambia una cita
- 🌙 Modo oscuro guardado en el dispositivo
- Navegación por pestañas y *stacks* separados por rol

## 🧱 Stack

React Native 0.81 · Expo SDK 54 · React Navigation 7 · Axios · AsyncStorage · EAS Build

## 🚀 Cómo correrlo

1. Levanta el [backend](https://github.com/CristianGarcia7/EpsLaravel).
2. Cambia `URL_BASE` en [`Src/Services/Conexion.js`](Src/Services/Conexion.js) por la URL de tu API (por ejemplo, un túnel de ngrok).
3. Instala y ejecuta:

```bash
npm install
npx expo start
```
