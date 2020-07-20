# Control Interface

This folder contains the source code and instructions to execute the interface developed to control vehicle inside GTA V game. This interface sends driving commands during simulations inside the game using as inputs real-time acquired images and normalized values of speed. These data are acquired with the data acquisition interface and are normalized to be used in model. The model output is processed using a virtual joystick simulated with vJoy driver and the Pvjoy library and software x360ce sends the commands to the game to control the vehicle.A diagram of the system is shown below:

![](henriqueyda/Autonomous-Vehicle-GTA-V/blob/master/images/control_interface.png)

The instructions to run this program are the following:

**Preparing System**
- Create speed.txt file in (D:) directory 
- Insert Velocidade.asi file in GTA V folder (in Steam usually is: C:\Program Files (x86)\Steam\steamapps\common\Grand Theft Auto V)
- Download ScriptHookV.dll mod library and follow instruction in http://www.dev-c.com/gtav/scripthookv
- Install x360ce and vJoy 
- Insert x360ce in GTA V folder
- Insert path to neural network model in "Model" variable

**Starting Mod**
- Get into a car inside game
- Press F4 to execute program 
- The text "ligando" will appear on screen
- Press key NUM_9 to check speed values in real time
- The text "Comunicar ativado" will appear on screen

**Executando a interface de controle**
- Each key execute the described function
    - Keys:
        - o: Starts vehicle control
        - p: Turns off vehicle control in simulation environment
        - z: Stops program execution
- Mod configuration:
        - NUM_1: Decreases counter that fast-foward time in one second
        - NUM_2: Increases counter that fast-foward time in one second
        - NUM_8: Turns on/off speed print on screen
        - NUM_9: Turns on/off speed recording in Speed.txt file