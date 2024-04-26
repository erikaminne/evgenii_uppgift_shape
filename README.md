# evgenii_uppgift_shape
Evgeniis uppgift där python coden ska känna igen vad för sorts shape som bilden visar.
Jag följde instruktioner på websidan https://www.geeksforgeeks.org/how-to-detect-shapes-in-images-in-python-using-opencv/ som Anton hade delat med mig.

Efter att jag har importerat alla nödvändiga modules så börjar jag med att läsa av bilden som jag har skapat. 
Efter det så convertar jag bilden till grayscale eftersom det gör de lättare att avläsa och identifiera de olika formerna i bilden. 
Programmet räknar sedan ut hur många kanter formern har och kan på basen av det säga vilken form det är.

if len(approx) == 3: 
        cv2.putText(img, 'Triangle', (x, y), 
                    cv2.FONT_HERSHEY_SIMPLEX, 0.6, (0, 0, 0), 2) 
  
   elif len(approx) == 4: 
        cv2.putText(img, 'Quadrilateral', (x, y), 
                    cv2.FONT_HERSHEY_SIMPLEX, 0.6, (0, 0, 0), 2) 
  
   elif len(approx) == 5: 
        cv2.putText(img, 'Pentagon', (x, y), 
                    cv2.FONT_HERSHEY_SIMPLEX, 0.6, (0, 0, 0), 2) 
  
   elif len(approx) == 6: 
        cv2.putText(img, 'Hexagon', (x, y), 
                    cv2.FONT_HERSHEY_SIMPLEX, 0.6, (0, 0, 0), 2) 
  
   else: 
        cv2.putText(img, 'circle', (x, y), 
                    cv2.FONT_HERSHEY_SIMPLEX, 0.6, (0, 0, 0), 2) 

Här sätter jag namn in på basen av hur många kanter former har. 
