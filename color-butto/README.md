# Getting Started with 'Testing library'

```
import { render, screen } from '@testing-library/react';
```

- [] la funcion **_render_** crea un virtual DOOM para argumentos jsx
- [] Mientras que la funcion **_screen_** nos da acceso a ese virtual DOOM que fue creado.

screen tiene muchos metodos por ejemplo
- _getByText_ el cual encontrara un cualquier texto mostrado por el DOOM

- recibe como argumento un string especifico o una funcion regular para que getByText haga una busqueda mas especifica

# assertions
- las afirmaciones determinan si es exitosa o fallida la prueba realizada 

```
expect(some).toBeInTheDocument();
```

_toBeInTheDocument_ verifica que algo exista dentro del documento o de nuestra vista.

expect(some).toBeInTheDocument(); = se espera que some este en el documento

## TDD (Test-Driven Development)

- Se escriben las pruebas antes de escribir el codigo
    - escribimos el codigo para que pase las pruebas
- "red-green" testing
    - Se crean test que fallen antes de escribir el codigo
    - Se escribe el codigo
    - Se escriben las pruebas que van a pasar el test
