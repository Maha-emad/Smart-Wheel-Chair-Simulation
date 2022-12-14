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
 
 
 

## Simulation
 - Control panel 

 Here on adding a new chair and defining its state , a new document will be created in the firestore and the data will be updated in the dashboard application in areal-time manner .
 
 - Through the  control panel we can determine the state of the smart chair  ,
   Define if there  exists an obstacle or not ,"Sense free space" field is only opened if there is a sensed oobstacle to select the next destination  ,battery charge is set and notify the user if the value is below 20%  
   determining the angle specifies going uphill ,downhill or in straighh direction 
   Id of the  chair helps to distinguish  between different chairs on the dashboard  

   Control panel allows  you to add a  chair or  update an existing chair.
   
   ![Screenshot (177)](https://user-images.githubusercontent.com/71048834/206568247-14f68026-1ee1-47dc-b9cb-2642bd0ddf84.png)


  Firbase  
  -
 
 Each created chair creates a document in the firebase   

 ![Screenshot (178)](https://user-images.githubusercontent.com/71048834/206568641-42a2f115-6290-4e78-97f5-64f007238ba9.png)

 Dashboard 
 -

Before sensing an obstacle 


![Screenshot (169)](https://user-images.githubusercontent.com/71048834/206568885-8ea6c159-8799-4e72-b2ba-9eea59725977.png) 


After sensing an obstacle 

![Screenshot (173)](https://user-images.githubusercontent.com/71048834/206569013-a7c49c5a-5786-405a-bbd0-444396229363.png)

Deployment
-
- [Panel](https://wheelchair-trials.web.app/Smart-Wheel-Chair-Simulation/)
 

 


 
