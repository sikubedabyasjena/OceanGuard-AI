# OceanGuard-AI
# 🌊 OceanGuard AI

OceanGuard AI is an environmental monitoring system that helps identify and assess ocean and coastal hazards from citizen reports. It analyzes observations submitted by users and provides a quick assessment of the potential issue, its severity, recommended actions, and cleanup guidance.

The goal is to support communities, environmental organizations, and local authorities in detecting and responding to marine environmental threats more efficiently.

---

## 🚀 Features

* Detects environmental incidents from natural language reports
* Classifies potential marine hazards
* Generates risk scores and severity levels
* Provides recommended response actions
* Creates authority-ready incident reports
* Suggests cleanup and mitigation plans
* Works with simple citizen observations

---

## 🌍 Supported Incident Types

### 🛢️ Oil or Chemical Pollution

Detects signs of:

* Oil spills
* Fuel leaks
* Chemical contamination
* Rainbow sheen on water
* Strong chemical odors

### 🐟 Marine Life Distress

Detects reports involving:

* Dead fish
* Dead turtles
* Dead dolphins
* Injured marine animals
* Floating fish

### ♻️ Plastic Pollution

Detects:

* Plastic waste
* Bottles and wrappers
* Garbage accumulation
* Foam and thermocol waste
* Microplastics

### 💧 Water Contamination

Detects:

* Sewage discharge
* Wastewater pollution
* Brown or green water
* Algae blooms
* Sludge accumulation

### 🎣 Illegal Fishing Activity

Detects:

* Illegal fishing operations
* Blast fishing
* Poison fishing
* Suspicious trawler activity
* Night fishing operations

### 🌱 Coral or Habitat Damage

Detects:

* Coral reef destruction
* Broken coral
* Mangrove damage
* Seagrass damage
* Anchor-related habitat destruction

---

## ⚙️ How It Works

1. A user submits an environmental observation.
2. The report text is cleaned and analyzed.
3. Keywords are matched against known environmental threats.
4. A risk score is generated.
5. The most likely issue is identified.
6. Severity is assigned.
7. Recommended actions and cleanup plans are produced.
8. An authority-ready report is generated.

---

## 📊 Severity Levels

| Risk Score | Severity  |
| ---------- | --------- |
| 80 – 100   | Emergency |
| 65 – 79    | High      |
| 40 – 64    | Medium    |
| 0 – 39     | Low       |

---

## 📝 Example Report

### Input

```python
location = "Puri Beach, Odisha"

report = """
Black oily liquid floating on water,
strong smell, and dead fish near shore.
"""

result = run_agent(location, report)
```

### Output

```text
Issue: Possible Oil or Chemical Pollution
Severity: Emergency
Confidence: 95

Reasons:
- Detected terms: black liquid, strong smell
- Highest-risk issue selected.
- Related concerns: Marine Life Distress
```

### Recommended Actions

* Keep people away from the area
* Avoid touching chemicals or dead animals
* Contact authorities immediately
* Record exact location and time
* Take photos if safe

---

## 📂 Project Structure

```text
OceanGuardAI/
│
├── oceanguard.py
├── README.md
└── requirements.txt
```

---

## ▶️ Running the Project

Clone the repository:

```bash
git clone https://github.com/yourusername/OceanGuardAI.git
cd OceanGuardAI
```

Run the application:

```bash
python oceanguard.py
```

No external dependencies are required. The project uses only Python standard libraries.

---

## 🏗️ Core Components

### `detect_issue()`

Identifies the most likely environmental issue from the report.

### `severity_from_score()`

Converts risk scores into severity categories.

### `action_plan()`

Generates response recommendations based on severity.

### `cleanup_plan()`

Provides cleanup guidance for the detected issue.

### `build_report()`

Creates an official authority-style incident report.

### `run_agent()`

Main function that performs the complete analysis workflow.

---

## 🔮 Future Enhancements

* GPS-based incident reporting
* Mobile application integration
* AI image analysis for pollution detection
* Real-time alerts to authorities
* Environmental monitoring dashboard
* Machine learning-based classification
* Multi-language support
* Historical incident tracking
* GIS and satellite data integration

---

## 🎯 Use Cases

* Coastal pollution monitoring
* Beach cleanup initiatives
* Marine conservation projects
* Citizen science programs
* Environmental NGOs
* Government monitoring agencies
* Disaster response teams
* Smart city environmental systems

---

## 🌊 Vision

OceanGuard AI aims to empower citizens to become active contributors to ocean conservation. By transforming simple observations into actionable environmental intelligence, communities can help protect marine ecosystems and respond more effectively to environmental threats.

Every report matters. Every observation helps. Together, we can build healthier oceans for future generations.

---

## 📜 License

MIT License

---

## 👨‍💻 Author
Siku Bedabyas Jena



Protecting oceans through intelligent environmental monitoring and citizen-powered reporting.

