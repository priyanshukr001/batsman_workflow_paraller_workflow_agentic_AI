# 🏏 Batsman Parallel Workflow | Agentic AI

A cricket statistics analysis project demonstrating how a workflow can process batting performance data and generate meaningful performance metrics from a structured input state.

## 🚀 Project Overview

This project analyses a batsman's performance using match statistics such as total runs, balls faced, fours, and sixes.

The workflow takes an initial state as input, processes the batting statistics, and returns additional performance indicators along with a summary.

The project is part of my journey into **Agentic AI and workflow orchestration**, where I am exploring how independent tasks can be organised and executed through structured workflows.

## 🎯 Objectives

- Understand workflow-based execution using Python.
- Explore parallel workflow orchestration.
- Process structured cricket statistics.
- Calculate meaningful batting performance metrics.
- Generate a consolidated performance summary.

## ⚙️ Input Data

The workflow accepts the following initial state:

| Parameter | Value |
|---|---:|
| Runs | 100 |
| Balls Faced | 50 |
| Fours | 6 |
| Sixes | 4 |

## 📊 Performance Metrics

Based on the sample execution, the workflow generates the following metrics:

| Metric | Result |
|---|---:|
| Strike Rate | 200.0 |
| Balls per Boundary | 5.0 |
| Boundary Percentage | 48.0% |

### Understanding the Metrics

**1. Strike Rate**

Measures the number of runs scored per 100 balls faced.

Formula: `(Runs / Balls Faced) × 100`

**2. Balls per Boundary**

Measures how frequently the batsman hits a boundary.

Formula: `Balls Faced / (Fours + Sixes)`

**3. Boundary Percentage**

Measures the percentage of total runs scored through fours and sixes.

Formula: `((Fours × 4) + (Sixes × 6)) / Runs × 100`

## 🧠 Workflow Execution

The notebook demonstrates how an initial state is passed into a workflow using:

`workflow.invoke(initial_state)`

The workflow processes the input and returns the original batting statistics along with calculated metrics and a performance summary.

The project is intended to demonstrate parallel workflow orchestration: independent calculations can be organised as separate tasks and combined into a final result.

## 🛠️ Tech Stack

- **Language:** Python
- **Workflow Orchestration:** LangGraph
- **Environment:** Jupyter Notebook
- **Concepts:** State Management, Workflow Execution, Parallel Processing, Data Analysis

## 📂 Project Structure

```text
batsman_workflow_paraller_workflow_agentic_AI/
│
├── 4_batsman_workflow.ipynb
└── README.md
```

## 💻 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/priyanshukr001/batsman_workflow_paraller_workflow_agentic_AI.git
```

### 2. Navigate to the project directory

```bash
cd batsman_workflow_paraller_workflow_agentic_AI
```

### 3. Create a virtual environment

```bash
python3 -m venv myenv
```

### 4. Activate the environment

For macOS/Linux:

```bash
source myenv/bin/activate
```

### 5. Install the required package

```bash
python -m pip install langgraph jupyter
```

### 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `4_batsman_workflow.ipynb` and execute the notebook cells.

## 📈 Sample Output

For the sample input:

```python
initial_state = {
    'runs': 100,
    'balls': 50,
    'fours': 6,
    'sixes': 4
}
```

The workflow returns additional values including:

```python
{
    'runs': 100,
    'balls': 50,
    'fours': 6,
    'sixes': 4,
    'sr': 200.0,
    'bpb': 5.0,
    'boundary_percent': 48.0
}
```

The workflow also generates a readable performance summary.

## 🔮 Future Enhancements

- Extend the workflow to analyse multiple players.
- Add comparative batting performance analysis.
- Integrate ball-by-ball match statistics.
- Build a dashboard for cricket performance insights.
- Explore LLM-powered cricket analysis and AI agents.

## 👨‍💻 Author

**Priyanshu Kumar**

Mathematics and Computing | Delhi Technological University

- GitHub: [@priyanshukr001](https://github.com/priyanshukr001)
- LinkedIn: [Priyanshu Kumar](https://www.linkedin.com/in/priyanshu-kumar-68a736229/)

---

⭐ If you find this project interesting, consider giving the repository a star!
