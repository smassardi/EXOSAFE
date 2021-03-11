# EXOSAFE
EXOSAFE project database

In this repository are uploaded the file .xlsx relative to each test perfomed for the system validation
The .xlsx files are composed by the following sheets and data:

1) Parameters:
ExoHip: Hip misalignment calculated as 	Leg-Replica_Hip_Position - Exo_Hip_Position [cm]
ExoKnee: Knee misalignment calculated as 	Leg-Replica_Knee_Position - Exo_Knee_Position	[cm]						
MarchVelocity: Selected velocity speed of the gait (1-10)	
TimeShift: Time shift between Leg-Replica data and Exoskeleton data [s] 	
SkinConfig: Configuration of soft tissue 
            0: No material
            1: Silicone material, contact points in the back of the Leg-Replica (shells 2,4,8,5)
            2: Silicone material, contact points in the front of the Leg-Replica (shells 1,3,7,6)
            3: Urethane material, contact points in the back of the Leg-Replica (shells 2,4,8,5)
            4: Urethane material, contact points in the front of the Leg-Replica (shells 1,3,7,6)

2) RawForces: 
Contains the force data directly recorded from the Leg-Replica at 1kHz frequency. Each of the 8 load cells has 3 components (x,y,z)
F_numcell_component [N] (Example F3x: load cell 3, x component)

3) ForceCells:
Contains the force data lowered in sample and adapted to the exoskeleton data at 100Hz frequency. Each of the 8 load cells has 3 components (x,y,z)
F_numcell_component [N] (Example F3x: load cell 3, x component)

4) H3raw:
Contains the raw data received from the exoskeleton evaluated in the testbed validation (H3 Technaid S.L.)
Time: Time of H3 data, 100Hz sample rate	
RhipPosition: Right hip angular position [deg]	
RkneePosition: Right knee angular position [deg]
RanklePosition: Right ankle angular position [deg]	
LhipPosition: Left hip angular position [deg]	
LkneePosition: Left knee angular position [deg]	
LanklePosition: Left ankle angular position [deg]	
RhipTorque: Right hip joint torque [Nm]	
RkneeTorque: Right hip joint torque [Nm]		
RankleTorque: Right hip joint torque [Nm]		
LhipTorque: Left hip joint torque [Nm]		
LkneeTorque: Left knee joint torque [Nm]	
LankleTorque: Left ankle joint torque [Nm]

5) H3processed:
Contains the processed data from the exoskeleton evaluated in the testbed validation (H3 Technaid S.L.)
LHipPos: Left hip filtered position [deg]	
LKneePos: Left knee filtered position [deg]		
LAnklePos: Left ankle filtered position [deg]		
LHipVel: Left hip filtered velocity [deg/s]		
LKneeVel: Left knee filtered velocity [deg/s]			
LAnkleVel	: Left ankle filtered velocity [deg/s]		
LHipAcc: Left hip filtered acceleration [deg/s2]			
LKneeAcc: Left knee filtered acceleration [deg/s2]			
LAnkleAcc: Left ankle filtered acceleration [deg/s2]				
RHipPos: Right hip filtered position [deg]		
RKneePos: Right knee filtered position [deg]		
RAnklePos: Right ankle filtered position [deg]		
LHipTorque: Left hip filtered torque [Nm]		
LKneeTorque: Left knee filtered torque [Nm]		
LankleTorque: Left ankle filtered torque [Nm]		
RHipTorque: Right hip filtered torque [Nm]		
RKneeTorque: Right knee filtered torque [Nm]		
RankleTorque: Right ankle filtered torque [Nm]	

6) Leg-Replica: Contains the data received from the Leg-Replica other than the force data
LegKneePosition: Leg-Replica knee angular position [deg]
LegKneeVelocity: Leg-Replica knee angular velocity [deg/s]
LegKneeTorque: Leg-Replica knee torque [Nm]	
LegKneePositionFiltered: Leg-Replica filtered knee angular position [deg]	
LegKneeVelocityFiltered: Leg-Replica filtered knee angular velocity [deg/s]	
LegKneeTorqueFiltered: Leg-Replica filtered knee torque [Nm]









