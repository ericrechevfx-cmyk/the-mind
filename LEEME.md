# The Mind (versión web)

Un solo archivo: `index.html`. No tiene servidor propio. Los móviles se conectan entre sí (WebRTC) usando el servidor gratuito de PeerJS solo para encontrarse.

## Publicarlo gratis (unos 2 minutos)

1. Entra en https://app.netlify.com/drop e inicia sesión (es gratis; sin cuenta, el enlace caduca en una hora).
2. Arrastra la carpeta `the-mind` (la que contiene `index.html`).
3. Netlify te da un enlace del tipo `https://algo.netlify.app`. Ese es el enlace del juego. Puedes cambiarle el nombre en *Site settings*.

También sirve GitHub Pages o cualquier hosting estático. Tiene que ser `https`.

## Cómo jugar

1. Uno pulsa **Crear partida**: le sale un código de 4 letras. Ese móvil es el anfitrión.
2. Los demás abren el enlace, ponen su nombre y el código (o abren el enlace de invitación, que ya trae el código).
3. El anfitrión elige el modo (con vidas o muerte súbita) y pulsa **Empezar**.
4. Cada nivel, todos ven sus cartas y pulsan **Listo**. Después, quien crea que le toca pulsa **Soltar** y lo confirma en el panel que aparece abajo.

## Cosas a tener en cuenta

- El móvil del anfitrión tiene que tener la página abierta. Si se bloquea la pantalla, la partida se pausa hasta que vuelva. La app pide mantener la pantalla encendida cuando el navegador lo permite.
- Si alguien recarga o se le cierra la página, al volver a abrir el enlace entra de nuevo con sus cartas.
- Para probar en un ordenador, cada pestaña cuenta como un jugador distinto.
