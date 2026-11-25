# Vaporeon

Descargas oficiales del launcher de Minecraft **Vaporeon**.

## Descargas

- [Última versión](https://github.com/hotcakes-py/Vaporeon/releases/latest)
- `Vaporeon-Installer.exe` — instalador de Windows. Instala solamente `Vaporeon.exe` y crea las carpetas de datos en `%APPDATA%\.vaporeon`.
- `Vaporeon-Portable.zip` — versión portable: contiene únicamente `Vaporeon.exe`, sin carpetas `src` ni archivos de compilación.

Cada `push` en el repositorio privado `VaporeonCode` compila automáticamente ambos archivos y los publica aquí como un release.

## Sobre el aviso de Windows SmartScreen

Si Windows muestra "Windows protegió su equipo" o dice que el archivo "no puede
ser seguro", **no significa que tenga un virus**: aparece porque el ejecutable
es nuevo y todavía no tiene reputación. La forma legítima de quitarlo es firmar
el código con un certificado de Code Signing; los builds se firman
automáticamente cuando el certificado está configurado. Un certificado **EV**
suele eliminar el aviso casi de inmediato; con un **OV** Windows puede seguir
mostrándolo hasta que el archivo gane reputación.

Puedes comprobar la firma de un archivo descargado con:

```powershell
signtool verify /pa Vaporeon-Installer.exe
```

## Datos

Toda la configuración, skins, instancias y archivos del juego se guardan en:

```text
%APPDATA%\.vaporeon
```

El desinstalador no borra esa carpeta.
