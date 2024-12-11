# Building a 1D Geomechanical Model  

This document outlines the step-by-step procedure to build a 1D geomechanical model, which involves analyzing well log data, calculating key rock properties, and estimating stresses and pressures within the subsurface.

---

## **Step 1: Data Loading and Preparation**  
1. **Load Well Log Data**: Begin by loading well log data into a structured format suitable for analysis. Ensure the data includes essential logs such as density, compressional and shear slowness, and gamma ray.  
2. **Define the Zone of Interest**: Select the depth range for the analysis to focus on the relevant interval of the subsurface.  
3. **Data Quality Control (QC)**: Perform a quality check on the data using visual tools like pair plots to identify outliers or inconsistencies. Ensure logs are complete and reliable for calculations.

---

## **Step 2: Rock Property Calculations**  
1. **P-Wave and S-Wave Velocities**: Convert compressional and shear slowness logs to velocities for elastic property calculations.  
2. **Density Conversion**: If density is recorded in g/cm³, convert it to kg/m³ for consistency in units.  
3. **Elastic Moduli**: Compute key elastic properties such as:  
   - **Bulk Modulus (K)**: Reflecting the material's resistance to uniform compression.  
   - **Shear Modulus (μ)**: Indicating the material's resistance to shear deformation.  
   - **Lame's Parameter (λ)**: A measure of the compressibility of the rock.  
4. **Poisson's Ratio and Young's Modulus**: Determine Poisson's ratio (ν) and Young's modulus (E) to characterize the elastic behavior of the rock.

---

## **Step 3: Unconfined Compressive Strength (UCS) Calculation**  
- Use calibrated relationships between log-derived properties and laboratory core data to estimate UCS values for the zone of interest.  

---

## **Step 4: Pore Pressure Calculation**  
- Estimate pore pressure using empirical or log-derived methods such as Eaton’s or Bowers’ methods. Calibrate the model using available formation pressure data (e.g., MDT measurements).  

---

## **Step 5: Fracture Pressure Calculation**  
- Calculate fracture pressure using a fracture gradient, which can be derived from empirical correlations or calibrated using field data. This defines the pressure required to induce fracturing in the formation.  

---

## **Step 6: Stress Profile Calculation**  
1. **Vertical Stress (σv)**: Integrate density logs over depth to compute the overburden stress.  
2. **Minimum Horizontal Stress (Shmin)**: Estimate using poroelastic equations and calibrated field data.  
3. **Maximum Horizontal Stress (SHmax)**: Derive using available stress field information, ensuring compatibility with borehole breakouts or drilling-induced fractures.

---

## **Step 7: Visualization and Interpretation**  
1. **Plot Pore Pressure and Fracture Pressure**: Visualize the calculated pore pressure, fracture pressure, and mud weight profiles to evaluate drilling safety margins.  
2. **Stress Profiles**: Present vertical, minimum horizontal, and maximum horizontal stress profiles, along with elastic moduli and UCS.  

---

## **Step 8: Calibration and Validation**  
- Cross-check calculated properties against available core, test, or field data (e.g., UCS tests, MDT, LOT). Update empirical constants and models as necessary to improve accuracy.

---

## **Step 9: Integration into 1D Model**  
- Combine all derived parameters into a comprehensive 1D geomechanical model. This model serves as a basis for wellbore stability analysis, hydraulic fracture design, and subsurface stress characterization.

