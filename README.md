# WFP ET – Targeting Verification Sampling App (Somali RAM)

**v3.2 FULL BUILD**
- Preserves **all original fields**.
- **Unique-only** (no replacement) sampling.
- **Reallocate shortfalls** within kebele.
- **Auto-add extra villages** (optional): if selected villages cannot meet per‑group target, add more villages from the same kebele (configurable max; PPS or largest-capacity strategy).
- Fixes for NumPy dtype and kebele summary concat.

## Run
```bash
python -m venv .venv
. .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -r requirements.txt
streamlit run app.py
```

## Docker
```bash
docker build -t wfp-verification-sampling:v3.2 .
docker run -p 8501:8501 wfp-verification-sampling:v3.2
```
