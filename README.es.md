<div align="center">

# Waypack

**Un organizador de equipaje y viajes que no puede conectarse.**

[Descargar el APK](https://github.com/bymaksym/waypack/releases/latest) ·
[Contar un fallo](https://github.com/bymaksym/waypack/issues/new?template=bug_report.yml) ·
[Política de privacidad](PRIVACY.md) ·
[Read in English](README.md)

</div>

---

Waypack organiza tus viajes y lo que llevas en ellos —por días, por bolsas y por personas— y todo se
queda en tu móvil. Sin cuenta, sin sincronización, sin servidor, sin anuncios y sin analítica.

No es «prometemos que no mandamos tus datos». **La app no tiene con qué mandarlos**: se publica con
el permiso de `INTERNET` explícitamente quitado del manifiesto, así que aunque lo intentara, Android
se lo impediría.

> Este repositorio es la casa de las **versiones, los fallos y las conversaciones** de Waypack. El
> código de la app no es público (todavía). Ver [¿Waypack es código abierto?](#waypack-es-código-abierto)
> más abajo.

## Qué hace

**El equipaje**
- Listas por viaje, por categorías, por días y por bolsas.
- Doble check —*preparado* y *en la bolsa*— y un *¿está listo?* para lo que puede estar guardado y
  no servir, como una cámara con la batería a cero.
- Unidades de verdad (unidades, pares, ml, g): la bolsa de líquidos se suma sola.
- Bolsas dentro de bolsas: la maleta grande se queda en el coche y de ella sale la de una noche.
- Personas dentro del viaje y material de grupo, para que en una salida de cinco no aparezcan dos
  filtros de agua y el bidón que no lleva nadie no se quede en casa.

**Tu material**
- Un inventario que no es de ningún viaje: lo que pesa cada cosa, por estaciones. Se llena solo
  según vas pesando cosas dentro de un plan.
- El material con vida: primer uso, caídas, caducidades de verdad, mantenimiento y qué se rompió.
  Solo resta fechas; no decide por ti.
- Tus propias plantillas, guardadas desde cualquier plan, además de las de fábrica.

**Para la montaña**
- El agua de la ruta, la luz de día que queda, comida y gas.
- Botiquín según la duración y la actividad, y el material que pide cada perfil (verano, invierno,
  glaciar, roca, agua, bici).
- Boletín de aludes, que tecleas tú y caduca solo.
- Barómetro y altímetro, con lo que el móvil puede saber y lo que no.

**El viaje entero**
- Tramos, lugares por día, documentos y adjuntos: el pasaporte y el track viven con el viaje y no en
  «Descargas» entre otros cuarenta ficheros.
- Copia de seguridad cifrada con tu contraseña, y un fichero para pasarle el plan a quien viaja
  contigo.
- Español, inglés, ruso y ucraniano, con selector de idioma dentro de la app.
- Bloqueo de capturas, ocultar en recientes y bloqueo de la app con la credencial del móvil.

## La privacidad, en forma comprobable

| | |
| --- | --- |
| Permisos | **Tres, y ninguno llega a tus datos ni a la red:** `USE_BIOMETRIC` y `USE_FINGERPRINT`, para que el bloqueo de la app pueda pedirle a tu móvil que te autentique, y un permiso de firma del propio paquete de Waypack que solo *restringe* el acceso a uno de sus receptores. `INTERNET` está quitado a propósito del manifiesto |
| Base de datos | Cifrada con SQLCipher |
| Portadas | Cifradas con el Keystore de Android |
| Copias de seguridad | Cifradas con una contraseña que eliges tú |
| Copia automática de Android | Apagada (`allowBackup=false`): nada sale en una copia del sistema |
| Google Play Services | Ni se usan ni hacen falta. Funciona en GrapheneOS y móviles desgooglizados |
| Analítica, informes de fallo, anuncios | Nada |

Dentro de la app, **Ajustes → Privacidad → «Verifícalo tú mismo»** enseña los permisos que declara la
copia en marcha y su huella de firma, para que puedas comprobar todo esto sin fiarte de esta página.

## Instalar

**Necesita Android 8.0 (API 26) o superior.**

- **Descarga directa**: coge `app-release.apk` de la
  [última versión](https://github.com/bymaksym/waypack/releases/latest) y ábrelo.
- **[Obtainium](https://github.com/ImranR98/Obtainium)**: apúntalo a este repositorio y él se encarga
  de avisarte de las versiones nuevas. El nombre del fichero no cambia entre versiones a propósito,
  justo para que eso siga funcionando.

### Comprobar lo que has descargado

Cada versión publica dos huellas. Las dos valen treinta segundos:

```
# 1. El fichero es el que se publicó
sha256sum app-release.apk        # tiene que coincidir con el .sha256 de la release

# 2. Lo firmó la clave de Waypack y no lo ha reempaquetado otro
apksigner verify --print-certs app-release.apk
```

La segunda es la que te enseña la app en «Verifícalo tú mismo». Si los tres valores —las notas de la
versión, tu descarga y la app en marcha— no coinciden, lo que has instalado no ha salido de aquí.

## Contar un fallo o pedir algo

- 🐞 [Informe de fallo](https://github.com/bymaksym/waypack/issues/new?template=bug_report.yml)
- 💡 [Idea o petición](https://github.com/bymaksym/waypack/issues/new?template=feature_request.yml)
- 💬 [Discusiones](https://github.com/bymaksym/waypack/discussions): dudas, cómo organizas tu
  equipaje, y todo lo que no sea un defecto
- 🔒 Un problema de seguridad va por [SECURITY.md](SECURITY.md), **no** en un issue público

Una petición que aquí importa más que en otras apps: **no pegues tus viajes en un issue**. Las
capturas y las exportaciones llevan nombres, fechas y lugares reales. Nada de eso ayuda a arreglar un
fallo, y este repositorio es público. Ver [CONTRIBUTING.md](CONTRIBUTING.md).

## ¿Waypack es código abierto?

Hoy no. Este repositorio tiene las versiones, los fallos y la documentación; el código de la app vive
en un repositorio privado.

Es una decisión sobre el código, no sobre la promesa: nada de lo de arriba depende de creerse al
autor. La lista de permisos la hace cumplir Android, la tarjeta de «Seguridad de los datos» de Google
Play la rellena Google, y la huella de la firma se comprueba desde la propia app. Si el código se
abre más adelante, será con una licencia copyleft (GPL o AGPL) y se anunciará aquí.

## Licencia

La app se distribuye compilada; todos los derechos reservados. Los documentos de este repositorio
—este README, la política de privacidad— se pueden citar libremente.
