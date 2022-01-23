# Introduction: What we do here
- Kind anything that you can measure, from installing sensors -> gathering data -> analysis and monitoring -> final result
- lot of different project, also more "simple" (stream of data and then analysis)

# General workflow
1. senors gathers data
1.1. they are stored in the cabinet
1.2. backup system -> database AWS .bin (raw but there might be very simple processing) -> labeld data (x,y,z or channel)
1.3. 10 minutes of data (but i could be more)
2. lambda calcus  
2.1. aggregation and processing (it can specify where the sensor is located) -> send the influxedb.
3. time series DB timestamp: column1 ... text()
3.1 you can have different measurement, one for each kind data.
3.2 text is important, it defines data stream
3.3 three database (RAW, FAT(temp, keep it clean), Derived (all measurement derived)
4. python scripts -> checkout
4.1 commit on my branch and then do pull request
4.2 crontab sch
5. graphana, for visualizing time series is the best; limited with scatter plot and histogram 
6. brewery -> it's already ready to go
6.1 python scripts for server
6.2 write on /work for stupid scripts, on /share for more serious stuff.
6.3 clone the repo -> create new branch -> checkout -> pull request 



