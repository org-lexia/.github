# LexIA — Sistema RAG Jurídico (Cuba)

**LexIA** es una plataforma inteligente basada en la arquitectura **RAG (Generación Aumentada por Recuperación)**, diseñada específicamente para automatizar la consultoría jurídica, el análisis normativo y la redacción de documentos legales dentro del contexto legal de la República de Cuba.

El sistema está optimizado para asistir tanto a **Bufetes Colectivos** y asesores del sector estatal como a **MIPYMES, cooperativas y nuevos actores económicos** en la toma de decisiones y el cumplimiento normativo.

---

## 🚀 Características Principales

* **Consulta Confiable sin Alucinaciones:** Respuestas basadas estrictamente en la base de conocimiento cargada, impidiendo que la IA invente leyes o decretos.
* **Base de Conocimiento Actualizada:** Indexación estructurada de la *Gaceta Oficial de la República de Cuba*, Códigos (Civil, Penal, de Procesos), Decretos-Leyes de MIPYMES y resoluciones ministeriales.
* **Redacción Automatizada:** Generación ágil de borradores de contratos económicos, dictámenes jurídicos, actas de socios y procedimientos laborales listos para su revisión.
* **Buscador Semántico Avanzado:** Recuperación de artículos y jurisprudencia del Tribunal Supremo por contexto e intención, superando las búsquedas tradicionales por palabras clave.

---

## 🛠️ Arquitectura Técnica Pensada

El sistema se compone de tres capas fundamentales diseñadas para adaptarse al entorno de conectividad local:

1. **Ingesta de Datos:** Script en Python para la descarga y extracción de texto de la Gaceta Oficial, aplicando OCR (`Tesseract`/`EasyOCR`) en documentos escaneados antiguos.
2. **Procesamiento y Vectorización:** Segmentación inteligente de leyes por capítulos/artículos (`Chunking`) y almacenamiento en una base de datos vectorial local (`ChromaDB` / `Pinecone`).
3. **Orquestación y LLM:** Uso de frameworks como `LangChain` o `LlamaIndex` integrados con modelos de lenguaje. Viable para despliegue en la nube o de forma local (**On-Premise**) mediante modelos pequeños eficientes (`SLMs` como *Llama 3* o *Phi-3*) para trabajar sin dependencia crítica de internet.

---

## 💼 Enfoque de Monetización (Modelos de Negocio)

* **SaaS (Software como Servicio):** Suscripciones mensuales/anuales para MIPYMES y abogados independientes con acceso a la plataforma web.
* **On-Premise (Llave en mano):** Instalación del sistema directamente en los servidores locales de grandes empresas estatales u organismos provinciales con contratos de mantenimiento y actualización.
* **API de Integración:** Conexión del "cerebro legal" con sistemas ERP de gestión empresarial ya existentes en el país (como el *Versat Sarasola*).

---

## 🔒 Estado Legal y Propiedad Intelectual

Este repositorio es estrictamente **PRIVADO**. El código fuente, los prompts de control optimizados y la arquitectura del sistema constituyen propiedad intelectual comercial de los desarrolladores. 

Para revisar el marco regulatorio del proyecto, consulte los archivos en la raíz:
* `LICENCIA.txt`: Términos de propiedad y prohibición de copia para despliegues locales.
* `TERMINOS_DE_SERVICIO.md`: Cláusulas de uso web y exención de responsabilidad jurídica para el modelo SaaS.
