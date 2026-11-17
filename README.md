# BUYACAR — Experiencia visual responsive basada en la referencia

## Ejecutar
Desde esta carpeta: `python -m http.server 8000` y abrir `http://localhost:8000`.

## Incluye
- Composición desktop inspirada en la referencia: barra superior, RobotCar a la izquierda, mensaje central, vehículo protagonista, categorías, catálogo de cuatro columnas, simulador lateral y bloque FUTURE LAB.
- Diseño móvil adaptado, con menú plegable, hero apilado, catálogo a dos columnas y chat flotante.
- 34 registros de vehículos transcritos del catálogo público BUYACAR consultado el 17-11-2026. Los listados marcados como vendidos se identifican como tales; validar inventario vigente antes de vender.
- Fotografías reales enlazadas desde las fichas oficiales BUYACAR para las unidades donde se recuperó imagen. Para algunas fichas sin imagen recuperable se usa una tarjeta con marca y modelo, sin asignarles fotos ajenas.
- RobotCar es visual y responde con reglas programadas; aún no es IA conectada.
- FUTURE LAB son conceptos visuales, no vehículos aéreos fabricados ni certificados.
- Revisar permisos para reutilizar fotografías del sitio oficial antes de publicar.

## Experiencia sonora de bienvenida
- Pantalla de entrada BUYACAR con botón "ENTRAR A BUYACAR".
- Al pulsarlo se inicia una pieza ambiental instrumental original sintetizada en el navegador mediante Web Audio API: cama armónica cinematográfica, tonos suaves y breve sonido de activación.
- Control flotante para silenciar/activar y ajustar volumen.
- No requiere MP3 ni música comercial de terceros.
- El audio requiere el gesto del visitante; no se fuerza al cargar la página por las restricciones de reproducción automática de los navegadores.

## Versión visual refinada (17-11-2026)
- Portada y hero rediseñados siguiendo la referencia BUYACAR enviada: RobotCar a la izquierda, mensaje central y vehículo/showroom a la derecha.
- La pantalla de bienvenida ahora presenta robot + automóvil + mensaje y CTA, manteniendo el arranque de música tras el clic.
- FUTURE LAB muestra tres tarjetas visuales independientes: AERION X1, VOLTERRA GT y ORION CARGO, con imágenes recortadas de la referencia suministrada. Son conceptos visuales, no vehículos fabricados.
- Los recortes locales se guardan en assets para evitar rutas externas en la portada.
- Se corrigió el logo para usar un archivo local y rutas relativas compatibles con GitHub Pages.
- Las imágenes remotas del catálogo conservan sus URLs oficiales; si alguna no carga por restricciones del sitio externo, la tarjeta muestra un respaldo visual en lugar del icono de imagen rota.


## Catálogo completo
- La página muestra automáticamente los 32 registros únicos disponibles en `vehicles.json`.
- Se eliminaron únicamente filas duplicadas idénticas; se conservaron listados del mismo modelo cuando cambian los datos o el precio.
- El catálogo carga todos los vehículos por defecto y permite filtrar por marca/modelo, categoría, rango de precio y ordenar.
- Si una fotografía alojada externamente deja de estar disponible, la tarjeta conserva su espacio y muestra una ficha gráfica de respaldo.
- Para probar localmente: `python -m http.server 8000` y abrir `http://localhost:8000`.
- Los precios y disponibilidad deben confirmarse con BUYACAR antes de publicar una oferta.
