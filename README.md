# 📋 Generador de Textos Legales

**IKEA Family & Ventajon** - Herramienta para generar textos legales de promociones financieras.

🔗 **Accede a la aplicación:** [https://gommez.github.io/textos-legales/](https://gommez.github.io/textos-legales/)

---

## 🚀 Características

- ✅ **Parser inteligente de Excel** - Extrae automáticamente plazos, TIN e importes mínimos
- ✅ **Parser de Word** - Extrae textos legales de documentos .docx
- ✅ **Generador de promociones** - Crea textos legales paso a paso
- ✅ **Biblioteca de campañas** - Acceso rápido a textos predefinidos
- ✅ **Datos compartidos** - Todos los usuarios ven los mismos datos
- ✅ **Sin servidor** - Funciona 100% en el navegador

---

## 👤 Para USUARIOS

Simplemente abre la aplicación y utiliza las funciones disponibles:
- **Crear promoción** - Genera textos legales paso a paso
- **Biblioteca** - Accede a campañas predefinidas

Los datos se cargan automáticamente desde el repositorio.

---

## 👨‍💼 Para el ADMINISTRADOR

### Actualizar los datos

1. **Abre la aplicación**
2. **Ve a Documentos** (📤)
3. **Sube los archivos** Excel y/o Word
4. **Click "Procesar y actualizar datos"**
5. **Click "📦 Exportar datos para GitHub"** → Se descargan `plazos.json` y `campanas.json`
6. **Sube esos archivos a GitHub** en la carpeta `/data/`

### Archivos soportados

| Tipo de archivo | Qué extrae |
|-----------------|------------|
| `Calculadora_Sin_Intereses_*.xlsx` | Plazos financiación 0% TIN |
| `Calculadora_Aplazado_*.xlsx` | Plazos con intereses (TIN variable) |
| `TEXTOS_LEGALES_*.docx` | Campañas y textos legales completos |

---

## 📁 Estructura del repositorio

```
/textos-legales/
├── index.html          ← La aplicación
├── data/
│   ├── campanas.json   ← Textos legales (actualizable)
│   └── plazos.json     ← Plazos de financiación (actualizable)
├── README.md
└── .gitignore
```

---

## 🛠️ Desarrollo

Este proyecto es un archivo HTML único con:
- **CSS** embebido (estilos IKEA)
- **JavaScript** vanilla (sin frameworks)
- **Librerías CDN:**
  - [SheetJS](https://sheetjs.com/) - Lectura de Excel
  - [Mammoth.js](https://github.com/mwilliamson/mammoth.js) - Lectura de Word

---

## 📄 Licencia

Uso interno IKEA Family & Ventajon.

---

Desarrollado con ❤️ y Claude AI
