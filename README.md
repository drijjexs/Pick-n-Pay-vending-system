# Pick-n-Pay-vending-system
PSEUDOCODE FOR THE SYSTEM
Pick n Pay vending system

DISPLAY’’WELCOM PICK N PAY VENDING SYSTEM SELECT AN OPTION TO  CONTINUE’’

DISPAY  ‘’1. Teller
                  2. Manager
                  3. Employee’’
IF option selected is  1. Teller
  THEN
     TELLERS MODULE
     DISPLAY’’WELCOME TO TELLER SIDE’’
                   -INITIALIZE integer productCode
                   -INITIALIZE string productName
                   -INITIALIZE double price
                   -INITIALIZE integer  quantity
                   -INITIALIZE double VAT 
                   -INITIALIZE read expireDate
 
END

-FUNCTION  sellProducts
                    READ productCode
                    READ quantity
                    CALCULATE  total=productCode*quantity
                   DISPLAY totalPrice
END

-FUNCTION ProductRecord(READ productCode)
                   DISPLAY ProductCode
                   DISPLAY ProductName
                   DISPLAY quantity
                   DISPLAY unitPrice
                   DISPLAY expireDate
END

-FUNCTION reorder (READ productCode)
                  -IF quantity is less than 30
                              THEN reorder MANAGER MODULE
                              END
                   ENDIF
             END
   
          END TELLERS MODULE 

ELSE option selected is  2. MANAGER

                   THEN 
                       MANAGERS MODULE
                       DISPLAY ‘’WELCOME MANAGERS’ SIDE’’
                       
                      -FUNCTION addNewStock (READ productCode)
                              -IF quantity is  less than 30
                                  THEN 
                                     Display’Stock is low’’
                                     READ productCode
                                     READ quantity
                                     READ unitPrice
                  ELSE 
                        THEN
                                     WRITE ‘’ stock level is fine’’

                    END IF
ELSE option selected is 3. EMPLOYEE
                   EMPLOYEES’ MODULE 
                   DISPLAY ‘’WELCOME TO EMPLOYEES ‘ SIDE’’

                     -FUNCTION add New employee
                                     READ employeeID
                                     READ employeeName
                                     READ employementDate 
                                     WRITE ‘’New employee added’’
                                     WRITE workingHours
                    
                     END

                     -FUNCTION read employementType(READ employeeID)
                                     DISPLAY employeeID
                                     DISPLAY  type if contract or permanent
                     END
                     -FUNCTION display EmployeeRecord(READ employeeID)
                                    DISPLAY employeeID
                                    DISPLAY  employeeName 
                                    DISPLAY employementDate
                                   DISPLAY  employementType
                                   RECORD hoursWorked
                    
                      END

                      -FUNCTION display employeeSalary (READ employeeID)
                                 GET hoursWorked
                                 Calculate Salary= hoursWorked*$95
                                 DISPLAY=Salary
                       END
                  ENDIF

