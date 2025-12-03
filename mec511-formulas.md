# MEC 511: Thermodynamics and Fluids - Formula Sheet

---

## 1. FLUID PROPERTIES & FUNDAMENTALS

### Basic Definitions
- **Density:** ρ = m/V [kg/m³]
- **Specific Volume:** v = V/m = 1/ρ [m³/kg]
- **Specific Weight:** γ = ρg [N/m³]
- **Specific Gravity:** SG = ρ/ρ_H₂O (where ρ_H₂O = 1000 kg/m³)

### Shear Stress
- **Shear Stress:** τ = F_shear/A [Pa]
- **Newtonian Fluid:** τ = μ(du/dy) [Pa]

### Viscosity
- **Dynamic Viscosity:** μ [Pa·s or kg/(m·s)]
- **Kinematic Viscosity:** ν = μ/ρ [m²/s]

---

## 2. PRESSURE

### Pressure Relations
- **Absolute Pressure:** P_abs = P_atm + P_gauge
- **Vacuum Pressure:** P_vac = P_atm - P_abs
- **Hydrostatic Pressure:** P = P_atm + ρgh
- **Pressure Variation with Depth:** P_below = P_above + ρgΔz
- **Gauge Pressure at Depth h:** P_gauge = ρgh

---

## 3. IDEAL GAS LAW

### Various Forms
- **With moles:** PV = nR̄T
- **With mass:** PV = mRT
- **Specific form:** Pv = RT
- **Molar form:** PV̄ = R̄T

### Constants
- **Universal Gas Constant:** R̄ = 8.314 J/(mol·K) = 8.314 kPa·m³/(kmol·K)
- **Specific Gas Constant:** R = R̄/M (M = molar mass)
- **For Air:** R = 0.287 kJ/(kg·K)

---

## 4. THERMODYNAMIC PROPERTIES

### Enthalpy
- **Definition:** h = u + Pv [kJ/kg]

### Quality (Two-Phase Mixtures)
- **Quality:** x = m_vapor/m_total
- **Any Property:** φ_x = φ_f + x(φ_g - φ_f) where φ = v, u, h, or s
- **Alternative:** φ_x = (1-x)φ_f + xφ_g

### Specific Heats
- **At constant volume:** c_v = (∂u/∂T)_v
- **At constant pressure:** c_p = (∂h/∂T)_p
- **Ideal Gas Relation:** c_p = c_v + R
- **Specific Heat Ratio:** k = c_p/c_v

### Internal Energy & Enthalpy Changes (Ideal Gas)
- **Δu = c_v,avg(T₂ - T₁)** [kJ/kg]
- **Δh = c_p,avg(T₂ - T₁)** [kJ/kg]

---

## 5. ENERGY

### Kinetic & Potential Energy
- **Kinetic Energy:** KE = ½mV² [kJ], ke = V²/2 [kJ/kg]
- **Potential Energy:** PE = mgz [kJ], pe = gz [kJ/kg]

---

## 6. WORK

### Boundary Work
- **General:** W_b = ∫PdV [kJ]

### Process-Specific Work
| Process | Work Formula |
|---------|--------------|
| Isochoric (V = const) | W = 0 |
| Isobaric (P = const) | W = P(V₂ - V₁) |
| Isothermal (T = const, ideal gas) | W = P₁V₁ ln(V₂/V₁) = mRT ln(V₂/V₁) |
| Polytropic (PVⁿ = C) | W = (P₂V₂ - P₁V₁)/(1-n) |

### Other Work Forms
- **Shaft Work:** Ẇ_sh = 2πṅT [W] (ṅ = rev/s, T = torque)
- **Spring Work:** W_spring = ½k(x₂² - x₁²)
- **Electrical Work:** W_e = VIt [kJ]

---

## 7. FIRST LAW OF THERMODYNAMICS

### Closed System (Control Mass)
- **Energy Balance:** ΔU = Q - W
- **Full Form:** m(u₂ - u₁) + ½m(V₂² - V₁²) + mg(z₂ - z₁) = Q - W
- **For Cycles:** Q_cycle = W_cycle

### Open System (Control Volume) - Steady State
- **Mass Balance:** Σṁ_in = Σṁ_out
- **Mass Flow Rate:** ṁ = ρVA = AV/v
- **Volume Flow Rate:** V̇ = AV = ṁv

- **Energy Balance (Steady Flow):**
  Q̇ - Ẇ = Σṁ_out(h + V²/2 + gz) - Σṁ_in(h + V²/2 + gz)

- **Single Inlet/Outlet:**
  q - w = (h₂ - h₁) + (V₂² - V₁²)/2 + g(z₂ - z₁)

---

## 8. SECOND LAW & ENTROPY

### Entropy Definition
- **Differential Form:** dS = (δQ/T)_int,rev

### Entropy Change
- **Liquids/Solids:** s₂ - s₁ = c_avg ln(T₂/T₁)

### Ideal Gas Entropy Change
- **Form 1:** s₂ - s₁ = c_v,avg ln(T₂/T₁) + R ln(v₂/v₁)
- **Form 2:** s₂ - s₁ = c_p,avg ln(T₂/T₁) - R ln(P₂/P₁)
- **Using Tables:** s₂ - s₁ = s°₂ - s°₁ - R ln(P₂/P₁)

### Entropy Balance
- **Closed System:** ΔS_sys = ΣQ_k/T_k + S_gen
- **Open System (Steady):** 0 = ΣQ̇_k/T_k + Σṁ_i·s_i - Σṁ_e·s_e + Ṡ_gen

### Entropy Generation
- S_gen > 0: Irreversible
- S_gen = 0: Reversible
- S_gen < 0: Impossible

---

## 9. ISENTROPIC RELATIONS (IDEAL GAS)

### Temperature-Volume-Pressure Relations (s = constant)
- **(T₂/T₁) = (v₁/v₂)^(k-1)**
- **(T₂/T₁) = (P₂/P₁)^((k-1)/k)**
- **(P₂/P₁) = (v₁/v₂)^k**

---

## 10. HEAT ENGINES, REFRIGERATORS & HEAT PUMPS

### Heat Engine
- **Thermal Efficiency:** η_th = W_net,out/Q_in = 1 - Q_out/Q_in
- **Net Work:** W_net = Q_in - Q_out

### Carnot Efficiency
- **η_th,Carnot = 1 - T_L/T_H** (temperatures in Kelvin)

### Refrigerator (COP)
- **COP_R = Q_L/W_net,in = Q_L/(Q_H - Q_L)**
- **Carnot COP_R = T_L/(T_H - T_L)**

### Heat Pump (COP)
- **COP_HP = Q_H/W_net,in = Q_H/(Q_H - Q_L)**
- **Carnot COP_HP = T_H/(T_H - T_L)**
- **Relation:** COP_HP = COP_R + 1

---

## 11. ISENTROPIC EFFICIENCIES

### Turbine
- **η_T = (h₁ - h₂ₐ)/(h₁ - h₂ₛ) = W_actual/W_isentropic**

### Compressor/Pump
- **η_C = (h₂ₛ - h₁)/(h₂ₐ - h₁) = W_isentropic/W_actual**
- **Pump:** η_P = v(P₂ - P₁)/(h₂ₐ - h₁)

### Nozzle
- **η_N = (V₂ₐ²)/(V₂ₛ²) = (h₁ - h₂ₐ)/(h₁ - h₂ₛ)**

---

## 12. POWER CYCLES

### General Definitions
- **Compression Ratio:** r_comp = V_max/V_min
- **Pressure Ratio:** r_P = P₂/P₁
- **Cutoff Ratio:** r_cut = V₃/V₂
- **Back Work Ratio:** r_bw = W_comp/W_turb
- **Mean Effective Pressure:** MEP = W_cycle/(V_max - V_min)

### Otto Cycle (Spark Ignition)
- **Efficiency:** η_Otto = 1 - 1/r_comp^(k-1)
- **Processes:** 1-2: Isentropic compression, 2-3: Constant V heat addition, 3-4: Isentropic expansion, 4-1: Constant V heat rejection

### Diesel Cycle (Compression Ignition)
- **Efficiency:** η_Diesel = 1 - (1/r_comp^(k-1))·[(r_cut^k - 1)/(k(r_cut - 1))]
- **Processes:** 1-2: Isentropic, 2-3: Constant P, 3-4: Isentropic, 4-1: Constant V

### Brayton Cycle (Gas Turbine)
- **Efficiency:** η_Brayton = 1 - 1/r_P^((k-1)/k)
- **Processes:** 1-2: Isentropic compression, 2-3: Constant P heat addition, 3-4: Isentropic expansion, 4-1: Constant P heat rejection

### Rankine Cycle (Steam Power)
- **Efficiency:** η_Rankine = (W_turb - W_pump)/Q_in = [(h₁ - h₂) - (h₄ - h₃)]/(h₁ - h₄)
- **Processes:** 1-2: Isentropic turbine, 2-3: Constant P condenser, 3-4: Isentropic pump, 4-1: Constant P boiler

---

## 13. FLUID MECHANICS - CONTINUITY

### Conservation of Mass
- **Integral Form:** ∂/∂t ∫∫∫ρdV + ∫∫ρV⃗·dA⃗ = 0
- **Steady Flow:** ṁ_in = ṁ_out
- **Incompressible:** A₁V₁ = A₂V₂

---

## 14. BERNOULLI EQUATION

### Standard Form (Incompressible, Inviscid, Steady)
**P₁/γ + V₁²/2g + z₁ = P₂/γ + V₂²/2g + z₂**

Or equivalently:
**P₁ + ½ρV₁² + ρgz₁ = P₂ + ½ρV₂² + ρgz₂**

### Terms
- P/γ or P/(ρg): Pressure head
- V²/2g: Velocity head
- z: Elevation head

### Energy Form (with losses)
**P₁/γ + α₁V₁²/2g + z₁ + h_pump = P₂/γ + α₂V₂²/2g + z₂ + h_turbine + h_loss**

where α = 1.0 (turbulent), α = 2.0 (laminar)

---

## 15. REYNOLDS NUMBER & FLOW REGIMES

### Reynolds Number
**Re = ρVD/μ = VD/ν**

### Flow Classification
- Re < 2300: Laminar
- 2300 < Re < 4000: Transitional
- Re > 4000: Turbulent

---

## 16. PIPE FLOW

### Major (Friction) Losses
**h_L = f(L/D)(V²/2g)** (Darcy-Weisbach)

### Friction Factor
- **Laminar:** f = 64/Re
- **Turbulent (Colebrook):** 1/√f = -2.0 log[(ε/D)/3.7 + 2.51/(Re√f)]
- **Explicit Approximation:** f₀ = 0.25[log(ε/D/3.7 + 5.74/Re^0.9)]^(-2)

### Minor Losses
**h_L,minor = K_L(V²/2g)** or **h_L,minor = f(L_eq/D)(V²/2g)**

### Hydraulic Diameter (Non-Circular)
**D_h = 4A/P** (A = area, P = perimeter)

---

## 17. LAMINAR PIPE FLOW

### Velocity Profile (Circular Pipe)
**u(r) = (ΔP/4μL)(R² - r²)**

### Maximum Velocity
**u_max = (ΔP·R²)/(4μL)** (at centerline)

### Average Velocity
**V_avg = u_max/2**

### Volume Flow Rate (Hagen-Poiseuille)
**Q = (πΔPR⁴)/(8μL) = (πΔPD⁴)/(128μL)**

---

## 18. DIMENSIONAL ANALYSIS

### Key Dimensionless Numbers
| Number | Formula | Physical Meaning |
|--------|---------|------------------|
| Reynolds (Re) | ρVL/μ | Inertia/Viscous |
| Froude (Fr) | V/√(gL) | Inertia/Gravity |
| Euler (Eu) | ΔP/(ρV²) | Pressure/Inertia |
| Mach (Ma) | V/c | Velocity/Sound speed |
| Weber (We) | ρV²L/σ | Inertia/Surface tension |
| Cavitation (Ca) | (P - P_v)/(½ρV²) | Pressure/Inertia |

### Buckingham Pi Theorem
Number of dimensionless groups = n - r
(n = number of variables, r = number of fundamental dimensions)

---

## 19. IMPORTANT CONSTANTS

| Property | SI Value |
|----------|----------|
| Standard Atmosphere | 101.325 kPa |
| Water Density (4°C) | 1000 kg/m³ |
| Air Density (STP) | 1.225 kg/m³ |
| g (Earth) | 9.81 m/s² |
| R̄ (Universal) | 8.314 kJ/(kmol·K) |
| R (Air) | 0.287 kJ/(kg·K) |
| c_p (Air, 300K) | 1.005 kJ/(kg·K) |
| c_v (Air, 300K) | 0.718 kJ/(kg·K) |
| k (Air) | 1.4 |

---

## 20. QUICK REFERENCE: STATE DETERMINATION

### Compressed Liquid
- P > P_sat at given T
- T < T_sat at given P
- v < v_f, u < u_f, h < h_f, s < s_f

### Saturated Liquid-Vapor Mixture
- v_f ≤ v ≤ v_g (similarly for u, h, s)
- Use quality x to find properties

### Superheated Vapor
- P < P_sat at given T
- T > T_sat at given P
- v > v_g, u > u_g, h > h_g, s > s_g

---

## 21. TdS EQUATIONS

### First TdS Equation
**Tds = du + Pdv**

### Second TdS Equation
**Tds = dh - vdP**

---

*Formula sheet compiled from MEC 511: Thermodynamics and Fluids course materials at TMU*
