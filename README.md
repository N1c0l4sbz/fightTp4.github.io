# TP4 — Migración a PHP, SSI y SSR

**Proyecto:** Lunar MCA / Impact Fight  
**Materia:** Programación Web

## Objetivo del trabajo

Convertir el sitio estático de Impact Fight en un sitio PHP ejecutado desde el servidor local, reutilizando componentes comunes y conservando el diseño del catálogo de indumentaria, uniformes, accesorios, cursos y otras secciones.

## Desarrollo

Se utilizó PHP para presentar las páginas y separar la estructura compartida en archivos de `includes/`, como `header.php`, `nav.php` y `footer.php`. La intención de la modularización SSI es evitar copiar el mismo menú y pie en todas las vistas. La captura del explorador de VS Code confirma que esos archivos están presentes; para demostrar las llamadas `include` o `require` también es recomendable mostrar una de las páginas que los utiliza.

La página de inicio y la sección Cursos se abren desde `localhost`, con la navegación correspondiente resaltada. Esto permite mostrar el resultado final generado por el servidor (SSR). También se prepararon los archivos `.env`, `.env.example` y `.gitignore`; en la captura se ven sus nombres, aunque **no su contenido**, por lo que la exclusión de `.env` debe verificarse aparte.

## Evidencias del TP4

**1. Inicio del sitio en PHP.**

![Página inicial Impact Fight abierta en localhost](capturas/01-inicio-php.png)

**2. Carpeta `includes/` y archivos reutilizables.**

![Explorador de VS Code con archivos header php nav php y footer php](capturas/02-includes.png)

**3. Navegación activa en la sección Cursos.**

![Cursos con menú activo en rojo](capturas/03-navegacion-php.png)

**4. Archivos de configuración presentes.**

![Explorador con punto env ejemplo y gitignore](capturas/04-env-gitignore.png)

## Pruebas adicionales para completar la consigna

- Comprobar que al cambiar entre páginas se reutilizan el encabezado y el pie.
- Mostrar una línea de `include` o `require` dentro de un archivo `.php`.
- Verificar que `.env` esté ignorado realmente por Git y que `.env.example` no incluya credenciales.
- Revisar el título dinámico de cada página y el marcado del enlace activo.

## Conclusión

PHP permitió organizar el sitio en componentes reutilizables, facilitando el mantenimiento del diseño y dejando una base preparada para los módulos dinámicos de las siguientes clases.
