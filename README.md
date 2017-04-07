# ArduinoESCTool
A simple Arduino code to calibrate or test ESC(Electronic Speed Controller) and/or Servomotors with customisable frequency and other parameters

WHAT DOES THIS DO?

Extremely lightweight Android code for ESC CALIBRATION AND/OR ESC TESTING
Customizable frequency, maximum time, minimum time, maximum signal and minimum signal.
  
This piece of code is a fully functional Arduino code which can be used to calibrate/test Electronic Speed Controllers and/or Servomotors.
 
HOWTO:
1. Set the configuration as per your requirement, in the CONFIGURATIONS area.
2. Upload the sketch to any arduino board.
3. Connect the ESCs' signal wires to any of the pins of PORTB
4. Switch ON the power to Arduino
5. Immediately after or along with the above step, switch ON the power to ESCs.
6. Watch the system while it does the following:

      Generate PWM signals on all pins of PORTB with
         frequency equal to ESC_FREQUENCY_HZ Hertz all over the time,
         Pulse Width equal to SIGNAL_MAX_US microseconds for inital TIME_MAX_SECONDS seconds,
         Pulse Width equal to SIGNAL_MIN_US microseconds for TIME_MIN_SECONDS after TIME_MAX_SECONDS,
         Pulse Width equal to SIGNAL_NORMAL_US microseconds afterwards.
 
LICENCING AND WARRANTY
   This code is openly provided AS IS for any modifications for application anywhere subject to the responsibility of the user.
   The author does not hold any responsibility of any unpredictable behaviour, or any events following the use of the code.
