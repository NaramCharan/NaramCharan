<div align="center">

<!-- HUD header — cyan/gold on the site's OLED black-navy, not the red suit palette -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:05080F,60:0e7d8f,100:22D3EE&height=170&section=header&text=NARAM%20CHARAN&fontSize=48&fontColor=eaf7fb&fontAlignY=36&desc=AI%20%26%20MACHINE%20LEARNING%20ENGINEER&descSize=14&descAlignY=56" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=20&pause=1400&color=22D3EE&center=true&vCenter=true&width=760&lines=%3E+I+teach+machines+to+predict+things.;%3E+End-to-end+ML+%E2%80%94+not+notebook+exercises.;%3E+Shipped+to+a+URL%2C+not+just+a+leaderboard." alt="I teach machines to predict things."/>

<br/><br/>

**`B.TECH CSE · AI & ML`**&nbsp;&nbsp;·&nbsp;&nbsp;**`GD GOENKA UNIVERSITY`**&nbsp;&nbsp;·&nbsp;&nbsp;**`YEAR 03`**&nbsp;&nbsp;·&nbsp;&nbsp;**`CGPA 8.98 / 10`**

<br/>

<a href="https://naramcharan.me"><img src="https://img.shields.io/badge/PORTFOLIO-22D3EE?style=for-the-badge&logo=googlechrome&logoColor=22D3EE&labelColor=05080F"/></a>
<a href="https://rsna-app.salmonmeadow-7644e67e.eastasia.azurecontainerapps.io"><img src="https://img.shields.io/badge/LIVE_APP-FFB23E?style=for-the-badge&logo=microsoftazure&logoColor=FFB23E&labelColor=05080F"/></a>
<a href="https://www.linkedin.com/in/naramcharan/"><img src="https://img.shields.io/badge/LINKEDIN-22D3EE?style=for-the-badge&logo=linkedin&logoColor=22D3EE&labelColor=05080F"/></a>
<a href="mailto:charannaram1710@gmail.com"><img src="https://img.shields.io/badge/EMAIL-FFB23E?style=for-the-badge&logo=gmail&logoColor=FFB23E&labelColor=05080F"/></a>

<br/>

`◢ OPEN TO INTERNSHIPS`&nbsp;&nbsp;·&nbsp;&nbsp;`GURUGRAM, INDIA`

</div>

---

## `00` ◢ CORE

Third-year CS student specializing in **AI & Machine Learning**, building systems that reach
production rather than stopping at a metric in a notebook. Recommendation architectures on learned
embeddings, gradient-boosted forecasters across thousands of parallel series, CNNs on medical
imaging — and the serving layer around them.

Two things I care about more than model choice:

- **Leakage-free validation.** Split before you engineer features, split on the entity and not the
  row, and touch the test set once. Every number below comes from a split built that way.
- **Metrics that describe behaviour.** Accuracy on imbalanced data is the number most likely to lie
  to you. Where it would mislead, the honest metric is the one reported.

---

## `01` ◢ SERVICE RECORD

> `◈` **MK-05** is deployed and answering requests. `◈` **MK-04** is the featured build.
> Every metric is from a held-out split, never from training.

| | PROJECT | HEADLINE | STACK | |
|:--|:--|:--|:--|:--|
| **`MK-05`** | **[RSNA Pneumonia Detection](https://github.com/NaramCharan/RSNA-Pneumonia-Detection)**<br/><sub>Medical Imaging · **deployed** · Aug 1 – Sep 4, 2026</sub> | **83% recall**<br/><sub>0.79 F1 · 86% acc</sub> | `PyTorch` `pydicom` `FastAPI` `React` `Docker` `Azure` | [**LIVE ↗**](https://rsna-app.salmonmeadow-7644e67e.eastasia.azurecontainerapps.io) |
| **`MK-04`** | **[Walmart Weekly Sales Forecasting](https://github.com/NaramCharan/Walmart-Store-Weekly-Sales-Forecasting)**<br/><sub>Time-Series Forecasting</sub> | **95.55% R²**<br/><sub>validation</sub> | `LightGBM` `XGBoost` `Scikit-Learn` `Pandas` | |
| **`MK-03`** | **[E-Commerce Churn Prediction](https://github.com/NaramCharan/ecommerce-customer-churn-prediction)**<br/><sub>Classification</sub> | **98.28% acc**<br/><sub>94.74% F1</sub> | `XGBoost` `PyTorch` `Scikit-Learn` `Optuna` | |
| **`MK-02`** | **[Neural Collaborative Filtering](https://github.com/NaramCharan/Collaborative_Filtering_Recommendation_system)**<br/><sub>Recommender Systems</sub> | **&lt;10ms**<br/><sub>retrieval</sub> | `PyTorch` `FAISS` | |
| **`MK-01`** | **[Book Scraping & DB Pipeline](https://github.com/NaramCharan/Book-webscrapper)**<br/><sub>Data Engineering</sub> | **980+**<br/><sub>in &lt;30 min</sub> | `BeautifulSoup` `SQLAlchemy` `SQLite` `Pandas` | |

---

## `02` ◢ MK-05 · THE ONE THAT SHIPPED

Pneumonia screening on chest radiographs — trained, benchmarked, and running on a public URL.

```
DICOM  →  patient-level split  →  transfer learning  →  FastAPI  →  Docker  →  Azure
```

| | |
|:--|:--|
| **Result** | 83% pneumonia recall · 0.75 precision · 0.79 F1 · 86% accuracy on 1,836 held-out studies |
| **Baseline** | 68% — what you score by always answering "no pneumonia" |
| **Why recall** | ~70% of studies are negative. Accuracy rewards a model that finds nothing |
| **Models** | DenseNet-121 vs EfficientNet-B2 vs ResNet-34, two-stage transfer learning, one protocol |
| **Integrity** | Split on unique patient IDs, not rows. Test set evaluated exactly once |
| **Cost** | $5.06/month — priced a Postgres layer at $25.68 to hold a 4 KB CSV, and deleted it |

**The bug worth the whole project.** A copied ImageNet pipeline ran `RandomCrop(224)` *first*, on
1024×1024 radiographs. Every training image was a random **4.8% patch** still carrying the label
"pneumonia" — most contained no lung opacity at all, many contained no lung. Deleting that one line
beat every architecture change in the project combined.

> Augmentation is not free. A transform that is standard in one domain can silently corrupt your
> labels in another.

---

## `03` ◢ SUIT SYSTEMS

<table>
<tr>
<td valign="top" width="50%">

**`◢ NEURAL` — Deep Learning & GenAI**

`PyTorch` · `Transfer Learning` · `CNNs`
`Neural Collaborative Filtering`
`Vector Embeddings` · `FAISS`
`Prompt Engineering`

</td>
<td valign="top" width="50%">

**`◢ MODELS` — Machine Learning**

`XGBoost` · `LightGBM`
`Random Forest` · `Logistic Regression`
`Scikit-Learn` · `Optuna`

</td>
</tr>
<tr>
<td valign="top" width="50%">

**`◢ SIGNALS` — Data Intelligence**

`Pandas` · `NumPy`
`Feature Engineering` · `KNNImputer`
`Imbalance Handling` · `RobustScaler`

</td>
<td valign="top" width="50%">

**`◢ CORE` — Engineering & Deploy**

`Python 3 · Advanced OOP` · `Data Structures`
`FastAPI · REST APIs`
`SQL · Schema Design` · `SQLAlchemy`
`Docker · Azure` · `Git`

</td>
</tr>
</table>

<div align="center">

![Python](https://img.shields.io/badge/PYTHON-05080F?style=for-the-badge&logo=python&logoColor=22D3EE)
![PyTorch](https://img.shields.io/badge/PYTORCH-05080F?style=for-the-badge&logo=pytorch&logoColor=FFB23E)
![scikit-learn](https://img.shields.io/badge/SCIKIT--LEARN-05080F?style=for-the-badge&logo=scikit-learn&logoColor=22D3EE)
![Pandas](https://img.shields.io/badge/PANDAS-05080F?style=for-the-badge&logo=pandas&logoColor=FFB23E)
![FastAPI](https://img.shields.io/badge/FASTAPI-05080F?style=for-the-badge&logo=fastapi&logoColor=22D3EE)
![Docker](https://img.shields.io/badge/DOCKER-05080F?style=for-the-badge&logo=docker&logoColor=22D3EE)
![Azure](https://img.shields.io/badge/AZURE-05080F?style=for-the-badge&logo=microsoftazure&logoColor=FFB23E)
![SQL](https://img.shields.io/badge/SQL-05080F?style=for-the-badge&logo=postgresql&logoColor=22D3EE)

</div>

---

## `04` ◢ CERTIFICATIONS

| | | |
|:--|:--|:--|
| `JUL 2026` | **Deep Learning Specialization** | DeepLearning.AI |
| `JUL 2026` | **Claude Code: A Highly Agentic Coding Assistant** | DeepLearning.AI · Anthropic |
| `MAY 2026` | **Machine Learning Specialization** | DeepLearning.AI · Stanford University |
| `NOV 2025` | **Databases & SQL for Data Science with Python** | IBM · Coursera |
| `MAR 2025` | **Python for Everybody Specialization** | University of Michigan · Coursera |
| `MAR 2025` | **Prompt Engineering & Generative AI** | Google · Vanderbilt University |

---

## `05` ◢ TELEMETRY

<div align="center">

<!-- github-readme-stats.vercel.app is deliberately not used here: its public
     instance answers 503 most of the time, and a broken image on a profile
     front page is worse than no image. shields.io and streak-stats are live. -->

<img src="https://img.shields.io/github/followers/NaramCharan?style=for-the-badge&logo=github&label=FOLLOWERS&color=22D3EE&labelColor=05080F"/>
<img src="https://img.shields.io/github/stars/NaramCharan?affiliations=OWNER&style=for-the-badge&logo=github&label=STARS&color=FFB23E&labelColor=05080F"/>

<br/><br/>

<img src="https://streak-stats.demolab.com?user=NaramCharan&hide_border=true&background=05080F&stroke=132a33&ring=22D3EE&fire=FFB23E&currStreakLabel=22D3EE&sideLabels=a8c6d2&dates=5a6472"/>

</div>

---

<div align="center">

### `◢ ESTABLISH LINK`

Channels are open — internships, collaborations, or to talk shop about ML.

<a href="mailto:charannaram1710@gmail.com"><img src="https://img.shields.io/badge/EMAIL-05080F?style=for-the-badge&logo=gmail&logoColor=FFB23E"/></a>
<a href="https://www.linkedin.com/in/naramcharan/"><img src="https://img.shields.io/badge/LINKEDIN-05080F?style=for-the-badge&logo=linkedin&logoColor=22D3EE"/></a>
<a href="https://naramcharan.me"><img src="https://img.shields.io/badge/NARAMCHARAN.ME-05080F?style=for-the-badge&logo=googlechrome&logoColor=22D3EE"/></a>
<a href="https://wa.me/919966214989"><img src="https://img.shields.io/badge/WHATSAPP-05080F?style=for-the-badge&logo=whatsapp&logoColor=FFB23E"/></a>

<br/><br/>

<sub>`MARK XLII · PERSONAL INTERFACE` — the full HUD version lives at **[naramcharan.me](https://naramcharan.me)**</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:22D3EE,50:0e7d8f,100:05080F&height=110&section=footer" width="100%"/>

</div>
