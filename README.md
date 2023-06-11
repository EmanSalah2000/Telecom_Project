# Telecom_Project
My project is to detect the crawded data in the specefic area with some features
1. read data 
    1. Traffic_volume data  before proccessing 
    https://docs.google.com/spreadsheets/d/1wWmAbokmI8TVoruv7x8PsYaHl9kqpGYg/edit?usp=sharing&ouid=111070117771916953975&    rtpof=true&sd=true  
        1. timestamp to detect the time of the user
        2. LocationLatitude and LocationLongitude to detect the postion of the user 
        3. RadioOperatorName to detect the operator of the user
        4. TrafficDirection to detect if up link [ from mobile to tower] or down link [from tower to mobile]
        5. TrafficVolume to check the volume of the users 

   2. RSRP data before proccessing 
     https://drive.google.com/file/d/1csBKhhQZd1RGF5URzkpghIELrh0yWmiD/view?usp=sharing
      1. RSRP to measure the quality of signal
      2. DeviceManufacturer and DeviceName to check the type and the name of the device

2. proccessing data 
    1. convert time and reomve unuse data 
    2. mobile not wifi 
    3. Enabled not notEnabled
    4. 4G not [2G, 3G]
    5. removing outliers from RSRP
    6. merge Traffic_volume data  and RSRP

3. visualize data
   1. time-lapse to visually the users activity through days and hours with opertator name
   2. Heat-Map to visually the RSRP value with operator name
   3. Bar Chart to measure [Sum , Average , Minimum , maximum , count , percentage of 90] of RSRP for each operator for each    device


4. machine learning part
   split data to uplink and downlink  then split each part to [Operator A , Operator B , Operator C]
   
   
   1.Linear Regression
    X will RSRP to chceck  Y the Traffic Volume
     
   3.Time Series 
    through the days and the hours measure the traffic volume and ARIMA series to predict the next stage
    


