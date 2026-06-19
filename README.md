# Catálogo Digital DU — Junio 2026

Catálogo estático de consulta para asesoras y clientes. Publicable en **GitHub Pages** o **Netlify** sin ningún backend.

---

## 📁 Estructura de archivos

```
catalogo-du/
├── index.html          ← Catálogo principal (diseño + lógica)
├── productos.json      ← Base de datos de productos
├── img/
│   ├── logo.png        ← Logo DU
│   └── productos/      ← Imágenes de productos (agregar aquí)
└── README.md
```

---

## 🚀 Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (ej. `du-catalogo`)
2. Sube todos los archivos de esta carpeta al repositorio
3. Ve a **Settings → Pages → Source** y selecciona la rama `main`, carpeta raíz `/`
4. Tu catálogo estará disponible en `https://tu-usuario.github.io/du-catalogo`

## 🚀 Publicar en Netlify

1. Crea una cuenta en [netlify.com](https://netlify.com)
2. Arrastra y suelta la carpeta `catalogo-du` en el panel de Netlify
3. En segundos tendrás un link para compartir

---

## ✏️ Cómo actualizar productos

Todos los cambios se hacen en `productos.json`. El HTML **no** necesita modificarse.

### Marcar producto como agotado
```json
{ "agotado": true }
```

### Agregar imagen a un producto
1. Sube la imagen a la carpeta `img/productos/`
2. En el JSON, actualiza el campo `"imagen"`:
```json
{ "imagen": "img/productos/mi-producto.jpg" }
```

### Agregar producto nuevo
Copia este bloque y agrega al array `"productos"`:
```json
{
  "id": "unico-123",
  "nombre": "Nombre del Producto",
  "referencia": "REF-CODIGO",
  "precio": 25000,
  "categoria": "Pestañas",
  "subcategoria": "Pestañas de fácil aplicación",
  "descripcion": "Descripción opcional del producto.",
  "imagen": "",
  "agotado": false
}
```

### Eliminar producto
Borra el bloque completo del producto en `productos.json` (solo si se confirma).

---

## 📋 Categorías disponibles

| Categoría | Subcategorías |
|-----------|--------------|
| **Accesorios** | Maletas, neceseres y carteras · Brochas, pinceles y accesorios · Hair Technology · Cepillos y peinillas · Cuidado del cabello · Herramientas y accesorios · Espejos |
| **Pestañas** | Pestañas de fácil aplicación · Pestañas pelo a pelo · Accesorios de pestañas |
| **Uñas** | Efectos y apliques · Stickers para uñas · Accesorios para uñas · Kits para uñas · Imanes |

---

## 🎨 Identidad visual

- Color principal: `#a6d8f2`
- Texto: `#ACADAF`
- Fuentes: Cormorant Garamond (titulares) + DM Sans (cuerpo)
