# Infinite Canvas — HTML + CSS + JavaScript

Proyecto estático, sin React y sin Next.js. Vercel lo puede servir directamente.

## Probar en local
Abre `index.html` con Live Server en VS Code, o:
`python -m http.server 5500`
y entra en `http://localhost:5500`.

## Supabase
Edita `js/app.js` al principio:
```js
const cfg={url:"https://TU-PROYECTO.supabase.co",key:"TU_ANON_PUBLIC_KEY"};
```
Usa solamente la clave `anon public`, nunca `service_role`.

Después ejecuta `supabase/schema.sql` en Supabase > SQL Editor.

## Vercel
1. Sube esta carpeta a GitHub.
2. En Vercel: Add New Project > importa el repositorio.
3. Framework Preset: Other.
4. Build Command: vacío.
5. Output Directory: vacío.
6. Deploy.

También puedes instalar Vercel CLI y ejecutar `vercel --prod`.

## Dominio
Vercel > Project > Settings > Domains > añade tu dominio.

## Funciones incluidas
Canvas infinito, pan, zoom, texto, notas, imágenes, selección múltiple, Ctrl+A/C/V/D/S, undo/redo, rotación, resize de imágenes, marcos, conectores, proyectos, miniaturas, guardado local, Supabase opcional, login y Storage, impresión PDF.

Nota: esta primera versión deja el PNG como siguiente mejora; el PDF usa la impresión del navegador. Para producción avanzada conviene implementar exportación real con imágenes, conectores inteligentes, snapping y colaboración en tiempo real.
