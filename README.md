# Laboratorio 8 — MM3014 Teoría de Probabilidades

**Universidad del Valle de Guatemala**
Diego Andre Calderon Salazar — 241263
Pedro Julio Caso — 241286

---

## Descripción

Este repositorio contiene las etapas 3 y 4 del Laboratorio 8 del curso MM3014. Ambas etapas estudian el problema de completar un álbum de estampas mediante simulación de Monte Carlo.

- **Etapa 3 (`ej3-lab8.ipynb`):** Análisis del proceso de compra considerando un presupuesto fijo de Q1,000. Se estudia la probabilidad de completar el álbum dentro del presupuesto y el gasto esperado.

- **Etapa 4 (`ej4-lab8.ipynb`):** Incorporación de un mecanismo de intercambio: cada $K$ estampas repetidas se pueden canjear por una nueva. Se analiza cómo distintos valores de $K$ afectan el número esperado de sobres necesarios y la probabilidad de completar el álbum con un número fijo de sobres.

---

## Parámetros del modelo

| Parámetro | Valor |
|-----------|-------|
| Estampas en el álbum (N) | 100 |
| Estampas por sobre (S) | 7 |
| Precio por sobre | Q9.50 |
| Simulaciones por configuración (R) | 10,000 |
| Semilla aleatoria | 2026 |
| Valores de K explorados (Etapa 4) | 1, 2, 5, 10 |
| Valores de M explorados (Etapa 4) | 20, 25, 30, …, 70 |

---

## Requisitos

- Python 3.10, 3.11 o 3.12 recomendado (Python 3.14 puede presentar incompatibilidades con la extensión Jupyter de VS Code)
- pip

---

## Configuración del entorno

### 1. Clonar el repositorio

```bash
git clone <url-del-repo>
cd lab8-prob
```

### 2. Crear el entorno virtual

```bash
python -m venv .venv
```

### 3. Activar el entorno virtual

```bash
# Linux / macOS
source .venv/bin/activate

# Windows
.venv\Scripts\activate
```

### 4. Instalar dependencias

```bash
pip install -r requirements.txt
```

---

## Cómo ejecutar los notebooks

### Opción A — Jupyter Lab en el navegador (recomendado)

```bash
source .venv/bin/activate   # o .venv\Scripts\activate en Windows
jupyter lab
```

Se abrirá automáticamente en el navegador. Desde ahí abrir `ej3-lab8.ipynb` o `ej4-lab8.ipynb` y ejecutar las celdas en orden con **Run All**.

### Opción B — VS Code

1. Abrir la carpeta del proyecto en VS Code.
2. Instalar las extensiones **Python** y **Jupyter** si no están instaladas.
3. Abrir el notebook deseado.
4. En el selector de kernel (arriba a la derecha), elegir **Select Another Kernel → Python Environments** y seleccionar el intérprete de `.venv`.
5. Ejecutar las celdas con **Run All**.

> Si el kernel queda en estado de carga indefinida en VS Code, usar la Opción A y conectar VS Code al servidor local con `Ctrl+Shift+P` → *Jupyter: Specify Jupyter Server for Connections* → pegar la URL que aparece en la terminal al ejecutar `jupyter lab`.

---

## Estructura del repositorio

```
lab8-prob/
├── ej3-lab8.ipynb       # Etapa 3: simulación con presupuesto
├── ej4-lab8.ipynb       # Etapa 4: simulación con mecanismo de intercambio
├── requirements.txt     # Dependencias de Python
└── README.md
```

---

## Dependencias principales

| Librería | Uso |
|----------|-----|
| `numpy` | Generación de números aleatorios y operaciones vectorizadas |
| `matplotlib` | Visualización de histogramas y curvas de probabilidad |
| `pandas` | Manejo de datos tabulares |
| `jupyter` / `ipykernel` | Ejecución de los notebooks |
