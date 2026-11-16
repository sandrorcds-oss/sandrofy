SANDROFY — PWA PARA IPHONE 16e

1. En Windows, descomprime este ZIP en una carpeta.
2. Sube EL CONTENIDO de la carpeta Sandrofy_PWA (index.html, manifest.webmanifest, sw.js e icons/) a un alojamiento HTTPS gratuito. Recomendado: GitHub Pages. No subas las canciones.
   - En GitHub: nuevo repositorio (por ejemplo, sandrofy); Add file > Upload files; selecciona todos los archivos y la carpeta icons.
   - Settings > Pages > Deploy from a branch > main > /(root) > Save.
   - Espera a que GitHub Pages muestre tu dirección https://USUARIO.github.io/sandrofy/.
   - GitHub Pages suele requerir un repositorio público con cuenta gratuita; el código será visible, NO las canciones, que se importan directamente en el iPhone.
3. En iPhone abre esa dirección CON SAFARI; botón Compartir > Añadir a pantalla de inicio > Abrir como app > Añadir.
4. Abre Sandrofy desde su icono en la pantalla de inicio. Ve a Biblioteca e importa un archivo MP3 desde Archivos.
5. Ponlo a reproducir, bloquea el móvil, comprueba si sigue sonando; prueba la reproducción y pausa en pantalla bloqueada, y después varias pistas seguidas.
6. Después de la primera carga online, la interfaz queda cacheada y puede abrirse offline. Las canciones se guardan en IndexedDB del iPhone siempre que iOS mantenga esos datos.

IMPORTANTE: iOS no garantiza audio continuo en segundo plano para PWA. Safari puede suspender la web y existen incidencias en iOS 26. No se puede activar AVAudioSession nativo desde HTML. Si dejas de escuchar, prueba también abrir la dirección en Safari (sin instalar) para comparar.
NO abras index.html directamente desde Archivos esperando instalar una PWA: se requiere origen HTTPS para instalar el service worker.
No borres la app ni los datos de sitios web si quieres conservar las canciones importadas. Conserva una copia original de la música fuera de Sandrofy.
