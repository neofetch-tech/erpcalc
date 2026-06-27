# ERPCalc++ 🚀

**ERPCalc++** is a high-performance, lightweight Enterprise Resource Planning (ERP) manufacturing calculator written in pure, hardcore C++ utilizing the **Dear ImGui** graphical framework. Designed with absolute efficiency in mind, this software provides real-time computational analysis of manufacturing timelines based on construction materials, personnel allocation, shift durations, and operational efficiency metrics.

---

## 🔥 Key Features

- **Hardware-Level Performance (Hardcore C++):** Zero runtime overhead. Complex computations over large datasets execute at bare-metal speeds.
- **Modern & Lightweight GUI:** Powered by **Dear ImGui** (with GLFW + OpenGL3 backend) for an engineered, ultra-responsive, zero-latency user experience.
- **Standalone Portability (Single `.exe`):** Compiles cleanly into a single independent binary file with zero external dynamic link library (`.dll`) dependencies. Fully portable for instant production deployment.
- **Proudly Open-Source:** Shared with the global developer community to demonstrate structural architecture, manual memory management optimization, and robust GUI workflows in C++.

---

## 📋 Technical Specification & Business Logic

### 1. Data Structures (`struct`)
The core application state operates around two critical architectural entities:

* **Materials & Production Processes (`struct Material`)**
  - `std::string name` — Name of the production task (e.g., *Bricklaying, Concrete Pouring*).
  - `double volumeNeeded` — Total physical workload required (measured in $m^3$, $m^2$, or units).
  - `double speedPerUnit` — Standard time metric required to process a single unit of material.

* **Workforce & Labor Management (`struct WorkForce`)**
  - `int workersCount` — Number of active workers assigned to the specific crew.
  - `double efficiency` — Team performance multiplier (e.g., `1.0` for standard baseline, `1.2` for high-velocity output).
  - `double shiftHours` — Actual operational working hours per shift (e.g., 8 hours/day).

### 2. Core Mathematical Engine
*The definitive calculation formulas and technical constraints are currently undergoing final alignment with the Lead Project Stakeholder and will be hardcoded upon verification.*

### 3. UI/UX Requirements
- [ ] **Dynamic Data Table:** Live tracking of available construction assets, active pipelines, and raw material throughput.
- [ ] **Intuitive Forms:** Instant runtime entry and structural updates for labor forces and resource constraints.
- [ ] **One-Click Execution:** Real-time evaluation button rendering instant scheduling insights.
- [ ] **Analytical Verdict Panel:** Clean display of final manufacturing deadlines broken down precisely into Days and Hours.

---

## 🛠️ Technology Stack

- **Language:** Standard C++ (C++17 / C++20 ISO Standard)
- **GUI Framework:** [Dear ImGui](https://github.com/ocornut/imgui) (Immediate Mode Graphical User Interface)
- **Windowing & Rendering Backend:** GLFW / OpenGL3
- **Environment & Compiler:** VS Code / GCC (MinGW-w64)

---

## 🚀 Getting Started (For Developers)

```bash
# Clone the repository
git clone [https://github.com/your-username/ERPCalcPlusPlus.git](https://github.com/your-username/ERPCalcPlusPlus.git)

# Navigate into the project folder
cd ERPCalcPlusPlus
