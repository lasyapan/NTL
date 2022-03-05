
# Website for NTL Hackathon Project

 
- Our project uses sensors to detect data like pulse rate, temperature, air quality or location coords. 
- The SIM900 GSM Module allows it to send data over a network. 
- It sends a request to the website, updates it in SQLite and redirects back to the main page.
- Every few seconds, the website refreshes and displays latest data.

This is the website part of the project, made with Flask. The ugly CSS is by yours truly. 

# [Click here to look at it](https://ntl-2022.herokuapp.com/)
The link won't really update anything because the GSM module needs to communicate with it, but if you want to see how it works, you could just send something like this and wait for the webpage to refresh:

   ```https://ntl-2022.herokuapp.com/update/PULSE=<value>/TEMP=<value>/MQ135=<value>/MQ9=<value>/LOC=<value>```
   
   LOC should ideally be longitudinal and latitudinal coords separated with a  `,`. 
   
 It will do something like this:

![gif (2)](https://user-images.githubusercontent.com/62711442/156856257-37620cdd-dbad-490d-a924-64e1daa21c03.gif)

I  want to get rid of refreshing every n seconds (because it makes me think I've given myself a virus or something) and try doing something else, so I'll revist this when I've learnt javascript.

