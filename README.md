<!-- # : título principal del README (lo primero que se ve en GitHub) -->
# Proyecto Django — Álvarez Cano César Damián

<!-- ## : subtítulo de la sección con el enlace a producción -->
## Demo en vivo (produccion)
<!-- la URL pública de tu Web Service u3s6-… en Render -->
https://u3s6-alvarez-cano-cesar-damian.onrender.com

<!-- ## : subtítulo con lo que se hizo esta semana -->
## Semana 6 — Autenticacion, sesiones y seguridad
<!-- primera línea de la descripción de la práctica -->
Registro/login/logout propios; cada usuario ve y edita solo
<!-- segunda línea de la descripción de la práctica -->
sus propios servicios (probado con usuario_a y usuario_b).

<!-- ## : subtítulo de la sección con la prueba de aislamiento -->
## Prueba de aislamiento
<!-- reemplaza el texto entre corchetes por la descripción de tu prueba -->
Se registraron dos cuentas (usuario_a y usuario_b) y cada una creó sus propios servicios.
Con la sesión de usuario_b, /servicios/ muestra únicamente los servicios de usuario_b.
Al escribir a mano /servicios/<id>/editar/ o /servicios/<id>/eliminar/ con el id de un servicio
de usuario_a, la app responde 404 y el servicio de usuario_a no se modifica ni se borra.

## Cómo correrlo localmente
1. Crear y activar un entorno virtual
2. `pip install -r requirements.txt`
3. Copiar `.env.example` a `.env` y completar con credenciales propias de Aiven (y una `SECRET_KEY` propia)
4. `python manage.py migrate`
5. `python manage.py runserver`
