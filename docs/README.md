# Material de Redes

Página con todo el material de estudio (guías, presentaciones, diagramas y PDFs), publicada con GitHub Pages.

## Agregar material nuevo

1. Copia los archivos a la carpeta `material/`.
2. Ejecuta: `python3 generar_indice.py` (actualiza `index.html`).
3. Sube los cambios:
   ```bash
   git add .
   git commit -m "Agregar material"
   git push
   ```

Los archivos repetidos (mismo contenido) se muestran una sola vez.
Las etiquetas por tema (OSPF, BGP, EIGRP…) se asignan según el nombre del archivo;
puedes agregar más en la lista `TEMAS` de `generar_indice.py`.

## Publicar en GitHub Pages (primera vez)

1. Crea un repositorio público en GitHub (por ejemplo `material-redes`).
2. En esta carpeta:
   ```bash
   git init
   git add .
   git commit -m "Primera versión"
   git branch -M main
   git remote add origin https://github.com/TU_USUARIO/material-redes.git
   git push -u origin main
   ```
3. En GitHub: **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**.
4. En 1–2 minutos estará en `https://TU_USUARIO.github.io/material-redes/`.
