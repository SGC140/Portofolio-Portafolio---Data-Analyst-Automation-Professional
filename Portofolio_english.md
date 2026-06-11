<div align="justify">

# Sebastián González Castillo
### Principal Data Analyst | Automation Architect | Solution Designer

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/sebastián-gonzález-castillo-4ab49133b)
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![RStudio](https://img.shields.io/badge/RStudio-75AADB?style=for-the-badge&logo=RStudio&logoColor=white)](https://posit.co/)
[![SQL](https://img.shields.io/badge/SQL-ANSI-F29111?style=for-the-badge&logo=database)](https://en.wikipedia.org/wiki/SQL)
[![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)](https://cloud.google.com/)
[![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=for-the-badge&logo=google-cloud&logoColor=white)](https://cloud.google.com/bigquery)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Plotly](https://img.shields.io/badge/Plotly-239120?style=for-the-badge&logo=plotly&logoColor=white)](https://plotly.com/)
[![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Gradio](https://img.shields.io/badge/Gradio-FF7C00?style=for-the-badge&logo=gradio&logoColor=white)](https://gradio.app/)
[![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![Looker Studio](https://img.shields.io/badge/Looker_Studio-4285F4?style=for-the-badge&logo=looker&logoColor=white)](https://lookerstudio.google.com/)
[![Google Workspace](https://img.shields.io/badge/Google_Workspace-DB4437?style=for-the-badge&logo=google-workspace&logoColor=white)](https://workspace.google.com/)
[![Google Sheets](https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=google-sheets&logoColor=white)](https://google.com/sheets)
[![n8n](https://img.shields.io/badge/n8n-FF6D5A?style=for-the-badge&logo=n8n&logoColor=white)](https://n8n.io/)
[![GenAI](https://img.shields.io/badge/GenAI-Gemini%20%7C%20Llama%20%7C%20DeepSeek-8A2BE2?style=for-the-badge&logo=openai&logoColor=white)](#)
[![Hugging Face](https://img.shields.io/badge/Hugging_Face_Spaces-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)](https://huggingface.co/)
[![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)](https://git-scm.com/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)
[![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)](https://colab.research.google.com/)
[![ETL/ELT](https://img.shields.io/badge/ETL%20%2F%20ELT-Pipelines-5C5C5C?style=for-the-badge)](https://en.wikipedia.org/wiki/Extract,_transform,_load)

---

## 🏛️ Executive Vision & Analytical Capabilities

My professional profile transcends traditional technical execution to position me as a Solution Architect who understands the organizational ecosystem in its entirety. With an interdisciplinary educational background anchored in **Political Science and Public Policy Evaluation**, I possess the unique ability to translate complex institutional and business problems into high-performance data architectures. I do not just write code for the sake of it; I design structured information flows, govern data models, and deploy operational intelligence systems that resolve information asymmetries and leverage empirical, quantitative evidence-based decision-making.

Technologically, I operate across the entire data lifecycle. I orchestrate multi-source ingestion by combining dynamic Web Scraping techniques (Selenium), API consumption, and hidden DOM telemetry extraction. I structure and clean massive data volumes using Pandas, NumPy, and advanced SQL, channeling them through ETL/ELT pipelines into centralized Cloud Data Warehouses (BigQuery). Finally, I materialize analytical value by integrating Generative AI models (Google Gemini, Llama, DeepSeek) and designing high-impact interactive visualizations in tools like Streamlit, Gradio, Power BI, and Looker Studio. My approach ensures that every delivered solution provides process standardization, human error mitigation, and an overwhelming operational Return on Investment (ROI).

---

## 🚀 Project Ecosystem & Results

### [1. Automated Class Auditing (Video & Multimodal Artificial Intelligence)](https://github.com/SGC140/Auditor-a-Clases)
![Gemini API](https://img.shields.io/badge/Gemini_API-AI-orange?style=flat-square) ![FFmpeg](https://img.shields.io/badge/FFmpeg-Video-lightgrey?style=flat-square) ![MoviePy](https://img.shields.io/badge/MoviePy-Processing-purple?style=flat-square) ![Google Drive](https://img.shields.io/badge/Google_Drive-Integration-green?style=flat-square) ![Pandas](https://img.shields.io/badge/Pandas-Data-150458?style=flat-square)

This project revolutionized quality control in higher education environments by directly connecting the project area with the academic core, replacing exhausting manual reviews with a comprehensive algorithmic and multimodal auditing system. The solution securely downloads recordings from Google Drive, processes them through heuristic compression and acceleration to optimize costs, and delegates the pedagogical and technical analysis to Google Gemini's AI, successfully extracting objective evaluations regarding teaching performance, student engagement, and subject mastery. The business impact was transformative: the system generated the capacity to optimize video auditing time by 96.67%, producing standardized reports in high-quality JSON, CSV, and PDF formats that democratize institutional feedback.

Architecturally, the system is a prime example of resilience and advanced resource management. It implements a robust iterative fallback mechanism between MoviePy and native FFmpeg via subprocesses, guaranteeing the processing of heavy files and mitigating server memory bottlenecks. Furthermore, to bypass the AI's strict context token limits, the code orchestrates dynamic video content segmentation, integrating an accumulated memory mechanism (inspired by RAG architecture) that injects the findings of previous fragments as context for the subsequent ones, thus ensuring a structurally coherent report from start to finish.

```python
# Robust video segmentation and compression via subprocesses
subprocess.run(['ffmpeg', '-i', video_path, '-filter_complex', '[0:v]setpts=0.666667*PTS...', '-segment_time', '1500', output])

# Accumulated memory logic for auditing segments with Gemini
contexto_acumulado = ""
for i, segmento in enumerate(segmentos_video):
    prompt_dinamico = f"You are an expert auditor. Previous context: {contexto_acumulado}. Analyze this new section."
    respuesta = client.models.generate_content([prompt_dinamico, segmento])
    contexto_acumulado = respuesta.text
```

<br>

### [2. Automated Repository Documentation (Advanced LLMs)](https://github.com/SGC140/Automatizacion-Documentacion-de-Repositorios-y-Proyectos)
![Groq](https://img.shields.io/badge/Groq_API-Llama_3-green?style=flat-square) ![GitHub API](https://img.shields.io/badge/GitHub_API-Automation-black?style=flat-square) ![DeepSeek](https://img.shields.io/badge/DeepSeek-AI-blue?style=flat-square) ![Python](https://img.shields.io/badge/Python-Scripting-3776AB?style=flat-square)

Technical debt management and documentation in agile methodologies represent a persistent challenge that often devours critical engineering team resources. This autonomous orchestrator eradicates that bottleneck by interacting directly with the GitHub API to iterate over repositories, recursively extract the business logic from source files (`.py`, `.sql`, `.ipynb`, `.json`), and generate comprehensive technical manuals, architectures, and dependencies utilizing the combined analytical power of models like Llama-3, DeepSeek, and Gemini. What previously required complex projects to be documented over multiple days of laborious manual writing now allows for contextualizing and documenting the entire data flow bilingually (Spanish and English) in a mere 10 minutes per iteration.

Technically, the script functions as an autonomous agent that controls its own state through a historical log (TXT file) to identify previously processed repositories, preventing redundant reprocessing and surgically optimizing API request quotas. Intricate fallback engines and exception controls were implemented using time delays (`time.sleep`) that evade network saturation interruptions, ensuring the atomic delivery of the final documentation through direct programmatic commits into GitHub's production branches.

```python
# Recursive search to extract source code from key files
acumulated_script = ""
elementos = repo.get_contents("")
while elementos:
    archivo = elementos.pop(0)
    if archivo.type == "dir":
        elementos.extend(repo.get_contents(archivo.path))
    elif archivo.name.endswith(('.py', '.sql', '.ipynb', '.json')):
        acumulated_script += f"\n\n### {archivo.path} ###\n{archivo.decoded_content.decode('utf-8')}"

# Automated commit of the generated bilingual README to production
repo.update_file(readme_path, commit_msg, english_readme, file_sha)
```

<br>

### [3. Territory Backend: Geospatial Analysis & Algorithmic Assignment](https://github.com/SGC140/Backend-Territorio)
![Geopy](https://img.shields.io/badge/Geopy-ArcGIS-lightgrey?style=flat-square) ![Hugging Spaces](https://img.shields.io/badge/Hugging_Spaces-Deployment-yellow?style=flat-square) ![Gradio](https://img.shields.io/badge/Gradio-UI-red?style=flat-square) ![Selenium](https://img.shields.io/badge/Selenium-Scraping-green?style=flat-square) ![Folium](https://img.shields.io/badge/Folium-Maps-purple?style=flat-square)

This project radically transformed territorial operational logistics through scientific calculation and spatial intelligence. The system agilely and automatically extracts critical address and contact information of various district social support entities (Youth Houses, Care Blocks, etc.) using dynamic scrapers built with Selenium. Subsequently, it unifies this data into a mathematical model that calculates complex geodesic distances to match and assign operational collaborators based on strict geographic proximity to the entities. The organic impact of this development allowed for the reactivation of networking campaigns that were showing declining figures; by mitigating travel inefficiencies and optimizing collaborator routes, the average daily success peaks in the campaigns rose steadily by 80%.

The solution's design is deployed on a modern architecture hosted on Hugging Face Spaces, which dynamizes the tool's consumption through interactive visual interfaces generated with Gradio and interactive cartographic maps rendered with Folium. All processing incorporates rate limiters (`RateLimiter`) for the ArcGIS geocoder, guaranteeing the precise extraction of latitude and longitude coordinates without compromising execution IPs to bans, denoting a profound understanding of designing secure, fault-tolerant systems in production environments.

```python
# Scientific calculation of geodesic distance considering Earth's curvature
df_combinado['Distancia_km'] = df_combinado.apply(
    lambda x: geodesic(x['Coordenadas_Entidad'], x['Coordenadas_Personal']).km, axis=1
)
# Optimal assignment guaranteeing the shortest route
asignacion_optima = df_combinado.sort_values(['Nombre_Entidad', 'Distancia_km']).groupby('Nombre_Entidad').head(1)
```

<br>

### [4. Enterprise Analytics Pipeline & Centralized Data Ingestion (BigQuery)](https://github.com/SGC140/BigQuery-Project---ETL-Data-Analysis-)
![BigQuery](https://img.shields.io/badge/BigQuery-Data_Warehouse-blue?style=flat-square) ![SQL](https://img.shields.io/badge/SQL_ANSI-Transformations-orange?style=flat-square) ![Looker Studio](https://img.shields.io/badge/Looker_Studio-BI-4285F4?style=flat-square) ![Power BI](https://img.shields.io/badge/Power_BI-BI-F2C811?style=flat-square)

This ambitious architecture resolved high fragmentation and operational data isolation by integrating databases from multiple independent social and educational impact projects (Ecolombia, Jóvenes a la E, Suba) into a centralized Data Warehouse within the Google Cloud Platform environment. At a business level, this effort unified analytical views, fueled executive dashboards in Power BI and Looker Studio, and dramatically optimized the time dedicated to strategizing rather than manually cleaning data. Its SQL traceability models enabled early tracking mechanisms, telemetry reconciliation, and employability profiling that were decisive in achieving a 97% academic retention rate and an 80% approval rate in the targeted projects.

The enterprise queries hosted in BigQuery were designed under the ELT (Extract, Load, Transform) paradigm, drastically minimizing Google Cloud processing costs through the use of analytical window functions (`QUALIFY ROW_NUMBER()`), advanced unnesting of dynamic and nested structures (`UNNEST` with `STRUCT`), and complex text string homogenization rules with Regular Expressions. This design masterfully unifies socioeconomic variables and generates preventive diagnostics regarding academic progress.

```sql
-- Sociodemographic normalization and analytical deduplication at low scan cost
SELECT
  DOCUMENTO,
  CASE 
    WHEN REGEXP_CONTAINS(LOWER(ESCOLARIDAD), 'universitario|pregrado') THEN 'Universitario Completo'
    ELSE ESCOLARIDAD 
  END AS NIVEL_EDUCATIVO
FROM `proyecto_gcp.dataset.raw_data`
QUALIFY ROW_NUMBER() OVER(PARTITION BY DOCUMENTO ORDER BY FECHA_ACTUALIZACION DESC) = 1
```
<br>

### [5. Data Ingestion and Management Pipeline (Periodization Control)](https://github.com/SGC140/Control_periodizacion_unificacion_DATA)
![Python](https://img.shields.io/badge/Python-Scripting-3776AB?style=flat-square) ![Google Sheets](https://img.shields.io/badge/Google_Sheets-API-34A853?style=flat-square) ![Pandas](https://img.shields.io/badge/Pandas-ETL-150458?style=flat-square)

Complementing the BigQuery architecture, this microservices ecosystem orchestrates massive extraction and automated loading of operational data from Google Sheets to the Google Cloud. Its main innovation is the implementation of a dynamic schema validation module (`validacion_dataframes.py`) that acts as a strict quality gatekeeper; the system algorithmically compares the clean DataFrame structure against the metadata of the destination table in BigQuery, preventing injections of corrupt data or incompatible schemas. This automation eliminates reliance on error-prone manual processes and guarantees institutional coherence.

The pipeline not only extracts and cleans, but also manages time: it includes specialized routines (`Append_DATA_BQ.py`) that generate historical snapshots of operational data on a monthly basis, adding periodization columns (`YYYY-MM`) through additive writes (`WRITE_APPEND`). The entire process is executed sequentially by a central orchestrator (`trigger.py`), which standardizes the simultaneous update of multiple projects, allowing the organization to diagnose bottlenecks and evaluate trends over time.

```python
# Aggressive header normalization fragment in the Ingestion Pipeline
DF.columns = (DF.columns
              .str.replace(" ","_")
              .str.normalize('NFKD')
              .str.encode('ascii', errors='ignore')
              .str.decode('utf-8')
              .str.lower()
              .str.replace(r"[\r\n]+", "", regex=True)
              .str.replace(r"[^a-z0-9_#]", "", regex=True))
```

<br>

### [6. Automated Job Market Intelligence Pipeline (Advanced Web Scraping)](https://github.com/SGC140/Vacantes-J-venes-a-la-E)
![Selenium](https://img.shields.io/badge/Selenium-Automation-green?style=flat-square) ![n8n](https://img.shields.io/badge/n8n-Orchestration-FF6D5A?style=flat-square) ![Google Colab](https://img.shields.io/badge/Google_Colab-Execution-F9AB00?style=flat-square)

Acquiring labor market intelligence is vital to connecting training programs with real corporate demand. This pipeline supplants manual inspection through a second-level scraper, executed in headless mode, which periodically audits high-traffic job portals such as elempleo.com. Instead of relying on fragile visual element selection techniques (XPath or CSS that constantly change), the tool intercepts and processes telemetry payloads injected hidden in the DOM (such as Google Analytics 4 JSON objects) to extract precise and comprehensive structured data on technical requirements, equivalent roles, and confidential salary bands. The automation vastly improves the suggestion logic of traditional employment agents, agilely filtering and synchronizing viable profiles periodically to trigger organized self-application.

The system integrates powerful dependencies like `dateparser` to normalize publication dates expressed in local natural language (e.g., "Published 2 days ago"), transforming them into standardized ISO formats that allow chronological ordering. The outputs are seamlessly integrated into storage ecosystems (CSV and Google Sheets API) to serve as immediate input for human resources analysts in their salary projections and market educational requirement diagnostics.

```python
# Hidden telemetry interception in the DOM (Structural bypass of visual interface)
json_telemetria = vacante.get_attribute("data-ga4-offerdata")
if json_telemetria:
    datos_estructurados = json.loads(json_telemetria)
    salario_real = datos_estructurados.get("salary", "Confidencial")
    
# Algorithmic normalization of natural language to Datetime ISO format
Fecha_publicacion = dateparser.parse(
    Fecha_publicacion_vacante.text.replace("Publicado", "")
).strftime('%Y-%m-%d')
```

<br>

### [7. Instagram Analytics Dashboard (Kairós Research Incubator)](https://github.com/SGC140/Kairos)
![Streamlit](https://img.shields.io/badge/Streamlit-UI-FF4B4B?style=flat-square) ![Plotly](https://img.shields.io/badge/Plotly-Visualizations-23F18F?style=flat-square) ![NumPy](https://img.shields.io/badge/NumPy-Math-013243?style=flat-square)

In the realm of digital marketing, intuition-based decision-making represents an unacceptable operational risk. This Business Intelligence tool consolidates raw telemetry exported from Meta Business Suite and transforms it into a high-performance interactive dashboard developed entirely in Python using Streamlit and Plotly. Its implementation proved critical for the "Kairós Research Incubator", allowing for the identification of bottlenecks in content administration and irrefutably clarifying conversion funnels, content longevity, and advertising incidences. 

Through the development of reusable code, scatter plots with Ordinary Least Squares (`trendline="ols"`) trend lines, and temporal correlation analysis, the information was disaggregated to diagnose patterns of possible shadowbans and predict absolute success peaks in publications ("Prime Time"). The system isolates exactly which variables and content formats correlate with high conversion rates in likes and comments, transforming vanity metrics into predictive intelligence.

```python
# Interactive scatter plot calculating trend lines (Least Squares)
fig1 = px.scatter(
    df, x="Alcance", y="Me gusta", size="Visualizaciones", color="Me gusta",
    color_continuous_scale="Plasma", hover_name="Desc_Hover", trendline="ols",
    template="plotly_dark"
)
```

<br>

### [8. Gamification Analytical Processing (Cerebritos)](https://github.com/SGC140/Cerebritos-Data-Analysis)
![Pandas](https://img.shields.io/badge/Pandas-Core-150458?style=flat-square) ![Python](https://img.shields.io/badge/Python-Scripting-3776AB?style=flat-square)

Measuring user participation in interactive platforms requires handling massive, structured data. This ETL pipeline in Python acts as a specialized aggregation and cleaning engine for immense transactional gamification logs generated in educational environments. The code utilizes Pandas' matrix manipulation capabilities to merge fragmented datasets, select key columns, and normalize internal, cryptic educational level identifiers into human-readable formats.

By standardizing raw data and eliminating categorical noise, the algorithm groups and calculates global engagement indicators (the "Amount of Cerebritos" obtained) by population segment, grade, and email. This allows the organization to accurately evaluate the return on investment of its gamified strategies, identify high-performing users, and diagnose participation gaps to optimize the design of future incentives.

```python
# Vertical merge of massive datasets and aggregation of transactional metrics
data_consolidada = pd.concat([pd.read_csv("Gamificación_1.csv"), pd.read_csv("Gamificación_2.csv")])
df_agrupado = data_consolidada.groupby(["Correo", "Grado"]).agg(
    Total_cerebritos=('Cantidad Cerebritos', 'sum')
).reset_index()
```

---

### 📬 Strategic Contact & Collaboration

Looking to optimize complex operations, build fault-tolerant data architectures, or design strategic information systems that empower decision-making? Don't look for a simple programmer; integrate a Solution Architect with comprehensive business vision.

Let's connect and transform your data into invaluable assets on **[LinkedIn](https://www.linkedin.com/in/sebastián-gonzález-castillo-4ab49133b)**.

</div>