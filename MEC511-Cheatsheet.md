# MEC 511: Thermodynamics & Fluids - COMPREHENSIVE CHEATSHEET

**Course**: MEC 511 (TMU) | **Textbooks**: A Brief Introduction to Fluid Mechanics by Young et al., Fundamentals of Engineering Thermodynamics by Moran et al.

---

## TABLE OF CONTENTS
1. [Unit Systems & Conversions](#unit-systems--conversions)
2. [Fluid Properties](#fluid-properties)
3. [Fluid Statics](#fluid-statics)
4. [Fluid Dynamics - Bernoulli & Continuity](#fluid-dynamics--bernoulli--continuity)
5. [Control Volumes & Mass Conservation](#control-volumes--mass-conservation)
6. [Thermodynamic First Law](#thermodynamic-first-law)
7. [Closed System Processes](#closed-system-processes)
8. [Pure Substances & Phase Properties](#pure-substances--phase-properties)
9. [Ideal Gases](#ideal-gases)
10. [Steady-Flow Energy Equation](#steady-flow-energy-equation)
11. [Common Symbol Reference](#common-symbol-reference)

---

## 1. UNIT SYSTEMS & CONVERSIONS

### MLT vs FLT Systems

| Quantity | MLT System | FLT System | SI Units |
|----------|-----------|-----------|----------|
| Mass | M | F·T²/L | kg |
| Force | M·L/T² | F | N |
| Pressure | M/(L·T²) | F/L² | Pa = N/m² |
| Energy/Work | M·L²/T² | F·L | J = N·m |

### Common Conversions (SI to BG Units)

| Parameter | From SI | To BG | Multiply by |
|-----------|---------|-------|------------|
| Length (m) | - | ft | 3.281 |
| Mass (kg) | - | slug | 6.852 × 10⁻² |
| Density (kg/m³) | - | slug/ft³ | 1.940 × 10⁻³ |
| Pressure (N/m²) | - | psi | 1.450 × 10⁻⁴ |
| Pressure (kPa) | - | psi | 0.145 |
| Energy (J) | - | ft·lb | 0.7376 |
| Power (W) | - | hp | 1.341 × 10⁻³ |

### Common Conversions (BG to SI Units)

| Parameter | From BG | To SI | Multiply by |
|-----------|---------|-------|------------|
| Length (ft) | - | m | 3.048 × 10⁻¹ |
| Mass (slug) | - | kg | 1.459 × 10¹ |
| Density (slug/ft³) | - | kg/m³ | 5.154 × 10² |
| Pressure (psi) | - | Pa | 6.895 × 10³ |
| Energy (Btu) | - | J | 1.055 × 10³ |
| Power (hp) | - | W | 7.457 × 10² |

---

## 2. FLUID PROPERTIES

### Fundamental Definitions

\(\rho = \frac{m}{V}\)
**Density** - mass per unit volume [kg/m³]

\(\gamma = \rho g\)
**Specific Weight** - weight per unit volume [N/m³]

\(SG = \frac{\rho}{\rho_{water@4°C}} = \frac{\gamma}{\gamma_{water}}\)
**Specific Gravity** - ratio of fluid density to water density (dimensionless)

\(v = \frac{1}{\rho} = \frac{V}{m}\)
**Specific Volume** - volume per unit mass [m³/kg]

### Viscosity

\(\tau = \mu \frac{du}{dy}\)
**Newtonian Shear Stress** - stress due to velocity gradient [Pa·s or N·s/m²]

| Symbol | Property | Units |
|--------|----------|-------|
| μ (mu) | Dynamic (absolute) viscosity | Pa·s or N·s/m² |
| ν (nu) | Kinematic viscosity | m²/s (ν = μ/ρ) |

**Standard Values (Water @ 20°C)**:
- Dynamic viscosity: μ ≈ 0.001 Pa·s
- Kinematic viscosity: ν ≈ 1.0 × 10⁻⁶ m²/s

### Ideal Gas Law

\(pv = RT\)
**Equation of State** - where R is specific gas constant

\(p = \rho RT\)
**Alternative form** - pressure in terms of density

**Common Gas Constants** (J/(kg·K)):
- Air: R = 287 J/(kg·K) = 0.287 kJ/(kg·K)
- Carbon Dioxide (CO₂): R = 189 J/(kg·K) = 0.189 kJ/(kg·K)
- Methane (CH₄): R ≈ 519 J/(kg·K) = 0.519 kJ/(kg·K)
- Nitrogen (N₂): R ≈ 297 J/(kg·K) = 0.297 kJ/(kg·K)

---

## 3. FLUID STATICS

### Hydrostatic Pressure

\(p = p_0 + \rho g(z_0 - z) = p_0 + \gamma h\)
**Hydrostatic Pressure Distribution** - for incompressible fluid

**Note**: Pressure increases linearly with depth. At same horizontal level, pressure is identical.

### Pressure Types

\(p_{abs} = p_{gage} + p_{atm}\)
**Absolute Pressure** - measured from vacuum [Pa (absolute)]

**Standard Atmospheric Pressure**:
- p_atm = 101.325 kPa = 1 bar = 14.696 psia

### Hydrostatic Force on Plane Surface

\(F_R = p_c A = \rho g h_c A\)
**Resultant Hydrostatic Force** - acts at center of pressure

\(h_{cp} = h_c + \frac{I_G}{h_c A}\)
**Center of Pressure Depth** - distance from surface to force application point

where:
- h_c = depth of centroid [m]
- I_G = second moment of area about centroid [m⁴]
- A = area of surface [m²]

### Manometers

**Simple Manometer** (U-tube with one leg exposed to atmosphere):
\(\Delta p = \rho_{fluid} g h\)

**Differential Manometer** (comparing two pressures):
\(p_1 - p_2 = \rho_{manometer fluid} g h_{difference}\)

**Inclined Manometer**: For small pressure differences, use low-density fluid and incline tube at shallow angle for more readable scale.

---

## 4. FLUID DYNAMICS – BERNOULLI & CONTINUITY

### Mass Flow Rate

\(\dot{m} = \rho A V\)
**Mass Flow Rate** - [kg/s]

### Continuity Equation (Incompressible Flow)

\(A_1 V_1 = A_2 V_2\)
**1D Steady Flow** - volume flow rate is constant

\(\sum \dot{m}_{in} = \sum \dot{m}_{out}\)
**General form** - mass conservation

### Bernoulli Equation (No Losses, No Pump/Turbine)

\(\frac{p_1}{\rho g} + \frac{V_1^2}{2g} + z_1 = \frac{p_2}{\rho g} + \frac{V_2^2}{2g} + z_2\)
**Energy Form** - in terms of energy per unit weight [J/N or m]

**Alternative Form** (energy per unit mass):
\(p_1 + \frac{1}{2}\rho V_1^2 + \rho g z_1 = p_2 + \frac{1}{2}\rho V_2^2 + \rho g z_2\)

**Bernoulli with Pump/Turbine and Losses**:
\(\frac{p_1}{\rho g} + \frac{V_1^2}{2g} + z_1 + h_p = \frac{p_2}{\rho g} + \frac{V_2^2}{2g} + z_2 + h_t + h_L\)

where:
- h_p = pump head [m]
- h_t = turbine head [m]
- h_L = head loss [m]

### Energy and Hydraulic Grade Lines

\(z_{EL} = \frac{p}{\rho g} + \frac{V^2}{2g} + z\)
**Energy Line (EL) Elevation** - total mechanical energy per unit weight

\(z_{HGL} = \frac{p}{\rho g} + z\)
**Hydraulic Grade Line (HGL) Elevation** - one velocity head below EL

### Key Bernoulli Applications

**Pitot Tube** (measures stagnation pressure):
\(p_{stag} = p + \frac{1}{2}\rho V^2\)

**Venturi Meter** (measures flow rate):
Uses continuity + Bernoulli with geometry constraints

---

## 5. CONTROL VOLUMES & MASS CONSERVATION

### General Mass Conservation

\(\frac{d}{dt}\int_{CV} \rho \, dV = \sum \dot{m}_{in} - \sum \dot{m}_{out}\)
**Unsteady Flow** - mass accumulation in control volume

**Steady Flow**:
\(\sum \dot{m}_{in} = \sum \dot{m}_{out}\)

### Momentum Equation (Control Volume)

\(\sum \vec{F} = \frac{d}{dt}\int_{CV} \rho \vec{V} \, dV + \sum \dot{m}_{out}\vec{V}_{out} - \sum \dot{m}_{in}\vec{V}_{in}\)
**General momentum balance** (vector equation)

---

## 6. THERMODYNAMIC FIRST LAW

### First Law - Closed System

\(\Delta E = Q - W\)
**Energy Balance** - change in total energy [kJ]

\(\Delta E = \Delta U + \Delta KE + \Delta PE\)
**Total Energy Change**:

\(\Delta PE = mg(z_2 - z_1)\)
**Potential Energy Change** [J or kJ]

\(\Delta KE = \frac{m}{2}(V_2^2 - V_1^2)\)
**Kinetic Energy Change** [J or kJ]

### Sign Convention
- **Q > 0**: Heat transfer INTO system
- **W > 0**: Work done BY system
- **ΔE > 0**: Energy increase in system

### Differential Form

\(\delta Q - \delta W = dE\)

---

## 7. CLOSED SYSTEM PROCESSES

### General Boundary Work

\(W = \int p \, dV\)
**Total Work** - work at boundary

### Polytropic Process

\(pv^n = \text{constant} = C\)
**Polytropic Relation** - for ideal gas

\(W_{1→2} = \frac{p_2 v_2 - p_1 v_1}{1 - n}\)
**Polytropic Work** (n ≠ 1) [kJ/kg]

**Special Cases**:
| Process | n | Relation | W = |
|---------|---|----------|-----|
| Isothermal | 1 | T = const | p(V₂ - V₁) or mRT ln(V₂/V₁) |
| Isobaric (const p) | 0 | p = const | p(V₂ - V₁) |
| Isochoric (const V) | ∞ | V = const | 0 |
| Adiabatic | k | pVᵏ = const | (p₂V₂ - p₁V₁)/(1-k) |

### Temperature-Pressure Relation (Ideal Gas)

\(\frac{T_2}{T_1} = \left(\frac{p_2}{p_1}\right)^{\frac{n-1}{n}}\)
**T-p relation in polytropic process**

\(\frac{T_2}{T_1} = \left(\frac{V_1}{V_2}\right)^{n-1}\)
**T-v relation in polytropic process**

---

## 8. PURE SUBSTANCES & PHASE PROPERTIES

### Two-Phase Region (Saturated Liquid-Vapor Mixture)

**Quality (Dryness Fraction)**:
\(x = \frac{v - v_f}{v_g - v_f} = \frac{m_{vapor}}{m_{total}}\)
**Quality** - mass fraction of vapor (0 ≤ x ≤ 1) [dimensionless]

### Property Relations in Two-Phase Region

\(u = u_f + x(u_g - u_f) = u_f + xu_{fg}\)
**Specific Internal Energy**

\(h = h_f + x(h_g - h_f) = h_f + xh_{fg}\)
**Specific Enthalpy**

\(s = s_f + x(s_g - s_f) = s_f + xs_{fg}\)
**Specific Entropy**

where subscripts:
- f = saturated liquid
- g = saturated vapor
- fg = g - f (difference)

### State Location Determination

1. **Single-phase identification**:
   - If T_sat < T: superheated vapor
   - If T_sat > T: compressed (subcooled) liquid
   - If T = T_sat and 0 < x < 1: two-phase mixture

2. **From tables**:
   - Use saturation tables for two-phase
   - Use superheated tables for superheated vapor
   - Use compressed liquid tables for compressed liquid

---

## 9. IDEAL GASES

### Ideal Gas Relations

\(pv = RT\)
**Equation of State** [J/(kg·K)]

\(u_2 - u_1 = c_v(T_2 - T_1)\)
**Internal Energy Change** - for ideal gas with constant c_v

\(h_2 - h_1 = c_p(T_2 - T_1)\)
**Enthalpy Change** - for ideal gas with constant c_p

### Specific Heat Relations

\(c_p - c_v = R\)
**Mayer's Relation**

\(k = \frac{c_p}{c_v}\)
**Specific Heat Ratio** (dimensionless)

**Typical Values** (Air):
- c_p ≈ 1.005 kJ/(kg·K)
- c_v ≈ 0.718 kJ/(kg·K)
- k ≈ 1.40

### Polytropic Process for Ideal Gas

\(T_2 = T_1 \left(\frac{p_2}{p_1}\right)^{\frac{n-1}{n}}\)
**Temperature Ratio**

\(W = \frac{mR(T_2 - T_1)}{1-n}\)
**Polytropic Work** - for ideal gas [kJ]

### Adiabatic Process (Ideal Gas)

\(pV^k = \text{constant}\)
**Adiabatic Relation**

\(TV^{k-1} = \text{constant}\)
**Alternative form**

\(Q = 0\) (no heat transfer)

---

## 10. STEADY-FLOW ENERGY EQUATION

### General Energy Balance

\(\dot{Q} - \dot{W} = \dot{m}\left[(h_2 - h_1) + \frac{V_2^2 - V_1^2}{2} + g(z_2 - z_1)\right]\)
**Steady-Flow First Law** - per unit time [kW]

where:
- \(\dot{Q}\) = heat transfer rate [kW]
- \(\dot{W}\) = shaft power [kW]
- h = specific enthalpy [kJ/kg]
- V = velocity [m/s]
- z = elevation [m]

### Special Devices

**Nozzle/Diffuser** (adiabatic, no W, ΔPE ≈ 0):
\(h_1 + \frac{V_1^2}{2} = h_2 + \frac{V_2^2}{2}\)

**Turbine** (adiabatic, no PE change):
\(\dot{W} = \dot{m}(h_1 - h_2)\)

**Compressor** (adiabatic, no PE change):
\(\dot{W} = \dot{m}(h_2 - h_1)\)

**Pump** (adiabatic, no PE change):
\(\dot{W} = \dot{m}(h_2 - h_1)\)

**Mixer** (adiabatic mixing, no W):
\(\sum(\dot{m}_{in}h_{in}) = \dot{m}_{out}h_{out}\)

**Throttle Valve** (adiabatic, no W, KE/PE change):
\(h_1 = h_2\)

### Mass Flow Rate for Ideal Gas

\(\dot{m} = \rho AV = \frac{pAV}{RT}\)
**Mass Flow Rate through area A** [kg/s]

---

## 11. COMMON SYMBOL REFERENCE

### Symbols & Standard Units (SI)

| Symbol | Property | Units |
|--------|----------|-------|
| m | mass | kg |
| V | volume | m³ |
| v | specific volume | m³/kg |
| ρ | density | kg/m³ |
| γ | specific weight | N/m³ |
| SG | specific gravity | – |
| p | pressure (gage) | Pa |
| p_abs | absolute pressure | Pa |
| T | temperature | K |
| R | gas constant | J/(kg·K) |
| τ | shear stress | Pa |
| μ | dynamic viscosity | Pa·s |
| ν | kinematic viscosity | m²/s |
| A | area | m² |
| z | elevation | m |
| g | gravity | m/s² |
| V | flow velocity | m/s |
| F_R | resultant force | N |
| h_c | centroid depth | m |
| h_cp | center-of-pressure depth | m |
| I_G | second moment of area | m⁴ |
| Q | heat transfer (total) | kJ |
| Ė | heat transfer rate | kW |
| W | work (total) | kJ |
| Ẇ | power (rate of work) | kW |
| E | total energy | kJ |
| U | internal energy | kJ |
| u | specific internal energy | kJ/kg |
| H | enthalpy | kJ |
| h | specific enthalpy | kJ/kg |
| KE | kinetic energy | kJ |
| PE | potential energy | kJ |
| x | quality (vapor fraction) | – |
| η_th | thermal efficiency | – |
| c_p | specific heat @ const p | kJ/(kg·K) |
| c_v | specific heat @ const v | kJ/(kg·K) |
| k | specific heat ratio (γ) | – |
| ṁ | mass flow rate | kg/s |
| h_p | pump head | m |
| h_t | turbine head | m |
| h_L | head loss | m |
| n | polytropic exponent | – |

---

## ADDITIONAL NOTES

### Thermodynamic Property Tables
- **Saturation Properties**: Use for two-phase (liquid-vapor) regions
- **Superheated Properties**: Use when T > T_sat at given pressure
- **Compressed Liquid**: Often approximated as saturated liquid at T

### Process Identification
- **Constant pressure (isobaric)**: pV diagram shows horizontal line
- **Constant volume (isochoric)**: pV diagram shows vertical line
- **Constant temperature (isothermal)**: pV diagram shows hyperbola
- **Adiabatic**: No heat transfer (Q = 0)
- **Polytropic**: pVⁿ = constant

### Common Exam Topics
1. Bernoulli equation applications
2. Continuity and mass balance
3. Hydrostatic force calculations
4. Throttling calorimeter (h₁ = h₂)
5. Polytropic processes with ideal gases
6. Steady-flow energy balance
7. Two-phase property calculations
8. Compressor/turbine power calculations

---

**Last Updated**: December 2025 | Based on MEC511 Course Materials and Textbooks