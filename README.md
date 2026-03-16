https://doi.org/10.5281/zenodo.19045363
# GRA Ramanujan Playground

Evolutionary formula discovery with **GRA Meta-Nullification**.

This playground shows how a multilevel GRA foam functional can discover symbolic formulas for constants (π, e, ln 2) and balance three goals:
- numerical accuracy,
- simplicity,
- Ramanujan-style structural beauty (powers, logs, meaningful constants). [web:848][web:865]

---

## Live Demo

Try it in your browser (no install needed):

- GRA Ramanujan Generator (Bolt demo):  
  https://gra-ramanujan-evolut-rvxf.bolt.host/ [web:877]

The full engine currently lives in a **private research repository**.  
This public playground demonstrates the idea and provides an online demo.

---

## For students / Для школьников

🇬🇧 **For students**

GRA Ramanujan Generator is a **math playground** for curious kids and students. [web:842]  
You pick a target number (π, e, ln 2), press “Run”, and watch how the AI evolves smarter and smarter formulas over generations. [web:842][web:863]  
You can compare which formulas are more accurate, which are simpler, and which ones look more “beautiful”.  
Teachers can use it in class to show that mathematics is not only final answers in a textbook, but also exploration, experiments, and creative thinking. [web:866][web:869]  

🇷🇺 **Для школьников и студентов**

GRA Ramanujan Generator — это математическая **игра с формулами**. [web:842]  
Вы выбираете число (π, e, ln 2), запускаете эволюцию и смотрите, как ИИ шаг за шагом придумывает всё более умные формулы. [web:842][web:863]  
Можно сравнивать: какие формулы точнее, какие короче, какие выглядят «красивее».  
Учитель может использовать это на уроке, чтобы показать, что математика — это не только готовые ответы из учебника, но и живой поиск и эксперименты. [web:866][web:869]  

---

## GRA Foam Experiment

We compare two setups:

1. **Without Ramanujan prior (2-level GRA):**  
   \(\Phi_{\mathrm{GRA}} = \alpha\Phi^{(0)} + (1-\alpha)\Phi^{(1)}\),  
   where \(\Phi^{(0)} = \text{error}\), \(\Phi^{(1)} = \text{error} + \lambda\cdot\text{complexity}\).  
   The system often finds trivial numeric hacks like `sqrt(9.901)` with low error but no structural meaning. [web:848][web:852]  

2. **With Ramanujan structural prior (3-level GRA):**  
   \(\Phi_{\mathrm{GRA}} = \alpha_0\Phi^{(0)} + \alpha_1\Phi^{(1)} + \alpha_2\Phi^{(2)}\),  
   where \(\Phi^{(2)}\) rewards Ramanujan-style structures (powers, ln 2, π, simple rationals) and penalizes noisy constants. [web:848]  

For the target **e**, a typical best formula with the 3-level GRA is:

- `(4.227 pow ln2)`  
- numerical error ≈ 2.4·10⁻³ (2.7159 vs e ≈ 2.7183),  
- low complexity = 3,  
- strongly negative Φ⁽²⁾ (structure) because it uses `ln 2` instead of random constants. [web:846][web:859][web:848]  

This shows how the GRA foam functional can steer symbolic regression toward **interpretable, structurally meaningful formulas**, not just overfitted numerical expressions. [web:848][web:865]  

---

## Why it matters

- **AI for science:** Prototype of a multilevel symbolic regression engine that can be adapted to scientific data (physics, chemistry, soft sensors) to discover interpretable equations, not only black-box models. [web:865][web:868]  
- **Education:** An interactive way to show students how formulas and conjectures can emerge from search and experiments, similar in spirit to the Ramanujan Machine. [web:842][web:863]  
- **Extensible:** The same GRA foam mechanism (error + complexity + structure) can be reused for models and theories, not only for pure math constants. [web:848][web:871]  
