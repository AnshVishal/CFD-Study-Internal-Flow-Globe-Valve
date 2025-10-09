<h1 align='center'>CFD STUDY OF GLOBE VALVE (INTERNAL FLOW)</h1>
<p align="center"><i>Disclaimer: This project is a part of Flowthermolab CFD mentorship Program.</i></p>
<h2 align='center'>OVERVIEW</h2>
<p align='left'><b>1. Problem Statement</b></p>
<ul>
  <li> Pressure Based Solver, Steady state CFD Simulation</li> 
  <li>Study the flow phenomenon, discharge coefficient and force on valve</li> 
  <li>Study must be conducted over different valve openings & different Inlet conditions</li>
</ul>
<p align="left"><b>Note: </b> <i>It is to highlight that this study has been performed to understand the internal fluid flow dynamics through the globe valve geometry and the studied parameters such as discharge rate and mass flow rate so as to understand what are the design changes from perspective of a CFD Engineer (Refer to Discussion Section for more details.)</i></p>
<p align='justify'><b>2. Software Used: </b><br/> Ansys Space-Claim  &nbsp | &nbsp Ansys Fluent Mesher &nbsp | &nbsp Ansys Fluent &nbsp | &nbsp Ansys Post Processor &nbsp | &nbsp MATLAB (for Scientific Plots)</p>
<p align='justify'><b>3. Skills Demonstrated: </b><br/>Dynamic Meshing &nbsp | &nbsp Transient &nbsp | &nbsp Turbulence (k-omega SST) and 6DOF Modeling &nbsp | &nbsp Data Post-Processing</p>





        
<h2 align='center'>METHODOLOGY</h2>
<p>Methodology for the following process comprised of geometry refinement, Domain Preparation in Spaceclaim, meshing the geoemtry for different valve openings, defning the solver details, Solution Details like generating run time residuals and animations, understanding the convergence of results through plots, study results and plot them in MATLAB/python, concluding the project with findings and future scope.</p> 
<p>Details for the Methodology can be seen from table below:</p> 
<p align="center">Table 1: Details of Project Methodology</p>  
<table align="center">
<thead> <tr> <th>Stage</th> <th>Details</th> </tr> </thead>
<tbody> 
  <tr> <th>Geometry & Domain</th>
  <th><img width="776" height="199" alt="image" src="https://github.com/user-attachments/assets/b8d99a99-d004-4786-9fb6-49ddbe87d82a" /><br/>
    <b>Figure 1: Globe Valve Geometry and Domain</b><br/>
    <pre><p align="left">Note: <br/> The inlet & outlet were extended to prevent errors during solving like backflow problem.</p></pre>
    
  </th></tr>
  
  <tr> <th>Meshing</th>
  <th><img width="728" height="141" alt="image" src="https://github.com/user-attachments/assets/0ab22edf-9bb5-4831-8887-e4c030fdce5c" /><br/>
    <b>Figure 2: Meshing at different valve openings (1mm, 3mm, 5mm, 11mm, 21mm)</b>
    <pre><p align="left">Note: <br/> Mesh was generated focusing on area of study that is (1) around the valve and (2) valve opening.
    For Boundary Layer Mesh, first layer height was calculated at Y<sup>+</sup> < 5. First Layer Height is 8 X 10<sup>-6</sup>
    Hexcore Volume Mesh was generated with 1mm as max cell length and 4mm  as min cell length
    Total Elements were ~900000 for all cases withh average orthogonality 0.95</p></pre>
  </th></tr>

  <tr> <th>Solver Details</th>
    <th>
      <pre><p align="left">
1. Solver:           Pressure Based
2. Time:             Steady
3. Viscous Model:    k-omega SST
4. Material:         Water-liquid
5. Inlet Boundary:   Pressure type, 4e<sup>5</sup>, 5e<sup>6</sup>, & 8e<sup>8</sup>
6. Outlet Boundary:  Pressure type, 3e<sup>5</sup>
7. Method:           Coupled Solver, Quick Scheme for Momentum Equation
8. Initialization:   Hybrid
9. Iterations:       5000~10000
      </p></pre>
    </th></tr>
    
  <tr><th>Results: Pressure & Velocity Contours</th>
    <th><img width="350" height="1077" alt="Screenshot 2025-10-06 225005" src="https://github.com/user-attachments/assets/9b7f86ea-f5ef-4ed4-8268-66ee1aef6637" /><img width="350" height="1079" alt="Screenshot 2025-10-06 225236" src="https://github.com/user-attachments/assets/a3fa04e4-f37f-414b-8149-86373dace995" /><br/>
    Figure 3: Pressure & Velocity Contours at Pressure Difference 1bar, 2bar, 5bar for different valve openings</tr>

  <tr><th>Results: Residuals & Report Definition</th>
    <th><img width="225" height="362" alt="image" src="https://github.com/user-attachments/assets/b2fda2c7-0770-486a-9ae8-7a34c0379351" /><img width="221" height="366" alt="image" src="https://github.com/user-attachments/assets/891551a1-c702-44c9-8324-7164e3422780" /><img width="229" height="357" alt="image" src="https://github.com/user-attachments/assets/94327bf1-000e-40d8-963e-29c4815ffb50" /><br/>
Figure 4: Residuals, Mass Flow Rate at outlet and Force on valve in y-direction
<pre><p align="left">Note:
It is only for one simulation case, there were altogether 15 cases</p></pre>
    </th></tr>

  <tr><th>Results: Discharge Rate & Mass Flow Rate</th>
    <th><img width="350" height="723" alt="image" src="https://github.com/user-attachments/assets/ff8cbd49-3fdf-4599-94be-59d69c523fe4" /><img width="350" height="723" alt="image" src="https://github.com/user-attachments/assets/d70ac64e-85a6-4c04-ab75-ea757e5b662f" /><br/>
Figure 5: Discharge Rate (C<sub>d</sub>) & Mass Flow Rate vs valve opening in Percentage
</tbody>
</table>



<h2 align='center'>DISCUSSION & FUTURE SCOPE</h2>
<p>In this study CFD Simulations for the Globe Valve over the valve for different valve openings (1mm, 3mm, 5mm, 11mm, 21mm) for different Pressure inlet conditions (4 bar, 5 bar, 8 bar) keeping pressure outlet at 3 bar constant (for all cases). Pressure and Velocity were studied through contours understanding the pressure changes and flow rates at different location. Plot for discharge coefficient and mass flow rate.<br/> 
  &nbsp&nbsp It can be observed from the results main pressure drop occured at the valve throat due to diminished area at less valve lift values. The inherent flow coefficient was obtained through CFD keeping the pressure difference constant for full range (1 ~ 21mm) of opening and obtained the discharge Coefficient and mass flow rate.<br/> 
  &nbsp&nbsp Three most common flow characteristics of a valve which are called quick (fast) opening type, linear type and equal percentage type.
  <ul>
    <li><b><i>Quick opening type</i></b> produces a large increase in flow rate for initial increase in valve ope is usually used for safety or cooling system where the instant large flow is required. </li>
    <li><b><i>Linear type</i></b> has a linear relationship between the flow rate and the valve opening that is commonly used in liquid level conrol applications.</li>
    <li><b><i>Equal percentage type</i></b> provides a small increase in flow rate with the initial valve openings and a significant rise with the greater openings and is widely found in pressure control and heat transfer process. </li>
  </ul>
  &nbsp&nbsp The pressure drop was studied from the contours, the pressure at two planes that comprised of proper representation of valve opening the flow circulation and pressure changes. As it is evident from the graph represented above quick opening flow charateristic and the graph resembles the common characteristic trend for discharge rate and mass flow rate.<br/> 
  &nbsp&nbsp Findings Summarized: 
  <ul>
    <li>The data generated concluded that there were significant changes in pressure around globe valve specially in small (1mm, 3mm) valve opening, maximum force on the valve 2143.762 N was recorded at pressure difference 5bar and with valve lift the it reduced upto 90.49 N.</li>
    <li>The discharge rate coefficient reduced with more valve lift decreased while the mass flow rate increased, maximum discharge coefficient 0.6012 was recorded at pressure difference 5bar Pa with minimum mass flow rate 1.54 kg.s<sup>-1</sup>recorded at pressure difference 1bar </li>
  </ul>
</p>
    
<h2 align='center'>CONTACT DETAILS</h2>
