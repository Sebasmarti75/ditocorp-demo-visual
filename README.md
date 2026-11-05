# DITOCORP System — DEMO visual B5.1

Muestra estática de DITOCORP System. **Publicación pública autorizada por DITOCORP el 5 de noviembre de 2026.**

Referencia exclusiva: commit funcionalmente aprobado `55aecdfc984683d8defe098f510acdd0cec49757`. Corte de la presentación: 5 de noviembre de 2026. No incorpora B5.2.

## Qué contiene

23 páginas HTML: Mi trabajo, Coordinación, Tareas y cuatro fichas, dos filtros ilustrativos, Solicitudes y dos fichas, formulario de nueva Solicitud desactivado, Documentos, Versiones, Historial, Bandeja, Entrada, Asuntos y dos fichas, Clientes y recorrido guiado.

Las pantallas se renderizaron con los componentes reales aprobados de B5.1 y datos nuevos exclusivamente ficticios. Se retiraron React, Next.js, scripts, llamadas de red y operaciones. Se conservaron los estilos originales; una hoja adicional adapta botones de navegación a enlaces y muestra los avisos de demostración. No es otro CRM ni una implementación de las reglas de negocio.

La vista de Clientes conserva el alcance de consulta del perfil ficticio mostrado. La confirmación de Cliente/contratación exige capacidades específicas en el sistema funcional. No se incorporó una pantalla de ofertas, contratos, Gmail, WhatsApp o Drive real. Los estados comerciales visibles corresponden al seguimiento aprobado de Solicitud.

## Componentes aprobados reutilizados

Se reutilizó su HTML renderizado, no sus scripts ni acceso a datos:

| Componente B5.1 | Pantallas de referencia |
|---|---|
| page.tsx | Estructura general, menú, Asuntos, Clientes y ficha de asunto. |
| RequestWorkspace | Solicitudes, formulario manual, ficha, procedencia e historial. |
| OperationsWorkspace / MatterOperations / TaskList | Mi trabajo, Coordinación, control de asunto, filtros y tareas. |
| EntryWorkspace | Bandeja, clasificación y procedencia SourceEvent. |
| DocumentWorkspace | Documentos, manifiestos, versiones y auditoría documental. |
| globals.css | Tipografía de sistema, colores, distribución y estilos aprobados. |

Una exportación directa de Next.js conservaría las llamadas a la API presentes en el frontend. Adaptar transporte, datos y acciones añadiría trabajo; esta muestra HTML evita esa dependencia y conserva las pantallas reales. No se copió código backend ni se publicó el proyecto original.

## Navegación y simulación

- Los enlaces permiten consultar pantallas y fichas coherentes con cada ejemplo.
- Los desplegables de información se abren con HTML nativo.
- Coordinación permite abrir dos ejemplos de filtro: vencidas y bloqueadas.
- Los formularios, búsqueda libre, otros filtros, guardado, asignación, carga y confirmación están desactivados.
- Las dos descargas de ejemplo son archivos TXT ficticios incluidos en assets. No proceden del almacenamiento del sistema.
- No hay autenticación, permisos efectivos, cookies, localStorage, IndexedDB, trabajadores ni persistencia.
- Las cifras y fechas son una fotografía ilustrativa de la fecha de corte, no indicadores en vivo.

## Archivos para GitHub Pages

```text
/
├── index.html                  # Mi trabajo
├── recorrido.html              # Contexto y recorrido para directivos
├── coordinacion.html
├── solicitudes.html
├── solicitud.html
├── solicitud-2.html
├── nueva-solicitud.html
├── tareas.html
├── tarea.html
├── tarea-2.html
├── tarea-3.html
├── tarea-4.html
├── tareas-vencidas.html
├── tareas-bloqueadas.html
├── documentos.html
├── versiones.html
├── auditoria.html
├── bandeja.html
├── entrada.html
├── asuntos.html
├── asunto.html
├── asunto-2.html
├── clientes.html
├── assets/
│   ├── ditocorp-b51.css
│   ├── demo.css
│   ├── documento-ficticio-v1.txt
│   └── documento-ficticio-v2.txt
├── robots.txt
├── .nojekyll
└── README.md
```

No requiere instalación, npm, compilación, variables de entorno ni backend. Todos los enlaces son relativos y admiten el prefijo de un repositorio de GitHub Pages. No se incluye CNAME ni configuración DNS.

## Revisar localmente

Abrir `recorrido.html` en un navegador o servir esta carpeta desde un servidor estático local. Por ejemplo, desde la carpeta del proyecto:

```sh
python3 -m http.server 13100 --bind 127.0.0.1
```

En ese caso, entrar a `http://127.0.0.1:13100/recorrido.html`. El servidor es solo para vista previa de archivos; la DEMO no necesita API. La vista previa que acompaña esta entrega también verifica el prefijo `/ditocorp-demo-visual/` y bloquea rutas ocultas.

## Seguridad y privacidad

Todo lo que se publique en GitHub Pages será público. Los nombres son ficticios, los correos usan example.test, los identificadores se crearon para esta presentación y los textos descargables no tienen validez legal. No se copiaron bases, credenciales, capturas históricas ni documentos internos.

No hay JavaScript, dependencias de CDN, fuentes externas, analítica, llamadas a backend ni enlaces institucionales. Cada HTML incluye una política CSP que impide scripts, conexiones, envío de formularios y recursos externos.

robots.txt y noindex solicitan que no se indexe: **no son protección de acceso ni garantizan confidencialidad**. No existe contraseña simulada en el navegador. No introducir información real en futuras revisiones.

## Verificación local realizada

- 23 páginas, 46 revisiones de Chrome: escritorio 1440 px y móvil 390 px.
- Sin errores JavaScript/consola ni desbordamiento horizontal.
- Enlaces y recorrido Solicitud → Documentos → Versiones verificados bajo el prefijo de repositorio.
- Cero scripts, controles de escritura activos o solicitudes a API/servicios externos.
- Inspección de todos los archivos: sin secretos, rutas privadas, identificadores históricos ni código backend.
- CSS base idéntico al commit B5.1. Archivos versionables de B5.1 y B5.2 conservados byte por byte.
- Pruebas de apertura, desplegables nativos y descarga de los dos ejemplos TXT.

## Publicación autorizada en GitHub Pages

1. DITOCORP autorizó publicar exclusivamente esta muestra estática, separada del sistema original.
2. Crear un repositorio GitHub independiente, propuesto `ditocorp-demo-visual`, con estos archivos estáticos. No publicar el repositorio original ni su historial.
3. Crear el commit y push exclusivamente del repositorio de la DEMO autorizado.
4. En Settings → Pages, seleccionar publicación desde la rama main y carpeta raíz. `.nojekyll` evita procesar el sitio con Jekyll.
5. Verificar HTTPS, enlaces bajo el prefijo del repositorio, fichas, descargas ficticias y ausencia de solicitudes a API/servicios externos.
6. Compartir la URL de Pages solamente después de comprobar el resultado.

GitHub Pages permite este esquema gratuito mediante un repositorio público. La URL inicial será la asignada por GitHub; no es necesario modificar DNS ni utilizar el VPS.

Referencias oficiales:
- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://nextjs.org/docs/app/guides/static-exports

Repositorio de publicación: `Sebasmarti75/ditocorp-demo-visual`. La publicación se limita a los archivos estáticos de esta carpeta; B5.1 y B5.2 permanecen fuera de este repositorio.
