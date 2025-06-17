# 🔔 Notificaciones Locales Flutter

Una aplicación Flutter colorida y moderna que permite enviar notificaciones locales personalizadas con títulos y mensajes customizables.

## ✨ Características

- 🎨 **Interfaz colorida** con gradientes y animaciones
- 📱 **Notificaciones personalizables** (título y mensaje)
- ✅ **Validación de campos** obligatorios
- 🔄 **Limpieza automática** de formularios
- 💫 **Feedback visual** con SnackBars
- 🎯 **Diseño responsivo** y moderno

## 🚀 Instalación

### Requisitos previos
- Flutter SDK (versión 3.32.4 o superior)
- Dart 3.8.1 o superior
- Android Studio o VS Code
- Android SDK para testing en Android

### Pasos de instalación

1. **Clonar el repositorio**
   ```bash
   git clone [url-del-repositorio]
   cd localnotifications
   ```

2. **Instalar dependencias**
   ```bash
   flutter pub get
   ```

3. **Verificar configuración**
   ```bash
   flutter doctor
   ```

4. **Ejecutar la aplicación**
   ```bash
   flutter run
   ```

## 📦 Dependencias

### Dependencias principales
```yaml
dependencies:
  flutter:
    sdk: flutter
  flutter_local_notifications: ^18.1.2
```

### Dependencias de desarrollo
```yaml
dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^5.0.0
```

## 📱 Configuración de Plataformas

### Android
La aplicación está configurada para Android con:
- **Canal de notificaciones**: `custom_channel_id`
- **Nombre del canal**: "Notificaciones Personalizadas"
- **Importancia**: Máxima prioridad
- **Características**: Sonido, vibración, color púrpura

### Permisos requeridos
El plugin maneja automáticamente los permisos de notificaciones en Android 13+.

## 🎯 Uso de la Aplicación

### Enviar una notificación

1. **Abrir la aplicación**
2. **Escribir un título** en el primer campo (obligatorio)
3. **Escribir un mensaje** en el segundo campo (obligatorio)
4. **Presionar "🚀 Enviar Notificación"**
5. **Ver la confirmación** en pantalla
6. **Revisar la notificación** en la barra de notificaciones

### Validaciones
- ⚠️ Ambos campos (título y mensaje) son obligatorios
- ✅ Mensaje de confirmación al enviar exitosamente
- 🧹 Los campos se limpian automáticamente después del envío

## 🛠️ Estructura del Proyecto

```
localnotifications/
├── lib/
│   └── main.dart              # Archivo principal de la aplicación
├── android/                   # Configuración específica de Android
├── pubspec.yaml              # Dependencias y configuración del proyecto
└── README.md                 # Este archivo
```

## 🎨 Personalización

### Colores del tema
```dart
// Colores principales utilizados
Colors.deepPurple     // Color primario
Colors.purple         // Color secundario
Colors.pinkAccent     // Color de acento
Colors.orange         // Color del ícono
```

### Modificar gradientes
Los gradientes se pueden personalizar en:
- **Fondo de la aplicación**: `LinearGradient` en el Container principal
- **AppBar**: `flexibleSpace` con gradiente personalizado
- **Botón**: `BoxDecoration` con gradiente rosa-púrpura

## 🔧 Configuración del IDE

### VS Code
Agregar al archivo `.vscode/settings.json`:
```json
{
    "dart.sdkPath": "/opt/homebrew/bin/dart",
    "dart.flutterSdkPath": "/opt/homebrew/bin/flutter"
}
```

### Android Studio
1. Ir a **Preferences > Languages & Frameworks > Dart**
2. Marcar **Enable Dart support**
3. Configurar **Dart SDK path**: `/opt/homebrew/bin/dart`

## 🐛 Solución de Problemas

### Error: "Dart SDK no configurado"
```bash
# Verificar instalación
dart --version
flutter --version

# Configurar PATH si es necesario
export PATH="$PATH:/opt/homebrew/bin/dart"
export PATH="$PATH:/opt/homebrew/bin/flutter"
```

### Error: "Android licenses"
```bash
# Aceptar licencias de Android
flutter doctor --android-licenses
```

### Error: "sdkmanager not found"
1. Abrir Android Studio
2. Ir a **SDK Manager**
3. Instalar **Android SDK Command-line Tools**

## 📚 Recursos Adicionales

- [Documentación oficial de Flutter](https://flutter.dev/docs)
- [flutter_local_notifications plugin](https://pub.dev/packages/flutter_local_notifications)
- [Guía de notificaciones Android](https://developer.android.com/guide/topics/ui/notifiers/notifications)

## 👨‍💻 Desarrollo

### Ejecutar en modo debug
```bash
flutter run --debug
```

### Compilar para release
```bash
flutter build apk --release
```

### Limpiar caché
```bash
flutter clean
flutter pub get
```

## 📄 Licencia

Este proyecto es de código abierto y está disponible bajo la licencia MIT.

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Para contribuir:

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/nueva-funcionalidad`)
3. Commit tus cambios (`git commit -m 'Agregar nueva funcionalidad'`)
4. Push a la rama (`git push origin feature/nueva-funcionalidad`)
5. Abre un Pull Request

## 📞 Soporte

Si tienes problemas o preguntas:
- Revisa la sección de **Solución de Problemas**
- Consulta la documentación oficial de Flutter
- Crea un issue en el repositorio

---

**¡Disfruta creando notificaciones personalizadas con Flutter! 🎉**
