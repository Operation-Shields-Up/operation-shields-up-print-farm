                   .:                     :,                                          
,:::::::: ::`      :::                   :::                                          
,:::::::: ::`      :::                   :::                                          
.,,:::,,, ::`.:,   ... .. .:,     .:. ..`... ..`   ..   .:,    .. ::  .::,     .:,`   
   ,::    :::::::  ::, :::::::  `:::::::.,:: :::  ::: .::::::  ::::: ::::::  .::::::  
   ,::    :::::::: ::, :::::::: ::::::::.,:: :::  ::: :::,:::, ::::: ::::::, :::::::: 
   ,::    :::  ::: ::, :::  :::`::.  :::.,::  ::,`::`:::   ::: :::  `::,`   :::   ::: 
   ,::    ::.  ::: ::, ::`  :::.::    ::.,::  :::::: ::::::::: ::`   :::::: ::::::::: 
   ,::    ::.  ::: ::, ::`  :::.::    ::.,::  .::::: ::::::::: ::`    ::::::::::::::: 
   ,::    ::.  ::: ::, ::`  ::: ::: `:::.,::   ::::  :::`  ,,, ::`  .::  :::.::.  ,,, 
   ,::    ::.  ::: ::, ::`  ::: ::::::::.,::   ::::   :::::::` ::`   ::::::: :::::::. 
   ,::    ::.  ::: ::, ::`  :::  :::::::`,::    ::.    :::::`  ::`   ::::::   :::::.  
                                ::,  ,::                               ``             
                                ::::::::                                              
                                 ::::::                                               
                                  `,,`


https://www.thingiverse.com/thing:909901
Retraction test  by deltapenguin is licensed under the GNU - GPL license.
http://creativecommons.org/licenses/GPL/2.0/

# Summary

(10/19/2016)
I did retraction calibration for B'struder.

Extruder drive: B’struder
Kysan Nema 17 5.18:1 geared stepper motor, 2.4 V, 1.0 A

config.g of RepRapFirmware-dc42 1.12a

M92 411.230
M201 X4000 Y4000 Z4000 E3000 ; Accelerations (mm/s^2)
M203 X15000 Y15000 Z15000 E15000 ; Maximum speeds (mm/min)
M906 X800 Y800 Z800 E800 ; Set motor currents (mA)
M92 411.230

Retraction setting in Slic3r 1.2.9:
Length: 3.4 mm
Z Lift: 0.4 mm
Speed: 15 mm/s (10 mm/s and 20 mm/s give similar result.)
Retraction after layer change: on
Wipe on retraction: on

Filament: eSun PLA 1.75 mm
Layer height: 0.2 mm 
Printing speed: 20 mm/s
Travel speed: 250 mm/s

190 degrees Celsius gave better result than 180 degrees Celsius. Why?!
(3/16/2016)

White one was done by RepRapPro Fisher last year.
There was huge improvement in retraction quality. 
Only modification I did I glued end of Bowden tube on the push fitting of the extruder half year ago. 

190 C or 180C wouldn't make much difference. 

Slic3r settings (3/16/2016):
Layer height: 0.25 mm
Travel speed: 200 mm/s

Retraction
Length: 2 mm
Lift Z: 0.4 mm
Speed: 40 mm/s
Minimum travel after retraction: 2 mm
Retract on layer change: on 
Wipe while retracting: on

Previous Slic3r settings (2015):  
Layer height; 0.1 mm  
Extrusion width: 0.28 mm  
Printing speed: 30 mm/s  
Travel speed: 20 mm/s  
Retraction   
Length: 4.5 mm  
Lift Z: 0.075 mm  
Speed: 150 mm/s  
Extra length on restart: 0.1 mm  

Source:  
Fine Positive Features Performance  
http://www.thingiverse.com/download:872736