# 🛡️ ANMI: Asistente Nutricional Materno Infantil

**ANMI** es un chatbot educativo basado en Inteligencia Artificial diseñado para apoyar a padres y cuidadores en la lucha contra la anemia infantil en el Perú. Utiliza modelos de lenguaje avanzados (Llama 3.1 a través de Groq) para brindar recomendaciones personalizadas sobre alimentación y suplementación según la edad del bebé.

## 📋 Características Principales

* IA Especializada: Responde dudas basándose estrictamente en guías oficiales del MINSA (Ministerio de Salud) y tablas nutricionales validadas.
* Asesoría por Edad: Detecta la edad del bebé (en meses) para adaptar las recomendaciones:
    * **0-6 meses:** Promoción exclusiva de la lactancia materna.
    * **6-36 meses:** Alimentación complementaria, texturas, cantidades y suplementación con hierro.
*  Recetario Rico en Hierro: Sugiere recetas prácticas con sangrecita, bazo, hígado y quinua.
*  Detección de Emergencias: Identifica palabras clave de riesgo (convulsiones, desmayos, etc.) y bloquea el chat para derivar inmediatamente a un centro de salud.
*  Privacidad: Sistema de consentimiento informado y manejo anónimo de datos.

## 🛠️ Tecnologías Utilizadas

* **Lenguaje:** Python 3.11+
* **Frontend:** [Streamlit](https://streamlit.io/)
* **IA / LLM:** [Groq API](https://groq.com/) (Modelo: `llama-3.1-8b-instant`)
* **Control de Versiones:** Git & GitHub



##  Instalación
```
pip install -r "ChatBot ANMI/requirements.txt"
```



## 📂 Estructura del Proyecto

```text
ChatBot-ANMI-/
├── .streamlit/                # 🔐 Archivo con la API KEY privada(propoio de cada usuario)
│   └── secrets.toml
├── ChatBot ANMI/
│   ├── ChatBot.py             # 🏠 Archivo principal de la aplicación
│   ├── datos_anmi.py          # 📚 Base de conocimiento estructurada
│   ├── requirements.txt       # 📦 Dependencias del proyecto
│   └── pages/
│       └── terminos_condiciones.py  # 📄 Página de Términos y Condiciones
└── README.md                  # 📖 Documentación


