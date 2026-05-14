# Dispersion-Limited-Fiber-Length
Dispersion Limited Fiber Length
# Objective: 
 
Calculate the dispersion-limited fiber length for a fiber optic transport system that 
employs standard single-mode fiber and a directly-modulated single-mode laser diode 
transmitter. 
 
Simulate the resulting system and verify that it meets performance objective.  
 
# Theory: 
 
The maximum allowable dispersion (or pulse spread) <img width="76" height="52" alt="image" src="https://github.com/user-attachments/assets/52dff457-e7aa-4312-aef4-aa4e234afb47" /> is given in terms of the transmission rate R by the following engineering guideline <img width="192" height="124" alt="image" src="https://github.com/user-attachments/assets/4fcb3de9-6a4a-48db-ba5f-f020a6c85d8b" /> This guideline provides reasonable assurance that there will be no significant inter
symbol interference (ISI) due to pulse spread. 
 
For standard single-mode fiber driven by a directly-modulated laser diode transmitter, the 
pulse spread due to chromatic dispersion is given by
<img width="898" height="694" alt="image" src="https://github.com/user-attachments/assets/5499f4b0-2405-4a5f-b773-ce004a76e850" />
<img width="1300" height="974" alt="image" src="https://github.com/user-attachments/assets/bbd90891-43d6-4a5d-92d2-73ed3e4e57eb" />
# Layout: 
Open up the OptiPerformer file called “Dispersion Limited Fiber.osp”. This layout uses 
the Laser Rate Equations laser diode component with default parameters.  It models a 
directly modulated laser diode based using a standard rate equation model. One of the 
effects of this model is that it generates a signal with a spectral width of about 0.6 nm for 
the default parameters with 2.5 Gb/s, return to zero modulation. 
Within the layout, there are several “Visualizers.” The “Optical Time Domain 
Visualizers” allow the user to the view the simulated signal as a function of time. There is 
one at the output of the laser and one at the end of the fiber.  This allows the user to 
directly observe the changes in the pulses due fiber dispersion. The “Optical Spectrum 
Analyzer” allows the user to view the spectral content of the signal. It this lab it is used to 
verify that the spectral width is about 6 nm. The “BER analyzer” provides calculations of 
the Q factor, the bit error rate (BER) and provides a plot of the eye diagram. 
# Simulation:  
Set the laser power such to achieve a transmitter output power of 0 dBm. The transmitter 
power can be viewed by double clicking the “Output Power Meter Visualizer.” The 
power will read -100 dBm until the first run is made.  
Using the chromatic dispersion factor equation, determine the dispersion of the fiber at 
1550 nm and set the fiber dispersion parameter accordingly. 
Using the equations above, determine the dispersion-limited fiber length. 
<img width="1262" height="1044" alt="image" src="https://github.com/user-attachments/assets/e0b20ca6-42b4-4f1b-ac9a-e4f931a85001" />

<img width="1920" height="1080" alt="Screenshot (4)" src="https://github.com/user-attachments/assets/033fa2f2-b488-4315-9cc5-9a26318ebec5" />
<img width="1920" height="1080" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/c1a2c51f-6af2-4fc7-8308-2ae71a3e97ce" />
<img width="1920" height="1080" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/5bcfa61c-3f63-4b8f-b161-7c6be7854fd1" />
<img width="1920" height="1080" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/73112cf2-f83f-42a7-9a1f-8bc084587f59" />
<img width="1920" height="1080" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/7f06221e-5549-4998-bbb8-a409576d9aa7" />
## tabulation 
<img width="721" height="1280" alt="image" src="https://github.com/user-attachments/assets/dce79fa8-0249-4977-aa66-14f960fc182f" />
<img width="897" height="1128" alt="image" src="https://github.com/user-attachments/assets/c018dec0-ec94-4d68-8f55-b3dd3763717d" />


# Result
The dispersion-limited fiber length for the given optical communication system was found to be approximately 10 km. The simulation results showed acceptable BER performance with a clear eye diagram and minimal intersymbol interference. Hence, the system performance was satisfactory and remained within the allowable dispersion limit.
