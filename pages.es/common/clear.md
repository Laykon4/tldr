# clear

> Limpia la pantalla de la terminal.
> Más información: <https://manned.org/clear>.

- Limpia la pantalla de la terminal (equivale a presionar `<Ctrl l>` en la interfaz de línea de comandos Bash):

`clear`

- Limpia la pantalla pero mantiene el buffer de desplazamiento:

`clear -x`

- Indica el tipo de terminal a limpiar (por defecto se utiliza el valor de la variable de entorno `TERM`):

`clear -T {{tipo_de_terminal}}`

- Muestra la versión de `ncurses` utilizada por `clear`:

`clear -V`
