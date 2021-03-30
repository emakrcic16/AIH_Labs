The third lab of the course Artificial Intelligence for Health (DT8029) at Halmstad University consisted of constructing Long Short-Term Memory (LSTM) models for prediction on sequential data. 
The data was collected from Halmstad Intelligent Home (HINT), a smart home located at the University. 
The data consisted of sensor readings from the apartment, telling where the person living in the apartment was. The apartment is split into six main rooms, Living 1, Living 2, Bedroom, Kitchen, Study room, and Bathroom. 
Each of these rooms were assigned a class, 2, 1, 3, 4, 5, 6, respectively. 
A sample sequence of the sensor readings could be [1, 2, 1], which would correspond to that the person was in Living 2, then moved to Living 1, and then back to Living 2.
