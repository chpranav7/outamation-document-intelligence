# Outamation — Document Intelligence (OCR + RAG)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1erSRle1QbNECqvSnjMejS_-noiQ_9CFD)

End-to-end document intelligence prototype built during the **Outamation AI-Powered Workflow Automation Externship**.  
It demonstrates a workflow for processing mortgage-style documents using **OCR + PDF parsing + information extraction + Retrieval-Augmented Generation (RAG)**, with a **Gradio UI** for interaction.

> Note: Gradio “share” links generated from Colab are temporary. Re-run the notebook to generate a new live link.

---

## Demo
![Gradio Demo](assets/gradio_demo.png)
<sub>Gradio UI demo generated from the Colab notebook.</sub>

---

## What this project does

Given a PDF/image document, the pipeline can:
- Read text from PDFs and scanned pages (**OCR**)
- Parse and clean extracted text (**document preprocessing**)
- Retrieve relevant chunks and answer questions using **RAG**
- Provide an interactive **Gradio UI** to test the system end-to-end

---

## Key components

- **Ingestion & parsing**: PDF parsing + page/image handling  
- **OCR**: extraction for scanned/embedded text (externship exercises + comparisons)  
- **RAG**: chunking → indexing → retrieval → answer generation  
- **UI**: Gradio interface for upload/Q&A and quick iteration  

---

## How to run

### Option 1 — Run in Colab (recommended)
1. Click the **Open in Colab** badge at the top  
2. **Runtime → Run all**  
3. Open the Gradio link printed in the output

### Option 2 — Run locally (optional)
If you add a `requirements.txt`:

```bash
pip install -r requirements.txt
