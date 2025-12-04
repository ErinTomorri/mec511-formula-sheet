# MEC 511: ADVANCED FORMULA SHEET WITH PROBLEM SOLVING STRATEGIES

**Course**: MEC 511 - Thermodynamics & Fluids (TMU)  
**Textbooks**: Young et al., Moran et al.  
**Version**: Enhanced with Theory, Variables, and Solution Strategies

---

## TABLE OF CONTENTS
1. [Unit Systems & Conversions](#1-unit-systems--conversions)
2. [Fluid Properties & Definitions](#2-fluid-properties--definitions)
3. [Fluid Statics](#3-fluid-statics)
4. [Fluid Dynamics - Bernoulli & Continuity](#4-fluid-dynamics--bernoulli--continuity)
5. [Control Volumes & Mass Conservation](#5-control-volumes--mass-conservation)
6. [First Law of Thermodynamics](#6-first-law-of-thermodynamics)
7. [Closed System Processes](#7-closed-system-processes)
8. [Pure Substances & Phase Properties](#8-pure-substances--phase-properties)
9. [Ideal Gases](#9-ideal-gases)
10. [Steady-Flow Energy Equation](#10-steady-flow-energy-equation)
11. [Problem-Solving Strategies](#11-problem-solving-strategies-by-topic)
12. [Reference Tables & Constants](#12-reference-tables--constants)

---

## 1. UNIT SYSTEMS & CONVERSIONS

### 1.1 MLT vs FLT Systems

**MLT System** (Mass-Length-Time):
- Primary variables: m (mass), L (length), t (time)
- Force derived: F = ma [kg·m/s² = N]
- Used in SI units

**FLT System** (Force-Length-Time):
- Primary variables: F (force), L (length), t (time)
- Mass derived: m = F/a [lb·s²/ft = slug]
- Used in British Gravitational units

| Quantity | MLT | FLT | SI (Preferred) |
|----------|-----|-----|----------------|
| Mass | M | F·T²/L | kg |
| Force | M·L/T² | F | N (newton) |
| Pressure | M·L⁻¹·T⁻² | F/L² | Pa (N/m²) |
| Energy | M·L²·T⁻² | F·L | J (N·m) |
| Power | M·L²·T⁻³ | F·L/T | W (J/s) |

### 1.2 SI to British Gravitational (BG) Conversions

| Parameter | SI Unit | BG Unit | Conversion Factor |
|-----------|---------|---------|-------------------|
| Length | m | ft | ×3.281 or ÷0.3048 |
| Mass | kg | slug | ÷14.59 |
| Density | kg/m³ | slug/ft³ | ÷515.4 |
| Pressure | Pa | psi | ÷6894.76 |
| Pressure | kPa | psi | ÷6.895 |
| Energy | J | ft·lbf | ÷1.356 |
| Power | W | hp | ÷745.7 |
| Viscosity (dyn) | Pa·s | lbf·s/ft² | ÷47.88 |

### 1.3 Standard Atmospheric Conditions

\(p_{atm} = 101.325 \text{ kPa} = 1 \text{ bar} = 14.696 \text{ psia}\)

\(g = 9.81 \text{ m/s}^2 \text{ (standard gravity)}\)

\(\rho_{water,4°C} = 1000 \text{ kg/m}^3\)

---

## 2. FLUID PROPERTIES & DEFINITIONS

### 2.1 Fundamental Fluid Properties

**Density** \((\rho)\) - mass per unit volume:
\[\rho = \frac{m}{V}\]
- Units: kg/m³ (SI) or slug/ft³ (BG)
- Water @ 20°C: ρ ≈ 998 kg/m³
- Air @ 20°C, 1 atm: ρ ≈ 1.20 kg/m³

**Specific Weight** \((\gamma)\) - weight per unit volume (gravitational):
\[\gamma = \rho g = \frac{W}{V}\]
- Units: N/m³ (SI) or lbf/ft³ (BG)
- Water: γ ≈ 9.81 kN/m³
- Related: \(\gamma = \frac{mg}{V} = \rho g\)

**Specific Gravity** \((SG)\) - dimensionless density ratio:
\[SG = \frac{\rho_{fluid}}{\rho_{water,4°C}} = \frac{\gamma_{fluid}}{\gamma_{water}}\]
- Dimensionless (no units)
- SG = 1 for water, SG > 1 for denser fluids, SG < 1 for lighter fluids
- Use at 4°C (water at maximum density) as reference

**Specific Volume** \((v)\) - inverse of density:
\[v = \frac{1}{\rho} = \frac{V}{m}\]
- Units: m³/kg (SI)
- Also called **molar volume** when per mole

**Viscosity** - fluid resistance to shear deformation

*Dynamic (Absolute) Viscosity* \((\mu)\):
\[\tau = \mu \frac{du}{dy}\]
- **Shear Stress**: \(\tau = \frac{F_{shear}}{A}\) [Pa or N/m²]
- **Velocity Gradient**: \(\frac{du}{dy}\) [s⁻¹]
- Units: Pa·s = N·s/m² (SI) or lbf·s/ft² (BG)
- Water @ 20°C: μ ≈ 0.001 Pa·s
- Air @ 20°C: μ ≈ 1.81 × 10⁻⁵ Pa·s

*Kinematic Viscosity* \((\nu)\):
\[\nu = \frac{\mu}{\rho}\]
- Units: m²/s (SI) or ft²/s (BG)
- Water @ 20°C: ν ≈ 1.0 × 10⁻⁶ m²/s (1 cSt)

**Bulk Modulus** \((K)\) - compressibility:
\[K = -\frac{dp}{dV/V} = -V\frac{dp}{dV}\]
- Units: Pa
- Water: K ≈ 2.2 GPa (incompressible assumption valid)
- Air: K ≈ 101 kPa (compressible)

### 2.2 Ideal Gas Law & Gas Constants

**Equation of State** (specific form):
\[pv = RT\]
- p = absolute pressure [Pa]
- v = specific volume [m³/kg]
- R = specific gas constant [J/(kg·K)]
- T = absolute temperature [K]

**Alternative forms**:
\[p = \rho RT \quad \text{or} \quad pV = mRT\]

**Common Gas Constants** \(R = \frac{R_{universal}}{M}\):
- Air: R = 287 J/(kg·K) = 0.287 kJ/(kg·K)
- Nitrogen (N₂): R ≈ 297 J/(kg·K)
- Oxygen (O₂): R ≈ 260 J/(kg·K)
- Carbon Dioxide (CO₂): R = 189 J/(kg·K)
- Methane (CH₄): R ≈ 519 J/(kg·K)
- Water Vapor (H₂O): R ≈ 462 J/(kg·K)

**Universal Gas Constant**:
\(R_{universal} = 8.314 \text{ J/(mol·K)}\)

---

## 3. FLUID STATICS

### 3.1 Hydrostatic Pressure Distribution

**Pressure Variation with Depth** (incompressible fluid):
\[p(z) = p_0 + \rho g(z_0 - z) = p_0 + \gamma h\]

where:
- p₀ = reference pressure at depth z₀
- h = vertical distance from reference (positive downward)
- Pressure increases linearly with depth
- **Key principle**: At the same elevation, pressure is identical in a static fluid

**Pressure Types & Relationships**:
- **Absolute Pressure** \(p_{abs}\): measured from perfect vacuum (0 Pa)
- **Gage Pressure** \(p_{gage}\): measured from atmospheric pressure
- **Atmospheric Pressure** \(p_{atm}\): local pressure of atmosphere

\[p_{abs} = p_{gage} + p_{atm}\]

**Standard Values**:
- Atmospheric: p_atm = 101.325 kPa = 1 bar
- Gauge pressure of 0 implies absolute = atmospheric
- Negative gage pressure = vacuum (suction)

### 3.2 Manometer Analysis

**Simple Manometer** (one end open to atmosphere):
\[\Delta p = p_{inside} - p_{atm} = \rho_{fluid} \cdot g \cdot h\]

where h = height difference of fluid columns [m]

**Differential Manometer** (comparing two pressures):
\[p_1 - p_2 = \rho_{manometer} \cdot g \cdot \Delta h\]

where Δh = height difference between two arms

**Inclined Manometer** (for small pressure differences):
- Increases sensitivity by using shallow angle θ
- True vertical height: \(h = L \sin(\theta)\) where L = incline length
- Readability: \(\Delta h_{incline} = \frac{\Delta h}{\sin(\theta)}\)
- Use low-density gauge fluids (alcohol, oil) for finer measurement

### 3.3 Hydrostatic Force on Submerged Surfaces

**Resultant Hydrostatic Force** (plane surface):
\[F_R = p_c \cdot A = \rho g h_c A\]

where:
- \(F_R\) = total hydrostatic force [N]
- \(p_c\) = pressure at centroid of area [Pa]
- \(h_c\) = depth of centroid below free surface [m]
- A = surface area [m²]

**Center of Pressure** (point where F_R acts):
\[h_{cp} = h_c + \frac{I_G}{h_c A}\]

where:
- \(h_{cp}\) = depth of center of pressure [m]
- \(I_G\) = second moment of area about centroid [m⁴]
- A = surface area [m²]

**Key insight**: Center of pressure ALWAYS acts BELOW centroid due to increasing pressure with depth.

**Second Moments of Area** (common shapes):
- Rectangular: \(I_G = \frac{bh^3}{12}\) (width × height about centroid)
- Circular: \(I_G = \frac{\pi D^4}{64}\)
- Triangle: \(I_G = \frac{bh^3}{36}\)

---

## 4. FLUID DYNAMICS – BERNOULLI & CONTINUITY

### 4.1 Mass & Volume Flow Rate

**Mass Flow Rate**:
\[\dot{m} = \rho A V\]
- Units: kg/s
- ṁ = mass per unit time through section A
- For compressible flow: check density at each section

**Volumetric Flow Rate**:
\[Q = A V = \frac{\dot{m}}{\rho}\]
- Units: m³/s
- Constant for incompressible flow along a streamline

### 4.2 Continuity Equation

**Steady Flow** (incompressible, 1D):
\[A_1 V_1 = A_2 V_2 = Q = \text{constant}\]

**General Form** (any control volume):
\[\sum \dot{m}_{in} = \sum \dot{m}_{out}\]

**Solution approach**:
1. Identify inlet and outlet sections
2. Write mass balance: \(\dot{m}_{in} = \dot{m}_{out}\)
3. For incompressible: use continuity on volume flow rate
4. For compressible: account for density changes

### 4.3 Bernoulli Equation (Energy Conservation)

**Form 1** - Energy per unit weight [J/N or m]:
\[\frac{p_1}{\rho g} + \frac{V_1^2}{2g} + z_1 = \frac{p_2}{\rho g} + \frac{V_2^2}{2g} + z_2 + h_L\]

**Form 2** - Energy per unit mass [J/kg]:
\[\frac{p_1}{\rho} + \frac{V_1^2}{2} + gz_1 = \frac{p_2}{\rho} + \frac{V_2^2}{2} + gz_2 + h_L g\]

**Components**:
- \(\frac{p}{\rho g}\) = pressure head [m]
- \(\frac{V^2}{2g}\) = velocity head [m]
- z = elevation head [m]
- \(h_L\) = head loss [m] (friction, bends, etc.)

**Assumptions**:
- Incompressible flow
- Steady flow
- No shaft work (pump/turbine)
- No heat transfer
- Frictionless (unless h_L specified)

**With Pump/Turbine**:
\[\frac{p_1}{\rho g} + \frac{V_1^2}{2g} + z_1 + h_p = \frac{p_2}{\rho g} + \frac{V_2^2}{2g} + z_2 + h_t + h_L\]

where:
- \(h_p\) = pump head (adds energy) [m]
- \(h_t\) = turbine head (removes energy) [m]

### 4.4 Energy & Hydraulic Grade Lines

**Total Energy Line** (EL):
\[z_{EL} = \frac{p}{\rho g} + \frac{V^2}{2g} + z\]
- Represents total mechanical energy per unit weight
- Horizontal for frictionless flow (no losses)
- Decreases with friction losses

**Hydraulic Grade Line** (HGL):
\[z_{HGL} = \frac{p}{\rho g} + z\]
- One velocity head below EL
- Shows piezometric head
- Where pressure changes occur
- Indicates if flow is possible (must be above pipe in siphon)

**Key relationships**:
- Distance from pipe to HGL = pressure head available
- Distance between EL and HGL = velocity head
- HGL drops in direction of flow (friction)

### 4.5 Applications

**Pitot Tube** (velocity measurement):
\[p_{stag} = p_{static} + \frac{1}{2}\rho V^2\]
- Stagnation (total) pressure: \(p_{stag}\)
- Static pressure: p_static
- Velocity: \(V = \sqrt{\frac{2(p_{stag} - p_{static})}{\rho}}\)

**Venturi Meter** (flow rate measurement):
- Uses continuity + Bernoulli
- Pressure difference measured between throat and entrance
- Flow rate: \(\dot{m} = C_d A \sqrt{\frac{2(p_1-p_2)}{\rho(1-(A_2/A_1)^2)}}\)

**Orifice Plate**: Similar principle with discharge coefficient

---

## 5. CONTROL VOLUMES & MASS CONSERVATION

### 5.1 General Mass Conservation

**Unsteady Flow** (mass accumulating):
\[\frac{d}{dt}\int_{CV} \rho \, dV = \sum \dot{m}_{in} - \sum \dot{m}_{out}\]

**Rate of mass accumulation** in control volume:
\[\frac{dm_{CV}}{dt} = \sum \dot{m}_{in} - \sum \dot{m}_{out}\]

**Steady Flow** (no accumulation):
\[\sum \dot{m}_{in} = \sum \dot{m}_{out}\]

### 5.2 Solution Strategy for Control Volume Problems

1. **Define the control volume** (fixed region in space)
2. **Identify inlet(s)** and **outlet(s)**
3. **List known quantities** at each section: p, T, V, A, ρ, h, etc.
4. **Write mass balance**: \(\dot{m} = \rho AV\)
5. **For unsteady**: Track accumulation: \(\frac{dm}{dt} = \rho AV - \rho AV_{out}\)

---

## 6. FIRST LAW OF THERMODYNAMICS

### 6.1 Closed System (Fixed Mass)

**First Law** (energy balance):
\[\Delta E = Q - W\]

where:
- ΔE = change in total energy [kJ]
- Q = heat transfer TO system [kJ] (positive in)
- W = work done BY system [kJ] (positive out)

**Total Energy**:
\[E = U + KE + PE\]
\[\Delta E = \Delta U + \Delta KE + \Delta PE\]

**Changes in energy components**:
\[\Delta U = m \cdot c_v \cdot \Delta T \quad \text{(internal energy)}\]
\[\Delta KE = \frac{m}{2}(V_2^2 - V_1^2) \quad \text{(kinetic energy)}\]
\[\Delta PE = m \cdot g \cdot (z_2 - z_1) \quad \text{(potential energy)}\]

### 6.2 Sign Convention

- **Q > 0**: Heat flows INTO system (absorption)
- **Q < 0**: Heat flows OUT OF system (rejection)
- **W > 0**: Work done BY system (expansion, turbine)
- **W < 0**: Work done ON system (compression, pump)
- **ΔE > 0**: System energy increases
- **ΔE < 0**: System energy decreases

### 6.3 Differential Form

For infinitesimal processes:
\[\delta Q - \delta W = dE\]

Note: Q and W are path functions (not state properties)

---

## 7. CLOSED SYSTEM PROCESSES

### 7.1 General Boundary Work

**Boundary Work** (pressure-volume work):
\[W = \int p \, dV\]

For any closed system undergoing volume change:
- Work is positive when system expands (V increases)
- Work is negative when system compresses (V decreases)

### 7.2 Polytropic Process

**Polytropic Relationship**:
\[pv^n = C = \text{constant}\]

or equivalently:
\[p_1v_1^n = p_2v_2^n\]

where:
- n = polytropic exponent (determines process type)
- Polytropic exponent depends on heat transfer during process

**Polytropic Work** (n ≠ 1):
\[W = \frac{p_2v_2 - p_1v_1}{1-n} \quad \text{[kJ/kg]}\]

**For total system** (n ≠ 1):
\[W = \frac{m(p_2v_2 - p_1v_1)}{1-n} = \frac{mR(T_2-T_1)}{1-n}\]

**Process Classification**:
| Process | n Value | Relation | Work Formula | Heat |
|---------|---------|----------|--------------|------|
| Isobaric (const p) | 0 | p = const | W = p(V₂-V₁) | Q = mc_p(T₂-T₁) |
| Isothermal (const T) | 1 | T = const | W = mRT ln(v₂/v₁) | Q = W |
| Adiabatic (Q=0) | k | pVᵏ = const | W = (p₂V₂-p₁V₁)/(1-k) | Q = 0 |
| Isochoric (const V) | ∞ | V = const | W = 0 | Q = mc_v(T₂-T₁) |

### 7.3 Polytropic Process Relations for Ideal Gas

**Temperature-Pressure Relation**:
\[\frac{T_2}{T_1} = \left(\frac{p_2}{p_1}\right)^{\frac{n-1}{n}}\]

**Temperature-Volume Relation**:
\[\frac{T_2}{T_1} = \left(\frac{V_1}{V_2}\right)^{n-1}\]

**Pressure-Volume Relation** (already stated):
\[\frac{p_2}{p_1} = \left(\frac{V_1}{V_2}\right)^n\]

### 7.4 Adiabatic Process (Special Case, Q = 0)

**No heat transfer**: \(\delta Q = 0\)

**For ideal gas**:
\[pV^k = \text{constant}\]

where \(k = \frac{c_p}{c_v} = \gamma\) = specific heat ratio

**Relations**:
\[T_2 = T_1 \left(\frac{p_2}{p_1}\right)^{\frac{k-1}{k}} = T_1 \left(\frac{V_1}{V_2}\right)^{k-1}\]

**Work done**:
\[W = \frac{mR(T_2-T_1)}{1-k} = \frac{p_2V_2 - p_1V_1}{1-k}\]

**Internal energy change** = work done (since Q = 0):
\[\Delta U = -W \quad \text{(for adiabatic)}\]

---

## 8. PURE SUBSTANCES & PHASE PROPERTIES

### 8.1 Two-Phase Region (Liquid-Vapor Mixture)

**Quality** (dryness fraction) - mass fraction of vapor:
\[x = \frac{m_v}{m_{total}} = \frac{m_v}{m_f + m_v}\]

Range: 0 ≤ x ≤ 1
- x = 0: saturated liquid (100% liquid, 0% vapor)
- x = 1: saturated vapor (0% liquid, 100% vapor)
- 0 < x < 1: two-phase mixture

### 8.2 Property Relations in Two-Phase Region

**Specific Volume**:
\[v = v_f + x(v_g - v_f) = v_f + xv_{fg}\]

**Specific Internal Energy**:
\[u = u_f + x(u_g - u_f) = u_f + xu_{fg}\]

**Specific Enthalpy**:
\[h = h_f + x(h_g - h_f) = h_f + xh_{fg}\]

**Specific Entropy**:
\[s = s_f + x(s_g - s_f) = s_f + xs_{fg}\]

where subscripts:
- f = saturated liquid properties
- g = saturated vapor properties
- fg = difference (g - f)

### 8.3 Calculating Quality from Two-Phase Properties

If you know two independent properties (p and v, or T and h, etc.):

**From specific volume**:
\[x = \frac{v - v_f}{v_g - v_f}\]

**From specific enthalpy**:
\[x = \frac{h - h_f}{h_{fg}}\]

**From specific internal energy**:
\[x = \frac{u - u_f}{u_{fg}}\]

### 8.4 State Identification Process

**Step 1**: Given two independent properties (p, T) or (p, h) etc.

**Step 2**: Determine saturation conditions
- If T given with p: compare T_sat @ given p
- If p given with T: compare p_sat @ given T

**Step 3**: Classify state:
- If T > T_sat (at given p): **SUPERHEATED VAPOR**
- If T < T_sat (at given p): **COMPRESSED (SUBCOOLED) LIQUID**
- If T = T_sat (at given p) AND 0 < x < 1: **TWO-PHASE MIXTURE**
- If T = T_sat (at given p) AND x = 0: **SATURATED LIQUID**
- If T = T_sat (at given p) AND x = 1: **SATURATED VAPOR**

**Step 4**: Use appropriate tables
- Saturation tables → for two-phase, or T_sat, p_sat lookup
- Superheated tables → for superheated vapor
- Compressed liquid tables → for compressed liquid (or approximate as saturated liquid)

---

## 9. IDEAL GASES

### 9.1 Ideal Gas Equation of State

**Specific Form** (most useful for engineering):
\[pv = RT\]

**Molar Form**:
\[pV = nR_{universal}T\]

**Mass Form**:
\[pV = mRT\]

where:
- R = specific gas constant [J/(kg·K)]
- T = absolute temperature [K]

### 9.2 Internal Energy & Enthalpy

**Specific Internal Energy** (ideal gas):
\[u_2 - u_1 = c_v(T_2 - T_1)\]

Note: Internal energy depends ONLY on temperature

**Specific Enthalpy** (ideal gas):
\[h_2 - h_1 = c_p(T_2 - T_1)\]

Note: Enthalpy depends ONLY on temperature

### 9.3 Specific Heat Relations

**Mayer's Relation**:
\[c_p - c_v = R\]

**Specific Heat Ratio**:
\[k = \gamma = \frac{c_p}{c_v}\]

**Typical Values** (Air at 20°C):
- \(c_p\) = 1.005 kJ/(kg·K)
- \(c_v\) = 0.718 kJ/(kg·K)
- k = 1.40
- R = 0.287 kJ/(kg·K)

**Other Gases**:
- Diatomic gases (N₂, O₂, air): k ≈ 1.40
- Monatomic gases (He, Ar): k ≈ 1.67
- Polyatomic gases (CO₂, H₂O): k ≈ 1.30

### 9.4 Polytropic Process for Ideal Gas

**Work in polytropic process**:
\[W = \frac{mR(T_2 - T_1)}{1-n}\]

**Adiabatic process** (n = k):
\[T_2 = T_1 \left(\frac{p_2}{p_1}\right)^{\frac{k-1}{k}}\]

---

## 10. STEADY-FLOW ENERGY EQUATION

### 10.1 General Energy Balance (Control Volume)

**Steady-Flow First Law**:
\[\dot{Q} - \dot{W}_s = \dot{m}\left[(h_2-h_1) + \frac{V_2^2-V_1^2}{2} + g(z_2-z_1)\right]\]

**With multiple inlets/outlets**:
\[\dot{Q} - \dot{W}_s = \sum_{\text{out}}\dot{m}(h + \frac{V^2}{2} + gz) - \sum_{\text{in}}\dot{m}(h + \frac{V^2}{2} + gz)\]

where:
- \(\dot{Q}\) = rate of heat transfer [kW] (positive in)
- \(\dot{W}_s\) = shaft power [kW] (positive out)
- \(\dot{m}\) = mass flow rate [kg/s]
- h = specific enthalpy [kJ/kg]
- V = velocity [m/s]
- z = elevation [m]
- g = gravity [m/s²]

### 10.2 Standard Devices (Adiabatic, Neglect PE)

**Nozzle** (accelerates flow):
\[h_1 + \frac{V_1^2}{2} = h_2 + \frac{V_2^2}{2}\]

Assumes: no Q̇, no Ẇ_s, Δz ≈ 0

**Diffuser** (decelerates flow):
\[h_1 + \frac{V_1^2}{2} = h_2 + \frac{V_2^2}{2}\]

Same as nozzle equation

**Turbine** (extracts work):
\[\dot{W}_s = \dot{m}(h_1 - h_2)\]

Assumes: adiabatic, negligible KE/PE changes
- Typically W_s > 0 (work output)

**Compressor** (requires work input):
\[\dot{W}_s = \dot{m}(h_2 - h_1)\]

Assumes: adiabatic, negligible KE/PE changes
- Typically W_s < 0 (work input required)

**Pump** (incompressible):
\[\dot{W}_s = \dot{m}(h_2 - h_1) \approx \dot{m}\frac{(p_2-p_1)}{\rho}\]

For liquids (essentially incompressible):
\[h_2 - h_1 \approx \frac{p_2-p_1}{\rho}\]

**Throttle Valve** (isenthalpic):
\[h_1 = h_2\]

No shaft work, adiabatic, negligible KE/PE
- Used to measure quality (throttling calorimeter)
- Useful for pressure reduction

**Mixer/Separator** (adiabatic):
\[\sum_{\text{in}}(\dot{m}h) = \sum_{\text{out}}(\dot{m}h)\]

Multiple inlet streams combine, or one stream separates

### 10.3 Throttling Calorimeter (Quality Measurement)

**Principle**: Isenthalpic expansion through valve
\[h_1 = h_2\]

**Procedure**:
1. Two-phase steam at unknown quality x₁ and pressure p₁
2. Expand through throttle to lower pressure p₂
3. Measure temperature T₂ at exit
4. Find h₂ from superheated tables @ (p₂, T₂)
5. Since h₁ = h₂, and h₁ = h_f + x₁·h_fg @ p₁
6. Solve: \(x_1 = \frac{h_2 - h_{f1}}{h_{fg1}}\)

---

## 11. PROBLEM-SOLVING STRATEGIES BY TOPIC

### 11.1 Strategy: Bernoulli Equation Problems

**Typical scenarios**: Flow through pipes, around objects, with pressure/height changes

**General Steps**:
1. **Identify sections** (1) and (2) along streamline
2. **List knowns/unknowns**:
   - Pressures: p₁, p₂
   - Velocities: V₁, V₂
   - Elevations: z₁, z₂
3. **Check assumptions**:
   - Incompressible flow?
   - Steady state?
   - Frictionless or specify h_L?
4. **Write Bernoulli**:
   \[\frac{p_1}{\rho g} + \frac{V_1^2}{2g} + z_1 = \frac{p_2}{\rho g} + \frac{V_2^2}{2g} + z_2 + h_L\]
5. **Apply continuity** if needed:
   \[A_1V_1 = A_2V_2\]
6. **Solve** for unknown

**Common traps**:
- Forgetting to convert pressure to gage vs absolute
- Using kinematic viscosity instead of dynamic (or vice versa)
- Neglecting elevation changes
- Using incompressible assumption for compressible gases

### 11.2 Strategy: Continuity Equation Problems

**Typical scenarios**: Flow through branching pipes, varying diameter sections

**General Steps**:
1. **Define control volume** around the system
2. **Identify all inlets** and **outlets**
3. **Write mass balance**:
   - Steady: Σṁ_in = Σṁ_out
   - Unsteady: dm/dt = Σṁ_in - Σṁ_out
4. **Calculate mass flow rates**: ṁ = ρAV
5. **Account for density changes** in compressible flow
6. **Solve** for unknown (velocity, area, density, or accumulation)

**For incompressible**: Σ(AV)_in = Σ(AV)_out

### 11.3 Strategy: Hydrostatic Force Problems

**Typical scenarios**: Gates, dams, submerged plates

**General Steps**:
1. **Sketch the surface** (vertical or inclined)
2. **Identify submerged area** A and its centroid h_c
3. **Calculate centroid pressure**:
   \[p_c = \rho g h_c\]
4. **Calculate resultant force**:
   \[F_R = p_c \cdot A = \rho g h_c A\]
5. **Calculate center of pressure**:
   \[h_{cp} = h_c + \frac{I_G}{h_c A}\]
6. **Draw force diagram** showing F_R acting at h_cp

**Key insight**: Center of pressure is always BELOW centroid

### 11.4 Strategy: Polytropic Process Problems

**Typical scenarios**: Gas compression/expansion in piston-cylinder

**Given**: Usually p₁, V₁, T₁, p₂ or V₂, and polytropic exponent n

**General Steps**:
1. **Use polytropic relation**:
   \[p_1V_1^n = p_2V_2^n\]
   OR use ideal gas relations:
   \[\frac{T_2}{T_1} = \left(\frac{p_2}{p_1}\right)^{(n-1)/n}\]

2. **Find missing state variable**:
   - If T₂ unknown: \(T_2 = T_1(p_2/p_1)^{(n-1)/n}\)
   - If V₂ unknown: \(V_2 = V_1(p_1/p_2)^{1/n}\)
   - If p₂ unknown: \(p_2 = p_1(V_1/V_2)^n\)

3. **Calculate work**:
   \[W = \frac{m R(T_2-T_1)}{1-n} = \frac{p_2V_2 - p_1V_1}{1-n}\]

4. **Calculate internal energy change**:
   \[\Delta U = m c_v(T_2-T_1)\]

5. **Calculate heat transfer** from First Law:
   \[Q = \Delta U + W\]

6. **Check polytropic exponent**:
   - If Q = 0: adiabatic (n = k)
   - If Q ≠ 0: intermediate (1 < n < k)

### 11.5 Strategy: Steam Table Problems

**Typical scenarios**: Finding properties, calculating work/heat for steam

**Step 1 - Identify state**:
- Given two independent intensive properties
- Use decision tree to classify: saturated, superheated, or compressed liquid

**Step 2 - Access correct table**:
- Saturation tables (for T_sat, p_sat, properties at saturation)
- Superheated tables (for superheated vapor)
- Compressed liquid tables (rare, usually approximated)

**Step 3 - Extract properties**:
- If two-phase: use quality formula: \(x = \frac{v-v_f}{v_g-v_f}\)
- If superheated: interpolate or read directly
- If compressed liquid: use compressed liquid tables or approximate

**Step 4 - Apply thermodynamic relations**:
- For throttling: h₁ = h₂
- For adiabatic: Q = 0
- Use First Law: Q = ΔU + W

**Common properties to find**:
- Quality x (in two-phase region)
- Enthalpy h (for steady-flow devices)
- Internal energy u (for closed systems)
- Entropy s (for isentropic processes)

### 11.6 Strategy: Compressor/Turbine Problems

**Typical scenario**: Steady-flow device with known inlet/outlet conditions

**General Steps**:
1. **List all given data**:
   - Inlet: p₁, T₁, V₁, ṁ
   - Outlet: p₂, T₂, V₂
   - Heat transfer: Q̇ (if any)
   - Other: gas properties (R, cp, cv, k)

2. **For polytropic process** (if given n):
   - Find exit pressure: \(p_2 = p_1(T_2/T_1)^{n/(n-1)}\)
   - Find exit density: \(\rho_2 = p_2/(RT_2)\)
   - Find inlet density: \(\rho_1 = p_1/(RT_1)\)

3. **Calculate enthalpy changes**:
   \[h_2 - h_1 = c_p(T_2-T_1)\]

4. **Calculate kinetic energy changes** (if velocities significant):
   \[\Delta KE = \frac{V_2^2 - V_1^2}{2}\]

5. **Apply steady-flow First Law**:
   \[\dot{Q} - \dot{W}_s = \dot{m}[(h_2-h_1) + \frac{V_2^2-V_1^2}{2}]\]

6. **Solve for unknown**:
   - Usually finding \(\dot{W}_s\) (power required or produced)

### 11.7 Strategy: Cycle Problems

**Typical scenario**: Multi-process cycle with known work/heat per process

**General Steps**:
1. **For each process** (1→2, 2→3, etc.):
   - Apply First Law: ΔE = Q - W
   - Identify if adiabatic (Q=0), constant volume (W=0), etc.

2. **For complete cycle**:
   - Net energy change: ΔE_cycle = 0 (returns to initial state)
   - Net heat: Q_net = Σ Q_i
   - Net work: W_net = Σ W_i
   - First Law: Q_net = W_net

3. **Calculate efficiency**:
   \[\eta_{th} = \frac{W_{net}}{Q_{in}} = 1 - \frac{Q_{out}}{Q_{in}}\]

4. **Check**: Q_net should equal W_net (for cycle)

---

## 12. REFERENCE TABLES & CONSTANTS

### 12.1 Standard Constants

\[g = 9.81 \text{ m/s}^2 \text{ (standard gravity)}\]
\[g_c = 1 \text{ (in SI units, dimensionless)}\]
\[R_{universal} = 8.314 \text{ J/(mol·K)}\]
\[p_{atm} = 101,325 \text{ Pa} = 1.01325 \text{ bar}\]

### 12.2 Common Fluid Properties @ 20°C, 1 atm

| Fluid | ρ (kg/m³) | μ (Pa·s) | ν (m²/s) | γ (kN/m³) |
|-------|-----------|----------|----------|-----------|
| Water | 998 | 0.001 | 1.0 × 10⁻⁶ | 9.79 |
| Air | 1.20 | 1.81 × 10⁻⁵ | 1.51 × 10⁻⁵ | 0.0118 |
| Oil | 860 | 0.110 | 1.28 × 10⁻⁴ | 8.44 |
| Mercury | 13,600 | 0.0015 | 1.1 × 10⁻⁷ | 133 |

### 12.3 Specific Heats (ideal gases at 20°C)

| Gas | R (kJ/kg·K) | cp (kJ/kg·K) | cv (kJ/kg·K) | k |
|-----|-------------|--------------|--------------|-----|
| Air | 0.287 | 1.005 | 0.718 | 1.40 |
| N₂ | 0.297 | 1.040 | 0.743 | 1.40 |
| O₂ | 0.260 | 0.918 | 0.658 | 1.40 |
| CO₂ | 0.189 | 0.846 | 0.657 | 1.29 |
| CH₄ | 0.519 | 2.25 | 1.73 | 1.30 |

### 12.4 Common Second Moments of Area (about centroid)

| Shape | Centroid Location | \(I_G\) |
|-------|-------------------|---------|
| Rectangle (b × h) | b/2, h/2 | \(\frac{bh^3}{12}\) |
| Circle (diameter d) | Center | \(\frac{\pi d^4}{64}\) |
| Triangle (base b, height h) | h/3 from base | \(\frac{bh^3}{36}\) |
| Trapezoid | Varies | See geometry tables |

---

**Document Complete**  
Last Updated: December 2025  
All formulas tested against MEC 511 exams (2012W, 2013W, 2014W)