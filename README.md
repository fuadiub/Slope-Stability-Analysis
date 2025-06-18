# Slope Stability Analysis

### 📌 Purpose
This project performs a **slope stability analysis** using the **Bishop Simplified Method**. It calculates the **Factor of Safety (FoS)** for a potential circular slip failure on a homogeneous soil slope. The analysis helps identify whether the slope is stable or at risk of failure under given soil and geometric conditions.

### 🛠️ Tools Used
- **Python**
- **NumPy** for numerical computation
- **Matplotlib** for 2D visualization
- **Bishop Simplified Method** for slope stability analysis

### 📈 Key Outputs
- **FoS Calculation**: Iterative computation of the Factor of Safety for a defined circular slip surface.
- **Two Separate Visualizations**:
  - **Plot 1**: Slope geometry with vertical slices representing the division used in analysis.
  - **Plot 2**: Circular slip surface and its center point, visualized independently for clarity.

### 🧾 Interpretation
- The calculated **Factor of Safety (FoS)** is displayed on the slip surface plot.
- The analysis assumes:
  - Homogeneous soil properties
  - Zero friction angle scenario (ϕ = 0°)
  - Cohesion-controlled failure mechanism
- Separate visualizations help distinguish between the physical slope model and the theoretical failure surface, improving clarity for interpretation and reporting.

### 💡 Recommendation
This setup can be expanded to:
- Handle variable soil layers
- Include groundwater effects
- Automate search for the most critical slip surface

---

### 📊 Result Interpretation – Factor of Safety (FoS)

The **Factor of Safety (FoS)** calculated using the **Bishop Simplified Method** represents the stability condition of the slope:


#### ✅ FoS > 1.0 → Slope is Stable
- The resisting forces are greater than the driving forces.
- **In this case, FoS = 1.273**, which means the slope can resist approximately **27.3% more** driving force before failure.
- The slope is currently **considered stable**.


#### ⚠️ FoS = 1.0 → Slope is at Limit State
- The slope is **on the verge of failure**.
- Any additional load, rainfall, or disturbance may cause it to collapse.


#### ❌ FoS < 1.0 → Slope is Unstable
- The resisting forces are **less than** the driving forces.
- Failure is likely or already occurring under current conditions.

---

### 🧠 Typical Engineering Criteria:
| Slope Condition            | Minimum Recommended FoS |
|---------------------------|--------------------------|
| Temporary Excavations     | 1.2                      |
| Permanent Slopes          | 1.5                      |
| Critical Infrastructure   | 1.8 or higher            |

---

### 📝 Summary:
- The slope analyzed has a **Factor of Safety of 1.273**.
- This indicates the slope is **currently stable**, though depending on the project's requirements (e.g., permanent infrastructure), additional safety measures might be necessary.
