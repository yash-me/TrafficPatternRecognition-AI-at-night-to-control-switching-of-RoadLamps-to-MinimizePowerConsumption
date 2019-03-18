# TrafficPatternRecognition-AI-at-night-to-control-switching-of-RoadLamps-to-MinimizePowerConsumption
Collecting videos of traffic at night which is processed using vehicle detection model to obtain relevant traffic frequency dataset which is preprocessed before feeding it into traffic_frequency_prediction model.  this traffic_frequency_prediction model is implemented using tensorflow which is further deployed on raspberry pi with movidius neural compute stick to control street lights in real time.

WHY?

I choosed this topic as this is one of the underlooked field that has the capability to shape the world in a new direction.

There is no proper infrastructure available for implementation of this idea. To implement this, a new control system need to be designed and implemented for proper functioning.

IMPLEMENTATION:

Collecting videos of traffic at night which is processed using vehicle detection model to obtain relevant traffic frequency dataset which is preprocessed before feeding it into traffic_frequency_prediction model.

this traffic_frequency_prediction model is implemented using tensorflow which is further deployed on raspberry pi with movidius neural compute stick to control street lights in real time.

CONCLUSION:

This is unexplored area of energy consumption which is underlooked and have a lot of potential to implement these kind of solutions solved using machine learning.

FUTURE SCOPE:

The idea and strategies can be implemented for person's safety and epidemics with same infrastructure established for this project.

Question / Proposal
There is lot of energy going waste by street lights glowing throughtout the city for whole night even though there might not be any traffic.

This energy wastage can be prevented by controlling street lights according to traffic frequency

Research
PAST DESIGN:

An idea already proposed goes as collecting data from sensors wheather vehicle is present or not and on that basis switching action is done on street lights. Although this implement the desired idea but it has many drawbacks: the sensors need to be installed throughout the street which leads to costly implementation and maintainence.The regular switching of street lights may affect life span of the lights.

PRESENT DESIGN:

In this a simple model deployed on rasberry pi using movidius is used to control the brightness of the lights. Hence  with very minimal hardware requirement and almost no mantainence power can be saved. 

Method / Testing and Redesign
The obtain data is processed in different batches according to timestamp associted with that data.

A batch contains time duration and number of vehicles on street during that interval.

A long sequence of these batches is fed to sequence detection deep learning model(LSTM) to analyse relevant patterns and hence training a model for the same.

 

To train this model data was collected from a  long sequence of traffic videos, which after training gives expected performance and accuracy.



Results
The model implemented for this project when presented with a new testing data, it performs very well at detecting sequences and improving itself with time. 

When trained using simple machine learning model like SVMs, Decision trees it outperformed initial deep learning model but with more data and training deep learning model achieved the highest desired accuracy.

Conclusion
The proposed solution is working well at detecting traffic congestion hence controlling street lights. Since model is designed to learn sequences overtime and also from the rewards it gains for its performance.

This project was experimented on real time data but on a small scale, on a larger scale its performance is still questionable and may require furter improvements.

This will lead to more unexplored regions where there might be scope of energy preservation or else they might be left unexplored.


