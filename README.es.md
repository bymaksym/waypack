<div align="center">

# Waypack

**Un organizador de equipaje y viajes: qué llevar, por días, por bolsas y por personas.**

[Descargar el APK](https://github.com/bymaksym/waypack/releases/latest) ·
[Contar un fallo](https://github.com/bymaksym/waypack/issues/new?template=bug_report.yml) ·
[Read in English](README.md)

</div>

---

Waypack organiza tus viajes y lo que llevas en ellos —por días, por bolsas y por personas—. Funciona
entero sin conexión, sin cuenta y sin anuncios.

> Este repositorio es la casa de las **versiones, los fallos y las conversaciones** de Waypack. El
> código de la app no es público (todavía).

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
- Tramos, lugares por día y documentos: el pasaporte es tuyo, no de un viaje, así que su caducidad
  está escrita en un solo sitio y Waypack la cruza con los viajes que vengan.
- Rutas: un `.gpx` o un `.kml` viaja con el viaje en vez de quedarse en «Descargas» entre otros
  cuarenta ficheros. Solo ficheros de ruta y hasta 10 MB — para un billete o una foto el gestor de
  ficheros del móvil lo hace mejor.
- Las copias las eliges tú: la del sistema con Google, un fichero automático en una carpeta tuya, o
  ninguna. Y encima la exportación a mano, con tu contraseña, para pasarle el plan a quien viaja
  contigo.
- Español, inglés, ruso y ucraniano, con selector de idioma dentro de la app.
- Bloqueo de capturas, ocultar en recientes y bloqueo de la app con la credencial del móvil.

## Instalar

**Necesita Android 8.0 (API 26) o superior.** No hacen falta los servicios de Google Play.

- **Descarga directa**: coge `app-release.apk` de la
  [última versión](https://github.com/bymaksym/waypack/releases/latest) y ábrelo.
- **[Obtainium](https://github.com/ImranR98/Obtainium)**: apúntalo a este repositorio y él se encarga
  de avisarte de las versiones nuevas. El nombre del fichero no cambia entre versiones a propósito,
  justo para que eso siga funcionando.

Para comprobar la descarga, compárala con el `.sha256` que se publica con cada versión:

```
sha256sum app-release.apk
```

## Contar un fallo o pedir algo

- 🐞 [Informe de fallo](https://github.com/bymaksym/waypack/issues/new?template=bug_report.yml)
- 💡 [Idea o petición](https://github.com/bymaksym/waypack/issues/new?template=feature_request.yml)
- 💬 [Discusiones](https://github.com/bymaksym/waypack/discussions): dudas, cómo organizas tu
  equipaje, y todo lo que no sea un defecto
- 🔒 Un problema de seguridad va por [SECURITY.md](SECURITY.md), **no** en un issue público

Por favor, **no pegues tus viajes en un issue**: las capturas y las exportaciones llevan nombres,
fechas y lugares reales, y este repositorio es público. Ver [CONTRIBUTING.md](CONTRIBUTING.md).

## ¿Waypack es código abierto?

Hoy no. Este repositorio tiene las versiones, los fallos y la documentación; el código de la app vive
en un repositorio privado. Si el código se abre más adelante, será con una licencia copyleft (GPL o
AGPL) y se anunciará aquí.

## Licencia

La app se distribuye compilada; todos los derechos reservados. Los documentos de este repositorio se
pueden citar libremente. La política de privacidad está en [PRIVACY.md](PRIVACY.md).
