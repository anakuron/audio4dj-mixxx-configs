# audio4dj-mixxx-configs
alsa configs to use mixxx with Native Instruments Audio4DJ USB interface 2 ouputs, vinyl control

# put the .asoundrc to your home folder  
this will create alsa audio devices called:   
outDJA channels 1-2  
outDJB channels 1-2  

set these for deck 1 and deck 2 outputs  

for vinyl control you set the same:  
outDJA channels 1-2  
outDJB channels 1-2  

inputs should be called inDJA and inDJB but for whatever reason they are not visible in mixxx, but they seem to work just fine.  

# starting mixxx  
if you are using pulseaudio you need to disable it  
pulseaudio --kill  
or you can try  
pasuspender mixxx  

# disable pulseaudio autospawn (optional)
edit /etc/pulse/client.conf  
and set autospawn = no  

#changing modes  
haven't tested this yet...  

