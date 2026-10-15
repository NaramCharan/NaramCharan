<!-- Upload this README AND the assets/ folder to NaramCharan/NaramCharan. -->
<div align="center">

<a href="https://naramcharan.me"><img src="assets/hud-header.svg" width="100%" alt="Naram Charan. I teach machines to predict things. Computer vision, forecasting and NLP. Visit naramcharan.me." /></a>

<br />

<a href="https://naramcharan.me"><img src="assets/portfolio.svg" height="42" alt="Explore portfolio →" /></a>
<a href="https://rsna-app.salmonmeadow-7644e67e.eastasia.azurecontainerapps.io/"><img src="assets/demo.svg" height="42" alt="Try the live ML application →" /></a>
<a href="https://naramcharan.me/armor/"><img src="assets/aegis.svg" height="42" alt="Explore Project Aegis 3D →" /></a>

<p><b>3rd-year CS · AI &amp; Machine Learning · Open to internships</b><br />
<sub>GD Goenka University · Gurugram, India · CGPA 8.98 / 10 · Graduating May 2028</sub></p>

<a href="https://www.linkedin.com/in/naramcharan/">LinkedIn</a> · <a href="mailto:charannaram1710@gmail.com">Email</a> · <a href="https://wa.me/919966214989">WhatsApp</a>

</div>

## `01` ◢ SELECTED BUILDS

Medical images, time series, language models, and the systems around them. Open a build to see the code and evaluation.

<table>
<tr>
<td width="50%"><a href="https://github.com/NaramCharan/RSNA-Pneumonia-Detection"><img src="assets/rsna.svg" width="100%" alt="RSNA Pneumonia Detection — deployed. 83% pneumonia recall, 0.79 F1 on 1,836 held-out studies. Patient-level split. PyTorch, FastAPI, Docker, Azure." /></a></td>
<td width="50%"><a href="https://github.com/NaramCharan/Handbuilt-Transformer"><img src="assets/gpt.svg" width="100%" alt="Handbuilt Transformer — ongoing. 1.82 validation loss on a roughly 210K-parameter decoder-only GPT, plus a byte-level BPE tokenizer written from scratch in PyTorch." /></a></td>
</tr>
<tr>
<td width="50%"><a href="https://github.com/NaramCharan/Walmart-Store-Weekly-Sales-Forecasting"><img src="assets/forecast.svg" width="100%" alt="Walmart Sales Forecasting — validation R² 0.9555 across roughly 3,000 store–department series. Custom recursive walk-forward engine. LightGBM, XGBoost, Pandas." /></a></td>
<td width="50%"><a href="https://github.com/NaramCharan/ecommerce-customer-churn-prediction"><img src="assets/churn.svg" width="100%" alt="E-Commerce Churn — selected XGBoost model: 94.74% test F1 and 98.28% test accuracy. Optuna tuning and comparison with a PyTorch network." /></a></td>
</tr>
<tr>
<td colspan="2" align="center"><a href="https://github.com/NaramCharan/Book-webscrapper"><img src="assets/books.svg" width="50%" alt="Book Data Pipeline — over 980 books in under 30 minutes. Structured extraction to SQLite and CSV using BeautifulSoup and SQLAlchemy." /></a></td>
</tr>
</table>

**[Try the deployed X-ray application ↗](https://rsna-app.salmonmeadow-7644e67e.eastasia.azurecontainerapps.io/) · [Read the full project briefs ↗](https://naramcharan.me/#projects)**

## `02` ◢ ENGINEERING PRINCIPLES

- **Check the data reaching the model.** Removing `RandomCrop(224)` from 1024 × 1024 chest X-rays mattered more than switching CNNs.
- **Separate evaluation from tuning.** Patient-level splits for radiographs; chronological evaluation for forecasting. Label validation and test results clearly.
- **Build the serving path.** Matching preprocessing, an API, a usable interface, and a deployment belong in the same project.

## `03` ◢ SYSTEMS I WORK WITH

| System | Tools & methods |
| :-- | :-- |
| **NEURAL** | <img src="assets/icons/pytorch.svg" width="18" height="18" alt="" />&nbsp;PyTorch&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/tensorflow.svg" width="18" height="18" alt="" />&nbsp;TensorFlow&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/keras.svg" width="18" height="18" alt="" />&nbsp;Keras<br /><br /><img src="assets/icons/network.svg" width="18" height="18" alt="" />&nbsp;CNNs&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/network.svg" width="18" height="18" alt="" />&nbsp;transfer&nbsp;learning<br /><br /><img src="assets/icons/network.svg" width="18" height="18" alt="" />&nbsp;self-attention&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/network.svg" width="18" height="18" alt="" />&nbsp;BPE&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/network.svg" width="18" height="18" alt="" />&nbsp;embeddings |
| **MODELS** | <img src="assets/icons/tree.svg" width="18" height="18" alt="" />&nbsp;XGBoost&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/tree.svg" width="18" height="18" alt="" />&nbsp;LightGBM&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/tree.svg" width="18" height="18" alt="" />&nbsp;Random&nbsp;Forest<br /><br /><img src="assets/icons/scikitlearn.svg" width="18" height="18" alt="" />&nbsp;scikit-learn&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/tuning.svg" width="18" height="18" alt="" />&nbsp;Optuna |
| **SIGNALS** | <img src="assets/icons/pandas.svg" width="18" height="18" alt="" />&nbsp;Pandas&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/numpy.svg" width="18" height="18" alt="" />&nbsp;NumPy&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/medical.svg" width="18" height="18" alt="" />&nbsp;pydicom<br /><br /><img src="assets/icons/features.svg" width="18" height="18" alt="" />&nbsp;feature&nbsp;engineering&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/timeline.svg" width="18" height="18" alt="" />&nbsp;walk-forward&nbsp;evaluation |
| **CORE** | <img src="assets/icons/python.svg" width="18" height="18" alt="" />&nbsp;Python&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/fastapi.svg" width="18" height="18" alt="" />&nbsp;FastAPI&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/sqlalchemy.svg" width="18" height="18" alt="" />&nbsp;SQLAlchemy<br /><br /><img src="assets/icons/database.svg" width="18" height="18" alt="" />&nbsp;SQL&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/sqlite.svg" width="18" height="18" alt="" />&nbsp;SQLite&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/docker.svg" width="18" height="18" alt="" />&nbsp;Docker<br /><br /><img src="assets/icons/azure.svg" width="18" height="18" alt="" />&nbsp;Azure&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/git.svg" width="18" height="18" alt="" />&nbsp;Git&nbsp;&nbsp; · &nbsp;&nbsp;<img src="assets/icons/claude.svg" width="18" height="18" alt="" />&nbsp;Claude&nbsp;Code |

## `04` ◢ NEXT BUILD

I'm extending my **handbuilt GPT and BPE tokenizer** while studying transformer internals. My goal is to understand the model, evaluate it clearly, and make it usable.

<details>
<summary><b>◢ Origin story</b></summary>

It started with a man in a suit of armor. What stayed with me was the AI he talked to.

I'm a third-year Computer Science student specializing in AI & Machine Learning. I work on medical-image classifiers, forecasting pipelines, and models built from scratch.

My [portfolio](https://naramcharan.me) connects those projects through an interactive ML taxonomy and a WebGL armor assembly sequence. I built it with Next.js and WebGL by directing Claude Code.

</details>

<details>
<summary><b>◢ Learning record</b></summary>

- [Deep Learning Specialization](https://learn.deeplearning.ai/certificates/07716d58-daf9-4806-80a5-cfdac044a258?usp=sharing)
- [Machine Learning Specialization](https://learn.deeplearning.ai/certificates/d6a3b687-26ba-4937-9e18-abbb3ce46570?usp=sharing)
- [Claude Code: A Highly Agentic Coding Assistant](https://learn.deeplearning.ai/accomplishments/1aa0da77-0c19-49ac-a36f-3652f5d9bab9?usp=sharing)
- [Databases & SQL for Data Science with Python](https://www.coursera.org/account/accomplishments/verify/YY9BFB88ZGTY)
- [Python for Everybody Specialization](https://www.coursera.org/account/accomplishments/specialization/9SMN49FA2C57)
- [Prompt Engineering & Generative AI](https://www.coursera.org/account/accomplishments/verify/G8SCN6OHEXWR)

</details>

---

<div align="center">

<p><code>CHANNELS OPEN // LET'S BUILD</code></p>

<b>Open to ML internships and collaborations.</b><br />
<a href="https://naramcharan.me">naramcharan.me</a> · <a href="https://www.linkedin.com/in/naramcharan/">LinkedIn</a> · <a href="mailto:charannaram1710@gmail.com">charannaram1710@gmail.com</a>

</div>
