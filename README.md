# SmartEdu - Backend

API y servicios de backend para la plataforma educativa gamificada SmartEdu.

## Tecnologías
- **Node.js & Express**: API REST principal
- **Supabase**: Base de datos PostgreSQL y autenticación
- **Python & FastAPI**: Microservicio de IA (`ai-service/`) para procesamiento de resúmenes, trivias y roadmaps adaptativos

## Estructura
```
SmartEdu-Backend/
├── ai-service/        # Servicio Python / FastAPI para IA
├── node_modules/      # Dependencias de Node.js
├── p.sql              # Scripts iniciales de base de datos
├── package.json       # Configuración y dependencias de la API
└── README.md
```

## Configuración y ejecución

### Backend (Node.js)
```bash
npm install
npm run dev
```

### AI Service (Python)
```bash
cd ai-service
python -m venv .venv
# Activar entorno virtual (Windows):
.venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```
