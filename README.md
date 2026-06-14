# 📐 Fundamentals of 3D Printing and Manufacturing Tolerances

## 🔧 FDM/FFF Technology

**FDM (Fused Deposition Modeling)** is a process in which a plastic filament is melted in an extruder and deposited layer by layer to build a part.

> ⚠️ **Note:** FDM is a registered trademark of Stratasys. In open-source and general industry contexts, the same process is commonly referred to as **FFF (Fused Filament Fabrication)**.

---

## 📏 Manufacturing Tolerances (per GOST 30893.1 / ISO 2768)

### Tolerance Grades
The **lower** the grade number, the **higher** the precision:

| Grade | Application | Examples |
|-------|-------------|----------|
| IT01–IT4 | Precision mechanisms | Watch components, aerospace |
| IT5–IT7 | Critical fits and assemblies | Bearing assemblies |
| IT8–IT11 | General machine building | Gears, shafts |
| **IT12–IT14** | **3D printing, casting, prototypes** | **Enclosures, mock-ups, brackets** |

### Tolerance Designations

- **H** (uppercase) — tolerance for **holes** (deviation in the positive direction)
- **h** (lowercase) — tolerance for **shafts** (deviation in the negative direction)
- **IT12/2** — symmetric tolerance (± half of the IT12 value)

### Example Calculation

**Dimension:** 50 mm  
**Tolerance:** IT12/2

1. Per GOST for the 30–50 mm range: IT12 = 0.25 mm
2. Symmetric tolerance: ±0.125 mm
3. **Result:** the dimension must fall within **49.875 – 50.125 mm**

---

## 🎯 Where Are IT12–IT14 Tolerances Applicable?

✅ FDM 3D printing (without post-processing)  
✅ Rapid prototyping  
✅ Sand casting  
✅ Non-critical parts: enclosures, decorative elements, brackets  

❌ **Not suitable for:**
- Precision fits (bearings, gears)
- Tight interference fits without clearance
- Parts requiring machining

---

## 💡 Practical Recommendations

1. **Design in clearance** for mating parts (make holes 0.2–0.3 mm larger than the corresponding shaft)
2. **Account for material shrinkage** (PLA ~0.2–0.5%, PETG ~0.2–1.0%, TPU 95A ~0.4–1.4%)
3. **Improve accuracy** with post-processing: reaming holes, sanding surfaces
4. **Calibrate the printer** before printing critical parts

---

📚 **Standards:** GOST 30893.1-2002, GOST 25346-2013, ISO 2768-1, ISO 286-1
