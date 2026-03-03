<h1 align='center'>Computing Internal Flow in a Globe Valve </br>
<h4 align='center'>Dynamic Meshing &nbsp | &nbsp Transient &nbsp | &nbsp Turbulence (k-omega SST) and 6DOF Modeling &nbsp | &nbsp Data Analysis</h4></h1>

<p align="right">Minor Project 1 - Internal Flows,</br> Flowthermolab </br>09/10/2025</p>
<h2 align='left'>Project Overview</h2>
<p align = "left">This project presents a comprehensive CFD investigation of internal flow through a globe valve to analyze: </br>
<ul>
      <li>Flow behavior at different valve openings</li>
      <li>Discharge coefficient (Cd)</li>
      <li>Mass flow rate</li>
      <li>Hydrodynamic force acting on the valve</li>
</ul>
The study evaluates the valve under multiple inlet pressure conditions to understand flow characteristics and identify possible design improvements from a CFD engineering perspective.
</p>

<h2 align "left">Problem Statement</h2>
<p align='left'>Perform Steady state, CFD Simulations for the Globe Valve Geometry, study the flow phenomenon, compare and discuss the discharge coefficient and force in y-direction over the valve for different valve openings (1mm, 3mm, 5mm, 11mm, 21mm) and evaluate performance at different inlet pressures (4 bar, 5 bar, 8 bar). 

<h2 align = "left">Software Used</h2>
<p align='justify'>
      1. &nbsp Ansys Space-Claim ------- Geometry Cleanup and refinement </br> 
      2. &nbsp Ansys Fluent Mesher ----- Mesh / Grid Generation </br>
      3. &nbsp Ansys Fluent ------------- Computation </br>
      4. &nbsp Ansys Post Processor ---- Post Processing </br>
      5. &nbsp MATLAB ------------------ Data Analysis & Scientific Plots</p>
    
<h2 align='left'>Methodology</h2>

<h3 align = "left">1. Geometry Cleanup and refinement</h3>
<p align = "justify">
      <ul><li>Inlet and outlet extensions were added to avoid backflow errors.</li>
            <li>Internal flow domain extracted for simulation.</li></ul></p>
<p align = "center"><img width="620" height="199" alt="image" src="https://github.com/user-attachments/assets/b8d99a99-d004-4786-9fb6-49ddbe87d82a" /><br/>
    <b>Globe Valve Geometry and Domain</b></p>

<h3 align = "left">2. Mesh Details</h3>
<p align = "justify">
      <ul><li>Focused on mesh refinement at: Valve throat, Valve seat, and Valve lift region.</li>
            <li>Mesh Details: 
                  <ul><li>Hexcore volume mesh</li>
                  <li>~900,000 elements</li>
                        <li>Average orthogonality: 0.95</li>
                        <li>Y⁺ < 5</li>
                        <li>First layer height: 8 × 10⁻⁶ m</li>
                        <li>Max cell length: 1 mm</li>
                        <li>Min cell length: 4 mm</li></ul></li>
            <li>Valve Lift Cases: 1mm, 3mm, 5mm, 11mm, 21mm</li></ul>
</p>
<p align = "center"><img width="620" height="141" alt="image" src="https://github.com/user-attachments/assets/0ab22edf-9bb5-4831-8887-e4c030fdce5c" /><br/>
            <b>Meshing at different valve openings (1mm, 3mm, 5mm, 11mm, 21mm)</b></p>


<h3 align = "left">3. Solver Settings</h3>
<table align = "center">
      <tr><th>Parameter</th><th>Setting</th></tr>
      <tr><td>Solver Type</td><td>Pressure-Based</td></tr>
      <tr><td>Time</td><td>Steady</td></tr>
      <tr><td>Turbulence Model</td><td>k-ω SST</td></tr>
      <tr><td>Material</td><td>Water (Liquid)</td></tr>
      <tr><td>Inlet BC</td><td>Pressure Inlet (4 bar, 5 bar, 8 bar)</td></tr>
      <tr><td>Outlet BC</td><td>Pressure Outlet (3 bar)</td></tr>
      <tr><td>Solver Scheme</td><td>Coupled</td></tr>
      <tr><td>Momentum Discretization</td><td>QUICK Scheme</td></tr>
      <tr><td>Residuals & Reports</td><td><ul><li>Mass flow rate,</li> <li>Y-direction force on valve</li></ul></td></tr>
      <tr><td>Initialization</td><td>Hybrid</td></tr>
      <tr><td>Iterations</td><td>5000–10000</td></tr>
</table>
<p align = "left"><b>Total simulation cases: 15 </br>(5 valve openings × 3 inlet pressures)</b></p>

<h3 align = "left">4. Results</h3>
<h4 align = "left">Velocity and Pressure Contours</h4>
<p align = "center"><img align = "center" width="350" height="1077" alt="Screenshot 2025-10-06 225005" src="https://github.com/user-attachments/assets/9b7f86ea-f5ef-4ed4-8268-66ee1aef6637" />
<img align = "center" width="350" height="1079" alt="Screenshot 2025-10-06 225236" src="https://github.com/user-attachments/assets/a3fa04e4-f37f-414b-8149-86373dace995" /><br/>
<b>Pressure & Velocity Contours at Pressure Difference 1bar, 2bar, 5bar for different valve openings</b></p>
<h4 align = "left">Discharge Rate & Mass Flow Rate</h4>
<p align = "center"><img width="350" height="723" alt="image" src="https://github.com/user-attachments/assets/ff8cbd49-3fdf-4599-94be-59d69c523fe4" /><img width="350" height="723" alt="image" src="https://github.com/user-attachments/assets/d70ac64e-85a6-4c04-ab75-ea757e5b662f" /><br/>
<b>Discharge Rate (C<sub>d</sub>) & Mass Flow Rate vs valve opening in Percentage</b></p>

<h3 align = "left">5. Discussion & Future Scope</h3>
<p align='justify'>In this study CFD Simulations for the Globe Valve over the valve for different valve openings (1mm, 3mm, 5mm, 11mm, 21mm) for different Pressure inlet conditions (4 bar, 5 bar, 8 bar) keeping pressure outlet at 3 bar constant (for all cases). Pressure and Velocity were studied through contours understanding the pressure changes and flow rates at different location. Plot for discharge coefficient and mass flow rate.<br/> 
  &nbsp&nbsp It can be observed from the results main pressure drop occured at the valve throat due to diminished area at less valve lift values. The inherent flow coefficient was obtained through CFD keeping the pressure difference constant for full range (1 ~ 21mm) of opening and obtained the discharge Coefficient and mass flow rate.<br/> 
  &nbsp&nbsp Three most common flow characteristics of a valve which are called quick (fast) opening type, linear type and equal percentage type.
  <ul>
    <li><b><i>Quick opening type</i></b> produces a large increase in flow rate for initial increase in valve ope is usually used for safety or cooling system where the instant large flow is required. </li>
    <li><b><i>Linear type</i></b> has a linear relationship between the flow rate and the valve opening that is commonly used in liquid level conrol applications.</li>
    <li><b><i>Equal percentage type</i></b> provides a small increase in flow rate with the initial valve openings and a significant rise with the greater openings and is widely found in pressure control and heat transfer process. </li>
  </ul>
  &nbsp&nbsp The pressure drop was studied from the contours, the pressure at two planes that comprised of proper representation of valve opening the flow circulation and pressure changes. As it is evident from the graph represented above quick opening flow charateristic and the graph resembles the common characteristic trend for discharge rate and mass flow rate.<br/> <br/>
  &nbsp&nbsp <b><i>Findings Summarized:</i></b> 
  <ul>
    <li>The data generated concluded that there were significant changes in pressure around globe valve specially in small (1mm, 3mm) valve opening, maximum force on the valve 2143.762 N was recorded at pressure difference 5bar and with valve lift the it reduced upto 90.49 N.</li>
    <li>The discharge rate coefficient reduced with more valve lift decreased while the mass flow rate increased, maximum discharge coefficient 0.6012 was recorded at pressure difference 5bar Pa with minimum mass flow rate 1.54 kg.s<sup>-1</sup>recorded at pressure difference 1bar </li>
  </ul>
  &nbsp&nbsp <b><i>Future Scope:</i></b> 
  <ul>
    <li>Perform study to capture cavitation effects</li>
    <li>Perform Preliminary Study and investigate the optimization methods</li>
    <li>Optimize the design of control valve and reduce the force exerted on valve make globe valve more efficient and reduce loud noise generated from globe valve </li>
  </ul>
</p>

<h2>Recommended Repository Structure</h2>

<pre>
CFD-Study-Globe-Valve/
│
├── README.md
├── Geometry image
├── Mesh images
├── Fluent_Case_Files
├── Results & Data
</pre>

    

