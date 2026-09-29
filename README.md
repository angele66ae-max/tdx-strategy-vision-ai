# TDX Strategy Vision AI

Asistente visual de solo lectura para **Tower Defense X (TDX)** en Roblox. Analiza la imagen de pantalla para leer datos del HUD —efectivo, oleada y vida— y presenta sugerencias tácticas. El jugador conserva el control de todas las acciones.

> Proyecto no oficial, sin afiliación con Roblox ni con Tower Defense X. No simula entradas ni automatiza el juego.

## Funciones

- Captura de pantalla local con `mss`.
- Procesamiento visual con OpenCV y lectura OCR con Tesseract/PyTesseract.
- Seguimiento de efectivo, oleada y vida, con recomendaciones basadas en el estado detectado.
- Arquitectura modular: `capture.py`, `analyzer.py` y `advisor.py`.

## Instalación rápida

Requiere Python 3.10 o posterior. Instala también el motor [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) en tu sistema operativo; `pytesseract` es el enlace de Python y no incluye el ejecutable.

```bash
git clone https://github.com/tu-usuario/tdx-strategy-vision-ai.git
cd tdx-strategy-vision-ai
python -m pip install -r requirements.txt
python main.py
```

Si Tesseract no está en el `PATH`, configura la ruta del ejecutable en el proyecto antes de iniciar el analizador. Mantén Roblox visible para que el programa pueda leer el HUD de la pantalla.

## Landing page

Consulta la [landing page del proyecto](outputs/index.html) para ver sus funciones, arquitectura y guía visual de instalación.

## Estructura prevista del proyecto

```text
.
├── outputs/
│   └── index.html       # Landing page
├── capture.py           # Captura de pantalla (módulo previsto)
├── analyzer.py          # OpenCV y OCR (módulo previsto)
├── advisor.py           # Recomendaciones estratégicas (módulo previsto)
├── main.py              # Bucle de análisis (módulo previsto)
└── requirements.txt     # Dependencias de Python
```

## Dependencias

Las librerías de Python están listadas en [`requirements.txt`](requirements.txt). Tesseract OCR se instala por separado como aplicación del sistema.

## Aviso

TDX Strategy Vision AI es una herramienta comunitaria no oficial. No está afiliada, respaldada ni aprobada por Roblox o los creadores de Tower Defense X. Las lecturas OCR y recomendaciones pueden ser inexactas; úsalas como referencia.

