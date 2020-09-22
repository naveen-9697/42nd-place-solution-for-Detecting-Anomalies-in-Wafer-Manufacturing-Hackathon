# 42nd place solution for "Detecting Anomalies in Wafer Manufacturing Hackathon"
link to hackathon: https://www.machinehack.com/hackathons/detecting_anomalies_in_wafer_manufacturing_weekend_hackathon_18

## A Brief Story of what has worked and what didn't:<br>
1. since the data was anonymised, all the techniques I had used to comprehend what's actually in the columns of the data was to no avail. Also the fact that the almost every column was binary only added the fuel.
2. So, I introduced polynomial interactions between the three continuous features, which actually gave me better results.
3. Using custom class weights for each class helped hugely.
4. I had learned the presence of skew in the continuous features during my initial data understanding; and treatment of which didn't work and further more results were very very bad.
5. A LightGBM with some tuned parameters and some that I usually use pushed me up on the leaderboard.

## On leaderboard:
<img src= ".images/leaderboard-position-screengrab.jpg" alt="my postition on leaderboard"/>

## Final Result on Public set:
AUroC= 0.82997 on test data of MachineHack.