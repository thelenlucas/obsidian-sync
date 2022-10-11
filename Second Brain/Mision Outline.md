# Ghist
Overview of the mission

Part of a series on #Cansat_2023 

# Description
The mission is to simulate the landing sequence of a planetary probe. Design a Cansat that shall consist of a container and a probe. The Cansat shall be launched to an altitude ranging from 670 meters to 725 meters above the launch site and deployed near apogee (peak altitude). Orientation of deployment is not controlled and is very violent with large shock forces. The Cansat must survive the forces incurred at launch and deployment. Once the Cansat is deployed from the rocket, the Cansat shall descend using a parachute at a rate of 15 m/s. At 500 meters, the Cansat shall release a probe that shall open a heat shield that will also be used as an aerobraking device with a descent rate of 20 meters/second or less. A parachute, streamer, parafoil or similar device shall not be used with the heat shield. When the probe reaches 200 meters, the probe shall deploy a parachute and slow the descent rate to 5 meters/second. Once the probe has landed, it shall attempt to upright itself and raise a flag 500 mm above the probe. A video camera shall be included and point toward the ground during descent.

# Informal Staging Overview

| Stage | Starting Condition | Ending Condition    |
| ----- | ------------------ | ------------------- |
| One   | Cansat is deployed | Cansat Reaches 500m |
| Two   | Altitude < 500m    | Altitude < 200m     |
| Three | Altitude < 200m    | Ground                    |

