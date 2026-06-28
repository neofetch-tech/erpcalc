# ERPCalc 🚀

**ERPCalc** is a high-performance, lightweight Enterprise Resource Planning (ERP) manufacturing calculator built with **Python**, powered by **NumPy** for ultra-fast matrix calculations, and backed by **MongoDB** for flexible data persistence. Featuring a sleek, modern desktop interface built with **CustomTkinter**, this software provides real-time computational analysis of manufacturing timelines based on extensive construction materials and industrial workforce variables.

---

## 🔥 Key Features

- **Blazing Fast Calculations:** Heavy mathematical scheduling and timeline evaluations are handled by **NumPy**, executing data operations at native-C speeds under the hood.
- **Modern & Fluid UI:** Powered by **CustomTkinter** for a polished, dark-themed, and responsive user experience out of the box.
- **Flexible Document Database:** Leverages **MongoDB** to handle complex, dynamic schemas, allowing real-time adjustments to materials, workforce logs, and job constraints without touching the source code.
- **Proudly Open-Source:** Shared with the global developer community to showcase clean Python architecture, NoSQL integration, and data-driven desktop app workflows.

---

## 📋 Technical Specification & Business Logic

### 1. Data Models (MongoDB Collections)
The core application state maps dynamic parameters into flexible document models:

* **Materials & Production Pipelines (`Materials Collection`)**
  - `name` (String) — Name of the production task (e.g., *Bricklaying, Concrete Pouring*).
  - `volume_needed` (Float) — Total physical workload required ($m^3$, $m^2$, or specific units).
  - `speed_per_unit` (Float) — Baseline time metric needed to process a single unit of material.
  - `technological_delay` (Float) — Built-in waiting phases (e.g., hours required for concrete curing).

* **Workforce & Labor Allocations (`Workforce Collection`)**
  - `workers_count` (Integer) — Total active crew members on site.
  - `efficiency_multiplier` (Float) — Team performance index based on active industrial scaling constraints.
  - `shift_duration` (Float) — Operational working hours per individual shift.

### 2. Core Mathematical Engine
*The definitive calculation formulas, scaling parameters, and specific material metrics are currently undergoing final alignment with the Lead Project Stakeholder (Dad) 👨‍👦 and will be fully integrated using NumPy arrays upon verification.*

### 3. UI/UX Requirements
- [ ] **Modern Dashboard:** Interactive tables utilizing CustomTkinter components for monitoring asset pipelines and material status.
- [ ] **Dynamic Forms:** Easy runtime data entry fields to update material indices, labor size, and timeline limits instantly.
- [ ] **One-Click Calculation:** Quick trigger for computing heavy matrix formulas and updating the active UI view.
- [ ] **Analytical Verdict Panel:** Clean visual output display breaking down exact delivery deadlines into Days and Hours.

---

## 🛠️ Technology Stack

- **Language:** Python (v3.10+)
- **Data Engine:** NumPy (Array manipulation and optimization)
- **Database Backend:** MongoDB (using PyMongo driver)
- **GUI Framework:** CustomTkinter (Modernized Tkinter extension)
- **Development Environment:** VS Code

---

## 🚀 Getting Started (For Developers)

```bash
# Clone the repository
git clone [https://github.com/your-username/ERPCalcPy.git](https://github.com/your-username/ERPCalcPy.git)

# Navigate into the project folder
cd ERPCalcPy

# Install mandatory dependencies
pip install customtkinter numpy pymongo
