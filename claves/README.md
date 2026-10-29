# Claves y APIs — tu bóveda

Aquí se lleva el control de tus claves (API de HubSpot, etc.) de forma **segura y sencilla**.

## La regla simple
**Las claves nunca se escriben en texto dentro de los archivos que se sincronizan a la nube**,
porque cualquiera con acceso a la carpeta podría leerlas. En su lugar:

- El **valor** de la clave vive en un lugar seguro (ver abajo).
- Aquí solo se guarda el **índice**: qué claves tienes y dónde están (`indice-claves.md`).

## Dónde vive el valor de la clave (elige una)
1. **Gestor de contraseñas (recomendado, gratis):** Bitwarden. Guardas ahí la clave y en
   `indice-claves.md` anotas en qué elemento quedó. Simple y seguro.
2. **Archivo local sin sincronizar:** un archivo `.env` en esta carpeta, pero **excluido**
   de Google Drive/OneDrive. Útil si quieres que la IA la lea directo. Copia `.env.ejemplo`
   como `.env` y pega ahí los valores. (Pídele a la IA que te ayude a excluirlo del sincronizado.)

## Cómo se usa
Solo dile a tu asistente: *"guarda mi clave de servicio de HubSpot"*. Él te guía para
ponerla en el lugar seguro y deja la referencia anotada en `indice-claves.md`.
Nunca te pedirá pegar la clave en un chat ni en un archivo que se sincronice.
