# neonatal-gut-microbiome-analysis
Analysis of gut microbiome composition in preterm infants, focusing on taxonomic profiles and longitudinal dynamics across early life.

# Neonatal Gut Microbiome Analysis

Análisis del microbioma intestinal neonatal utilizando enfoques taxonómicos, funcionales y composicionales.

Repositorio:  
https://github.com/shadayguerrero/neonatal-gut-microbiome-analysis

---

# 📚 Contenido

1. Introducción  
2. Procesamiento de datos  
3. Diversidad alfa  
4. Diversidad beta  
5. Abundancia taxonómica  
6. Dinámica longitudinal  
7. Análisis composicional (CLR)  
8. Diversidad funcional  
9. Conclusiones  

---

# 1. 🧬 Introducción

Este proyecto analiza la composición y dinámica del microbioma intestinal neonatal a partir de datos metagenómicos.

Se aplican diferentes enfoques:

- Diversidad alfa (intra-muestra)
- Diversidad beta (inter-muestras)
- Análisis de abundancia
- Dinámica longitudinal
- Transformaciones composicionales (CLR)
- Análisis funcional

---

# 2. ⚙️ Procesamiento de datos

Se utilizaron tres fuentes principales:

- Tabla de abundancia taxonómica
- Metadatos clínicos
- Datos funcionales

Los datos fueron:

- Filtrados
- Normalizados a abundancias relativas
- Integrados con metadatos

---

# 3. 📊 Diversidad Alfa

Se calcularon métricas como:

- Shannon
- Simpson
- Richness

Estas métricas permiten evaluar la diversidad dentro de cada muestra.

### Resultados

Ejemplo de distribución de diversidad:

![Alpha Diversity](plots/alpha_diversity_boxplot.png)

---

# 4. 🌐 Diversidad Beta

Se evaluaron diferencias entre muestras usando:

- Bray-Curtis
- (y opcionalmente CLR + distancia euclidiana)

Se aplicaron métodos de reducción de dimensionalidad:

- PCoA
- PCA

### Resultados

PCoA Bray-Curtis:

![PCoA](plots/pcoa_braycurtis.png)

---

# 5. 🧫 Abundancia Taxonómica

Se analizaron los taxones más abundantes a diferentes niveles:

- Phylum
- Family
- Genus

### Resultados

Abundancia relativa:

![Abundance](plots/stacked_bar_top_taxa.png)

---

# 6. ⏳ Dinámica Longitudinal

Se evaluó la evolución del microbioma a lo largo del tiempo.

Se generaron visualizaciones tipo:

- Stacked area plots
- Heatmaps longitudinales

### Resultados

Dinámica temporal:

![Streamplot](plots/streamplot_taxa_over_time.png)

Heatmap de abundancia:

![Heatmap](plots/heatmap_taxa_over_time.png)

---

# 7. 🔬 Análisis Composicional (CLR)

Dado que los datos microbiológicos son composicionales, se aplicó:

- CLR (Centered Log-Ratio transformation)

Esto permite análisis estadísticos más robustos.

Se realizaron:

- PCA sobre datos CLR
- Distancias euclidianas (beta diversidad)
- Clustering

### Resultados

PCA con CLR:

![PCA CLR](plots/pca_clr.png)

Clustering:

![Clustering](plots/clustering_clr.png)

---

# 8. 🧪 Diversidad Funcional

Se analizaron perfiles funcionales derivados de los datos metagenómicos.

Incluye:

- Diversidad alfa funcional
- Diversidad beta funcional
- Abundancia de funciones

### Resultados

Diversidad funcional:

![Functional Alpha](plots/functional_alpha.png)

PCoA funcional:

![Functional Beta](plots/functional_beta.png)

---

# 9. 📌 Conclusiones

- El microbioma neonatal muestra cambios dinámicos a lo largo del tiempo.
- Existen diferencias entre grupos en términos de diversidad y composición.
- El análisis composicional (CLR) mejora la interpretación estadística.
- Los perfiles funcionales complementan la información taxonómica.

---

# 🛠️ Notebooks

Los análisis están organizados en notebooks:

- Alpha diversidad
- Beta diversidad
- Abundancias
- Dinámica longitudinal
- CLR / composicional
- Funcional

---

# 📁 Estructura del repositorio
