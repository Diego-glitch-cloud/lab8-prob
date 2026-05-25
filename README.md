# Lab 8 — MM3014 Teoría de Probabilidades

## Setup rápido

### 1. Crear y activar el entorno virtual

```bash
python -m venv .venv
source .venv/bin/activate        # Linux/macOS
# .venv\Scripts\activate         # Windows
```

### 2. Instalar dependencias

```bash
pip install -r requirements.txt
```

### 3. Registrar el kernel en Jupyter

```bash
python -m ipykernel install --user --name=lab8-prob --display-name "Lab8 Probabilidades"
```

### 4. Abrir Jupyter

```bash
jupyter notebook
```

---

## Notebooks

| Archivo | Contenido |
|---------|-----------|
| `ej3-lab8.ipynb` | Etapa 3: Incorporación del presupuesto y costo |
| `ej4-lab8.ipynb` | Etapa 4: Efecto del intercambio de repetidas |

---

## Parámetros generales

| Parámetro | Valor |
|-----------|-------|
| N (estampas) | 100 |
| S (estampas/sobre) | 7 |
| Precio por sobre | Q9.50 |
| Presupuesto (Etapa 3) | Q1000 |
| Simulaciones (R) | 10,000 |
| Semilla | 2026 |
| K valores (Etapa 4) | 1, 2, 5, 10 |
