# The Mind (versión web): guía completa

Versión web del juego de cartas **The Mind** para jugar con amigos, cada uno desde su móvil u ordenador.

- **Repositorio:** https://github.com/ericrechevfx-cmyk/the-mind
- **Archivo del juego:** `index.html` (es un único archivo, no hace falta nada más)

---

## 1. Por qué va lento o no carga el link de githack

El link `raw.githack.com/...` es un servicio gratuito de pruebas. Muchas veces va lento o no carga. **No es un problema del juego.** Hay que publicarlo en un sitio de verdad (punto 2). Tarda 1 minuto.

---

## 2. Publicarlo (elige una opción)

### Opción A: GitHub Pages (recomendada, el juego ya está subido)

1. Abre https://github.com/ericrechevfx-cmyk/the-mind/settings/pages
2. En **Source** elige **Deploy from a branch**.
3. En **Branch** elige **main** y la carpeta **/(root)**.
4. Pulsa **Save**.
5. Espera 1 o 2 minutos y recarga esa página. Arriba saldrá: *"Your site is live at…"*

**Link del juego:** https://ericrechevfx-cmyk.github.io/the-mind/

> Si al abrirlo sale un error 404, espera un par de minutos más. La primera publicación tarda un poco.

### Opción B: Netlify Drop

1. Descarga `index.html` (desde el repositorio: abre el archivo → botón **Download raw file**).
2. Crea una carpeta en el escritorio, por ejemplo `the-mind`, y mete dentro el `index.html`.
3. Entra en https://app.netlify.com/drop e inicia sesión (con Google vale, es gratis).
   - Sin iniciar sesión, el link se borra en 1 hora.
4. Arrastra la **carpeta** a la página.
5. Te da un link tipo `https://nombre-raro.netlify.app`. En **Site configuration → Change site name** puedes ponerle un nombre más bonito, por ejemplo `the-mind-eric`.

---

## 3. Cómo se juega con la app

1. **Una persona crea la partida.** Abre el link, pone su nombre y pulsa **Crear partida nueva**. Le sale un **código de 4 letras**, por ejemplo `BZPK`. Esa persona es el **anfitrión**.
2. **Los demás entran.** Abren el mismo link, ponen su nombre y el código, y pulsan **Entrar**.
   - El anfitrión también puede pulsar **Copiar enlace de invitación** y mandarlo por WhatsApp. Ese enlace ya lleva el código.
3. **El anfitrión elige el modo** y pulsa **Empezar partida**:
   - **Con vidas (oficial):** empezáis con tantas vidas como jugadores y 1 estrella.
   - **Muerte súbita:** un fallo y se acaba.
4. **Cada nivel:** todos miran sus cartas y pulsan **Listo**. La ronda empieza cuando todos están listos.
5. **Soltar carta:** cuando creas que te toca, pulsa **Soltar carta** y luego otra vez para confirmar. Siempre se suelta tu carta más baja.
6. La carta aparece en grande en todos los móviles:
   - Si estaba en orden, seguís jugando.
   - Si alguien tenía una más baja, sale **¡Fallo!** con quién tenía qué carta, y perdéis una vida.
7. Cuando no quedan cartas, **nivel superado**. Cualquiera pulsa **Repartir nivel X** para seguir.

### Reglas del juego

| | |
|---|---|
| Cartas | Del 1 al 100 |
| Nivel 1, 2, 3… | 1, 2, 3… cartas por persona |
| Niveles para ganar | 2 jugadores: 12 · 3 jugadores: 10 · 4 o más: 8 |
| Comunicación | Prohibido decir números. Vale decir cosas como «voy en pañales» o «el mío está jubilado» |
| Fallo | Perdéis 1 vida y se descartan todas las cartas más bajas que la soltada |
| Estrella ★ | Si **todos** pulsáis **Pedir estrella**, cada uno descarta su carta más baja |
| Premios | Al superar los niveles 2, 5 y 8 ganáis una ★. Al superar los niveles 3, 6 y 9, una ♥ |

---

## 4. Cosas importantes

- **El móvil del anfitrión es la "mesa".** Tiene que tener la página abierta todo el rato. Si se le bloquea la pantalla, la partida se pausa hasta que la desbloquee.
- **Si a alguien se le cierra la página**, al volver a abrir el link entra otra vez con sus mismas cartas.
- **Para probar en un ordenador**, cada pestaña cuenta como un jugador distinto.
- **Hace falta internet** en todos los móviles. Los móviles se conectan entre sí usando un servicio gratuito (PeerJS). No hay que configurar nada.

---

## 5. Si algo falla

| Problema | Solución |
|---|---|
| El link de githack va lento o no carga | Normal. Usa GitHub Pages o Netlify (punto 2) |
| GitHub Pages da error 404 | Espera 2 o 3 minutos después de pulsar Save y recarga |
| «No existe ninguna partida con el código…» | Revisa el código, o comprueba que el anfitrión sigue con la página abierta |
| «Reconectando…» arriba en rojo | Espera unos segundos; se reconecta solo. Si no, recarga la página |
| No se conecta en la red de casa | Prueba con datos móviles en vez de WiFi (algunos routers bloquean la conexión directa) |
| «La partida ya ha empezado» | No se puede entrar a mitad. El anfitrión puede pulsar Salir → **Volver a la sala** y empezar otra |
