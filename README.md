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
    <p align="left">Note: <br/> The inlet & outlet were extended to prevent errors during solving like backflow problem.</p>
    
  </th></tr>
  
  <tr> <th>Meshing</th>
  <th><img width="728" height="141" alt="image" src="https://github.com/user-attachments/assets/0ab22edf-9bb5-4831-8887-e4c030fdce5c" /><br/>
    <b>Figure 2: Meshing at different valve openings (1mm, 3mm, 5mm, 11mm, 21mm)</b>
    <p align="left">Note: <br/> Mesh was generated focusing on area of study that is (1) around the valve and (2) valve opening.</p>
  </th></tr>

  <tr> <th>Solver Details</th>
    <th>Validation Case
      <p align="left"><b>Solver: </b> Pressure Based<br/>
      <b>Time: </b> Steady (1) & Transient (2)<br/>
      <b>Gravity: </b> -9.81 ms<sup>-1</sup> (2)<br/>
      <b>Viscous Model: </b> Laminar, Spallart Allmaras, K-omega SST, Reynolds Stress Model (1) & k-omega SST (2)
      </p>
      <p align="center">Final Case</p>
      <p align="left">Final Case</p>
      
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
