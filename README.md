# Company profile 

## Validaciones de los campos del formulario:
**Email:** 
El `nombre del usuario` : admite mayusculas, minusculas y números (0-9).

El dominio está compuesto por dos subgrupos:

La `organización` (o el nombre del Servidor de la Organización): un mínimo de 3 caracteres alfanuméricos.

El `tipo` (característica que define la funcionalidad del dominio): un mímino de tres caracteres (a-z).

Regex de validación:
``` js
/([A-Z|a-z|0-9](\.|_){0,1})+[A-Z|a-z|0-9]\@([A-Z|a-z|0-9])+((\.){0,1}[A-Z|a-z|0-9]){2}\.[a-z]{2,3}$/

```
**Teléfono:**
El campo `telefono` valida que tenga una longitud de nueve dígitos y debe empezar por (6|7)

Regex de validación:
``` js
/^(6|7)([0-9]*){8}/
```
**Website (URL):**
El campo `URL` valida los siguentes tipos rutas:
- `www.google.com`
- `http://www.google.com`
- `mailto:somebody@google.com`
- `somebody@google.com`
- `www.url-with-querystring.com/?url=has-querystring`

Regex de validación:
``` js
/((([A-Za-z]{3,9}:(?:\/\/)?)(?:[-;:&=\+\$,\w]+@)?[A-Za-z0-9.-]+|(?:www.|[-;:&=\+\$,\w]+@)[A-Za-z0-9.-]+)((?:\/[\+~%\/.\w-_]*)?\??(?:[-\+=&;%@.\w_]*)#?(?:[\w]*))?)/
```
