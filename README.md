# Aircraft Performance Calculator

A Python tool designed for calculating fundamental flight dynamics, aerodynamic forces, weight distribution, and performance metrics of an aircraft.

---

## 📌 Features

- **Range & Endurance Calculation:** Estimates maximum flight distance (in miles) and flight duration (in hours) based on fuel capacity and consumption rate.
- **Weight & Balance Analysis:** Computes total aircraft weight and Center of Gravity (CG) location.
- **Aerodynamic Forces:** Calculates aerodynamic Lift ($L$) and Drag ($D$) forces using standard fluid dynamics formulations.
- **Flight Kinematics & Dynamics:** Solves for net acceleration, velocity changes over time, and distance traveled.
- **Automated Reporting:** Formats performance metrics for console display and automatically exports results to a text summary (`aircraft_performance_analysis.txt`).

---

## 📐 Formulas & Mathematical Model

The script uses standard aerospace equations:

- **Range ($R$):**
  $$R = \left( \frac{\text{Fuel Capacity}}{\text{Fuel Consumption Rate}} \right) \times \text{True Air Speed}$$

- **Endurance ($E$):**
  $$E = \frac{\text{Fuel Capacity}}{\text{Fuel Consumption Rate}}$$

- **Aerodynamic Lift ($L$) & Drag ($D$):**
  $$L = \frac{1}{2} C_L \rho v^2 S$$
  $$D = \frac{1}{2} C_D \rho v^2 S$$

- **Center of Gravity ($\text{CG}$):**
  $$\text{CG} = \frac{\sum \text{Moments}}{\text{Total Weight}}$$

- **Acceleration ($a$):**
  $$a = \frac{T - D - W}{m}$$

---

## 🛠️ Prerequisites & Requirements

- **Python 3.8+**
- No third-party external dependencies required (uses built-in Python capabilities).

---

## 🚀 How to Run

1. Clone or navigate to the project directory:
   ```bash
   cd Aircraft_Performance
   ```

2. Run the script:
   ```bash
   python aircraft_performance_calculator.py
   ```

---

## 📄 Output Example

Upon execution, the script prints formatted results directly to the console:

```text
Performance Calculations:
Range: 3000.0 miles
Endurance: 20.0 hours
Total Weight: 11000 pounds
Center of Gravity Position: 1.1363636363636365 feet
Lift: 183750.0 Newtons
Drag: 2450.0 Newtons
Weight: 49050.0 Newtons
Acceleration: -9.1 m/s^2
Velocity: -41.0 m/s
Distance: -410.0 meters
```

Additionally, it generates a file named `aircraft_performance_analysis.txt` in the same directory containing the exported values.