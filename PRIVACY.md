# Privacy Policy — Waypack

**Last updated: 22 November 2026**

*[Versión en español más abajo.](#política-de-privacidad--waypack)*

Waypack is an app for organizing your trips and your packing that **works offline**.

**We collect no data.** Waypack contains no ads or trackers, and uses no analytics services or
third-party SDKs. The developer has no server, and **cannot** see, receive, store or retrieve
anything you write.

**What Waypack connects to, and when.** Waypack uses the Internet for three things only. The first
two carry nothing from your trips; the third is off unless you turn it on, and carries only the
rounded area of a plan:

- **The map.** When you look at the map or save an area to use it offline, Waypack downloads the map
  images (tiles) from **OpenFreeMap** (tiles.openfreemap.org), with OpenStreetMap data. That request
  tells OpenFreeMap which area of the map is being viewed and, like any connection, carries your IP
  address. OpenFreeMap handles it under its own privacy policy. You can turn the map's Internet off
  in **Settings → Offline maps**; the map then shows only the areas you saved.
- **A shared map link, if you ask.** If you share a Google Maps, Apple Maps or Mapy link with
  Waypack and tap «Get it from…», Waypack asks that service where the link points and, for a shared
  Google list, which places it has. Only the link travels, plus your IP address as in any
  connection; no cookies and no account. If you don't tap it, nothing connects.
- **The weather where you are going, if you turn it on** (since version 1.4.0). It is off by
  default. Once you turn it on in **Settings → Outside the app** or from the card in Days, Waypack
  asks **Open-Meteo** (api.open-meteo.com) for the forecast and time zone of each plan's area. What
  travels is that area **rounded to about 10 km** (a tenth of a degree), plus your IP address as in
  any connection — never the plan's name, its dates or anything else in it. No cookies and no
  account. Open-Meteo handles the request under its own privacy policy. The forecast is kept on your
  phone, encrypted. Turning the setting off stops the requests.

Nothing else goes out: Waypack's connections are limited, inside the app, to those servers alone.

**Your data stays on your device.** Everything you enter — trips, packing lists, quantities, bags,
people, places, documents, attachments and any cover photos you choose — is stored **only in your
device's local storage**, encrypted.

**Backups: on by default where Google backup exists, and yours to change.** On phones with Google
Play Services, Waypack turns on the Google backup when you finish the welcome screen. On phones
without them nothing is turned on. You can change it at any time in **Settings → Backup**:

- **Google backup** (the default on phones with Google Play Services). Waypack places one encrypted backup file in a private folder, and Android's own
  system backup uploads it to your Google account together with the rest of your phone's backup.
  This is the only setting under which anything you wrote leaves your device. What travels is a
  file, encrypted, that Android additionally encrypts with your screen lock before uploading; the
  developer never sees it and has no access to your Google account. **This option only exists on
  phones that have Google Play Services**, so on GrapheneOS or a de-Googled phone it is not offered.
- **A folder you choose.** Waypack writes an encrypted backup into a folder you pick, using a
  password you pick. Waypack itself never uploads anything; if that folder happens to be synced by
  another app you have installed, the sync is that app's doing and under your control.
- **No, thanks.** Nothing leaves your device automatically. This is what you get on phones without
  Google Play Services, and on any phone as soon as you choose it.

**What never leaves, under any setting.** The encrypted database itself, your settings, your cover
photos and your attachments are excluded from every system backup and from phone-to-phone transfer.

**The backup upload is not Waypack's doing.** In the Google option the upload is performed by the
Android operating system, not by the app, and the app's own connections (the map, the links and the
weather, above) never carry your data beyond what is described there.

**Your plans in your phone's calendar, if you turn it on** (since version 1.4.0). It is off by
default. Turned on in **Settings → Outside the app**, Waypack asks for calendar permission and
creates a calendar called «Waypack» that is **local to your phone**: no account syncs it, so it does
not go to Google or anywhere else. It holds one all-day event per dated plan with the plan's name
only (with the app lock on, not even that). Like any calendar on your phone, other apps you have
allowed to read your calendar can see it. Turning the setting off deletes that calendar. Waypack
does not read your other calendars.

**Your location, only when you ask.** «Nearby» and «I'm here» in Places ask for your location at the
moment you use them, never at start-up. It is read once on your phone, without Google Play
Services, used for that one thing and **not stored**. Waypack never asks for background location.
Everything works without granting it.

**Dictation.** Adding items by voice uses your phone's speech service, not Waypack: Waypack has no
microphone permission and only receives the text. Depending on how your phone is set up, that
service may process the audio online; Waypack tells you so before the first use.

**No accounts.** No sign-up or login is required.

**What you choose to send.** If you export a backup or a trip file, or open an attachment in another
app, that file goes wherever you send it. That is your action and your choice; Waypack neither
uploads nor keeps a copy.

**Deletion.** If you uninstall the app or clear its data in Android settings, that information is
removed from your device. Switching the backup setting to «No, thanks» deletes the backup file from
your phone immediately, so nothing further is uploaded. A copy already stored in **your** Google
account is deleted from your phone's own backup settings — Waypack cannot reach it.

**Google Play.** Download and distribution via Google Play is subject to Google's privacy policy;
that processing is done by Google, not by Waypack.

**Changes.** If a future version adds features that process data, we will update this policy before
enabling them.

**Contact:** bymaksymdev@gmail.com

---

# Política de privacidad — Waypack

**Última actualización: 22 de noviembre de 2026**

Waypack es una aplicación para organizar tus viajes y tu equipaje que **funciona sin conexión**.

**No recopilamos ningún dato.** Waypack no contiene anuncios ni rastreadores, y no utiliza servicios
de analítica ni SDK de terceros. El desarrollador no tiene ningún servidor y **no** puede ver,
recibir, almacenar ni recuperar nada de lo que escribes.

**A qué se conecta Waypack, y cuándo.** Waypack usa Internet para tres cosas y nada más. Las dos
primeras no llevan nada de tus viajes; la tercera está apagada salvo que la enciendas, y solo lleva
la zona redondeada de un plan:

- **El mapa.** Al mirar el mapa o al guardar una zona para usarla sin conexión, Waypack pide las
  imágenes del mapa (teselas) a **OpenFreeMap** (tiles.openfreemap.org), con datos de
  OpenStreetMap. Esa petición dice qué zona del mapa se está viendo y, como cualquier conexión,
  lleva tu dirección IP. OpenFreeMap la trata según su propia política de privacidad. Puedes apagar
  el uso de Internet del mapa en **Ajustes → Mapas sin conexión**; entonces el mapa solo enseña las
  zonas que hayas guardado.
- **Un enlace de mapa compartido, si lo pides.** Si compartes con Waypack un enlace de Google Maps,
  Apple Maps o Mapy y tocas «Traer de…», Waypack le pregunta a ese servicio a dónde lleva el enlace
  y, si es una lista compartida de Google, qué sitios tiene. Solo viaja el enlace y, como en
  cualquier conexión, tu dirección IP; sin cookies ni cuenta. Si no lo tocas, no se conecta.
- **El tiempo del destino, si lo enciendes** (desde la versión 1.4.0). Viene apagado. Cuando lo
  enciendes en **Ajustes → Fuera de la app** o desde la tarjeta de Días, Waypack le pide a
  **Open-Meteo** (api.open-meteo.com) la previsión y la zona horaria de la zona de cada plan. Lo que
  viaja es esa zona **redondeada a unos 10 km** (una décima de grado) y, como en cualquier conexión,
  tu dirección IP — nunca el nombre del plan, sus fechas ni nada más de él. Sin cookies ni cuenta.
  Open-Meteo trata la petición según su propia política de privacidad. La previsión se guarda en tu
  teléfono, cifrada. Al apagar el ajuste, dejan de hacerse las peticiones.

No sale nada más: las conexiones de Waypack están limitadas, dentro de la app, a esos servidores y a
ninguno más.

**Tus datos se quedan en tu dispositivo.** Todo lo que introduces —viajes, listas de equipaje,
cantidades, bolsas, personas, lugares, documentos, adjuntos y las fotos de portada que elijas— se
guarda **únicamente en el almacenamiento local de tu dispositivo**, cifrado.

**Las copias de seguridad: activadas por defecto donde existe la copia de Google, y las cambias
tú.** En los teléfonos con Google Play Services, Waypack activa la copia de Google al terminar la
pantalla de bienvenida. En los que no los tienen no se activa nada. Puedes cambiarlo cuando quieras
en **Ajustes → Copia de seguridad**:

- **Copia de Google** (la opción por defecto en teléfonos con Google Play Services). Waypack deja un fichero de copia cifrado en una carpeta privada, y la copia
  del propio sistema Android lo sube a tu cuenta de Google junto con el resto de la copia de tu
  teléfono. Es la única opción con la que algo de lo que has escrito sale de tu dispositivo. Lo que
  viaja es un fichero cifrado, que Android además cifra con el bloqueo de tu pantalla antes de
  subirlo; el desarrollador no lo ve nunca y no tiene ningún acceso a tu cuenta de Google. **Esta
  opción solo existe en teléfonos con Google Play Services**, así que en GrapheneOS o en un móvil
  desgooglizado no se ofrece.
- **Una carpeta que tú elijas.** Waypack escribe una copia cifrada en la carpeta que le indiques, con
  una contraseña que eliges tú. Waypack no sube nada por su cuenta; si esa carpeta la sincroniza otra
  app que tengas instalada, esa sincronización es cosa de esa app y está bajo tu control.
- **No, gracias.** No sale nada de tu dispositivo de forma automática. Es lo que tienes en los
  teléfonos sin Google Play Services, y en cualquiera en cuanto lo elijas.

**Lo que no sale nunca, elijas lo que elijas.** La base de datos cifrada, tus ajustes, tus fotos de
portada y tus adjuntos quedan excluidos de toda copia del sistema y de la transferencia entre
móviles.

**La subida de la copia no la hace Waypack.** En la opción de Google, la subida la hace el sistema
operativo Android, no la app, y las conexiones de la propia app (el mapa, los enlaces y el tiempo,
más arriba) no llevan nunca tus datos más allá de lo que se cuenta ahí.

**Tus planes en el calendario del móvil, si lo enciendes** (desde la versión 1.4.0). Viene
apagado. Al encenderlo en **Ajustes → Fuera de la app**, Waypack pide el permiso de calendario y crea
un calendario llamado «Waypack» que es **local de tu teléfono**: ninguna cuenta lo sincroniza, así
que no va a Google ni a ningún otro sitio. Tiene un evento de día entero por cada plan con fecha,
solo con el nombre del plan (con la puerta de la app echada, ni eso). Como cualquier calendario de
tu teléfono, lo ven las apps a las que hayas dejado leer tu calendario. Al apagar el ajuste, ese
calendario se borra. Waypack no lee tus otros calendarios.

**Tu ubicación, solo cuando la pides.** «Cerca» y «Estoy aquí», en Lugares, piden tu ubicación en el
momento de usarlos, nunca al arrancar. Se lee una vez en tu teléfono, sin Google Play Services, se
usa para eso y **no se guarda**. Waypack no pide nunca la ubicación en segundo plano. Todo funciona
sin concederla.

**El dictado.** Añadir cosas por voz usa el servicio de voz de tu teléfono, no Waypack: Waypack no
tiene permiso de micrófono y solo recibe el texto. Según cómo tengas el teléfono, ese servicio puede
procesar el audio por Internet; Waypack te lo dice antes del primer uso.

**Sin cuentas.** No necesitas registrarte ni iniciar sesión.

**Lo que mandas tú.** Si exportas una copia de seguridad o un fichero de viaje, o abres un adjunto en
otra app, ese fichero va a donde tú lo mandes. Eso es una acción tuya y una decisión tuya; Waypack ni
lo sube a ningún sitio ni se queda una copia.

**Borrado.** Si desinstalas la app o borras sus datos desde los ajustes de Android, esa información
desaparece de tu dispositivo. Cambiar la copia de seguridad a «No, gracias» borra el fichero de copia
del teléfono en ese momento, así que deja de subirse nada. Una copia que ya esté en **tu** cuenta de
Google se borra desde los ajustes de copia de tu propio teléfono — Waypack no puede llegar a ella.

**Google Play.** La descarga y distribución a través de Google Play está sujeta a la política de
privacidad de Google; ese tratamiento lo realiza Google, no Waypack.

**Cambios.** Si en el futuro alguna versión añadiera funciones que traten datos, actualizaríamos esta
política antes de activarlas.

**Contacto:** bymaksymdev@gmail.com
