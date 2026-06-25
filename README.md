# Unidad-17Desarrollo-de-notebook-integrador-
Unidad 17 · Desarrollo de notebook integrador  
# 🏛️ Enterprise NLP End-to-End Pipeline: Multi-Aspect Routing, Business KPIs & GDPR Compliance

Este repositorio contiene el **Proyecto Integrador Final** de la materia, consolidando un pipeline de Procesamiento de Lenguaje Natural (NLP) industrial diseñado para la auditoría y monitoreo síncrono de la experiencia de usuario en una plataforma global de comercio electrónico (*E-commerce*).

El desarrollo implementa un flujo *End-to-End* transparente y reproducible que soluciona los problemas de significancia estadística (corpus balanceado de **40 interacciones libres**), sesgo multilingüe y cumplimiento normativo legal internacional de privacidad.

---

## 🛠️ Arquitectura y Modularización del Pipeline

El software está estructurado de manera desacoplada en celdas y funciones reutilizables con tipado estricto:

1. **Filtro de Privacidad Corporativa (GDPR Compliance):** Módulo de preprocesamiento determinista mediante expresiones regulares encargada de enmascarar Datos de Identificación Personal (PII) como correos electrónicos corporativos e identificadores financieros antes del análisis lingüístico.
2. **Preprocesamiento Avanzado con spaCy:** Tokenización, lematización profunda y remoción selectiva de stopwords segmentada dinámicamente según el idioma nativo de origen (*en_core_web_sm* / *es_core_news_sm*).
3. **Core Técnico Dual (Baseline vs. Deep Learning):** Implementación comparativa entre modelos estadísticos clásicos (**TF-IDF + Regresión Logística con pesos balanceados**) frente a la inferencia contextual fina de un **Transformer**.
4. **Enrutamiento por Aspecto y Detección de Emociones:** Mapeo paralelo que clasifica el área afectada (*Calidad, Logística, Soporte, Finanzas*) y extrae el estado psicológico reactivo del cliente (*Ira, Frustración, Alegría, Gratitud*).

---

## 📈 Cuadro de Mando de KPIs (Resultados Auditados del Sistema)

Para garantizar la **integridad absoluta de los resultados**, las métricas presentadas a continuación coinciden de forma exacta y determinista con el bloque matemático calculado por el cuaderno de código:

* **Macro F1-Score Global del Sistema:** **0.75**
* **Macro F1-Score en Idioma Inglés (High-Resource):** **0.93**
* **Macro F1-Score en Idioma Español (Mid-Resource):** **0.58**
* **KPI: Tasa de Detección de Fricción Crítica (CFDR):** **79.17%** (Porcentaje de usuarios detractores capturados automáticamente para contención prioritaria. Objetivo comercial: >90% | Frecuencia: Diaria).
* **KPI: Tasa de Falsas Alarmas por Sarcasmo (FOAR):** **7.50%** (Costo operativo derivado de errores de clasificación ante ironías lingüísticas. Objetivo comercial: <10% | Frecuencia: Semanal).

---

## 🌍 Diagnóstico de Brecha Multilingüe y Mitigación

El dashboard expone un **Gap de 35 puntos de rendimiento** en perjuicio del idioma español (0.93 vs. 0.58). Para mitigar el sesgo de datos de origen en los modelos comerciales, se proponen dos soluciones técnicas concretas para los siguientes sprints de ingeniería:
* **Fine-Tuning Local:** Ajuste fino sobre la arquitectura profunda de `XLM-RoBERTa-Large` utilizando un corpus balanceado de modismos comerciales hispanohablantes.
* **Data Augmentation:** Implementación de técnicas de *Back-Translation* para duplicar la significancia estadística de las clases minoritarias en español, penalizando las clases dominantes mediante funciones de pérdida ponderadas.

---

## ⚙️ Instrucciones de Despliegue e Ingesta Local

Garantice la consistencia del ecosistema analítico instalando las dependencias puras congeladas en el archivo de control corporativo libre de comentarios markdown:

```bash
# 1. Clonar el repositorio institucional
git clone [https://github.com/TU_USUARIO/TU_REPOSITORIO.git](https://github.com/TU_USUARIO/TU_REPOSITORIO.git)

# 2. Instalar dependencias puras congeladas
pip install -r requirements.txt

# 3. Descargar modelos lingüísticos base de spaCy
python -m spacy download en_core_web_sm
python -m spacy download es_core_news_sm
