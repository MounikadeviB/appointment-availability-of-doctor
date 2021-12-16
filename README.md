# tasks

#%RAML 1.0
title: Doctors appointment
description: Details of availability of doctors appointment

/add-information of a patient:
   post:
     body:
       application/json:
         example:
       {
             '  "name of the patient" : "Ravi"
              "contact number" : "9465286655"
              "age" : "43"        
       }
    responses:
      10:
        body:
          application/json:
            example:
              {
              "status":10,
              "message": " Appointment is fixed"
               }   
      11:
        body:
          application/json:
            example:
              {
                "status" : 11,
                "message" : "Appointment is not available"
              }     
