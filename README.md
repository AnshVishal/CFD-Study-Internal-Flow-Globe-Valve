<h1 align='center'>CFD STUDY OF GLOBE VALVE (INTERNAL FLOW)</h1>

<h2 align='center'>OVERVIEW</h2>
<p align='left'>1. Problem Statement</p>
<ul>
  <li> Pressure Based Solver, Steady state CFD Simulation</li> 
  <li>Study the flow phenomenon, discharge coefficient and force on valve</li> 
  <li>Study must be conducted over different valve openings & different Inlet conditions</li>
</ul>
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
    
  <tr><th>Results: Pressure Contours</th>
    <th><img width="362" height="506" alt="image" src="https://github.com/user-attachments/assets/ded4e104-739b-41f9-84bb-ce66ed5022f5" />
  <img width="325" height="506" alt="image" src="https://github.com/user-attachments/assets/26eff6d6-75f1-4d2c-90b0-f93b13fc5600" /><br/>
    Figure 3: Pressure Contours at Pressure Difference 1bar, 2bar, 5bar for different valve openings</tr>
      
  <tr><th>Results: Velocity Contours</th>
    <th><img width="362" height="484" alt="image" src="https://github.com/user-attachments/assets/d27820ca-17f8-4fc6-a68f-ca6dd85e8765" /><img width="303" height="506" alt="image" src="https://github.com/user-attachments/assets/de724afb-9a96-4f8e-bae1-41fb08d1fb8c" /><br/>
Figure 4: Velocity Contours at Pressure Difference 1bar, 2bar, 5bar for different valve openings</th>

  <tr><th>Results: Residuals & Report Definition</th>
    <th><img width="225" height="362" alt="image" src="https://github.com/user-attachments/assets/b2fda2c7-0770-486a-9ae8-7a34c0379351" /><img width="221" height="366" alt="image" src="https://github.com/user-attachments/assets/891551a1-c702-44c9-8324-7164e3422780" /><img width="229" height="357" alt="image" src="https://github.com/user-attachments/assets/94327bf1-000e-40d8-963e-29c4815ffb50" /><br/>
Figure 5: Residuals, Mass Flow Rate at outlet and Force on valve in y-direction
<pre><p align="left">Note:
It is only for one simulation case, there were altogether 15 cases</p></pre>
    </th></tr>

  <tr><th>Results: Discharge Rate & Mass Flow Rate</th>
    <th><img width="350" height="723" alt="image" src="https://github.com/user-attachments/assets/ff8cbd49-3fdf-4599-94be-59d69c523fe4" /><img width="350" height="723" alt="image" src="https://github.com/user-attachments/assets/d70ac64e-85a6-4c04-ab75-ea757e5b662f" /><br/>
Figure 6: Discharge Rate (C<sub>d</sub>) & Mass Flow Rate vs valve opening in Percentage
</tbody>
</table>


<h3 align='left'>Solver Details</h3>


<h2 align='center'>4. RESULTS & DISCUSSION</h2>

<p>It is intended thorugh this study to perform Steady state, CFD Simulations for the Globe Valve, study the flow phenomenon, compare and discuss the discharge coefficient and force in y-direction over the valve for different valve openings (1mm, 3mm, 5mm, 11mm, 21mm) for different Pressure inlet conditions (4 bar, 5 bar, 8 bar) keeping pressure outlet at 3 bar constant (for all cases). 
</p>


<p align="center">
<img width="768" height="467" alt="image" src="https://github.com/user-attachments/assets/74c170d3-c8f3-4ce3-bf39-5157df7ebaca" /><br/>
<b>Figure 3: Velocity Contours for Preasure Difference of 1bar, 2bar, 5bar</b><br/>
  <img width="400" height="221" alt="image" src="https://github.com/user-attachments/assets/0d461341-18d2-4520-b309-59df52d8cce3" />
    <img width="400" height="221" alt="image" src="https://github.com/user-attachments/assets/316c6568-0263-4ec6-839b-569558c67f22" /><br/>
<b>Figure 4: Discharge Rate vs Lift Percent Graph</b>
<b>Figure 5: CFD Mass Flow Rate vs Lift Percent Graph</b>
</p>


<h2 align='center'>5. CONCLUSION</h2>

<h2 align='center'>CONTACT DETAILS</h2>
