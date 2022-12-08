# Smart-Wheel-Chair-Simulation

We create an angular web application that simulates a real-time movement of a smart wheel chair .


## The application is divided into 3 modules : 
- Control Panel :

Its a panel where the chair operating and movement systems are controlled ,

-  Speed and breaking subsystem :
      -pre-define the constant speed of the chair
      -controle the speed on going uphill and downhill as the application simulates the action of gyrometer sensor that measure the angular velocity and help in controlling speed where ,

     a) righ angle, represents the normal state  of the straigh movment . 
     b) acute angle , represents going uphill  .  
     c) obtuse angle , represents going downhill  . 
       ![Screenshot (147)](https://user-images.githubusercontent.com/71048834/205659984-f8028285-a42c-4e46-974c-506146c53973.png) 

-  Navigation and location monitoring subsystem : 
  
  A simulation for the action of ulrasonic sensor as on sensing an obstacle , it will give the motor an order       to stope till it gets another order for moving in a certain direction . 


- Power and energy consumption : 

   That system responsible for monitoring the battary and upon reaching a certain level it will notify the user     of the chair to charge the battary ( once battary is less than 20 % )   
## Firebase module  

   All the updates that happens in the controle panel is stored in the firebase automatically and updated in the    dashboard to show the current state of the chair  
## Dashboard module 
 Its a separete page that shows the current state of the chair and updates it in a real time manner according to the changes happens to chair's environment or state   
