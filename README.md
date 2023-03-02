# audio4dj-mixxx-configs
alsa configs to use mixxx with Native Instruments Audio4DJ USB interface 2 ouputs, vinyl control

# Setup
fist put the `.asoundrc` to your home folder  
`mv .asoundrc ~`  
this will create alsa audio devices called:   
outDJA channels 1-2  
outDJB channels 1-2  

# Mixxx setup
when you are using external mixer there's no master output so leave it empty

set DJA and DJB channels for deck 1 and deck 2 outputs  

for vinyl control you set the same:  
outDJA channels 1-2  
outDJB channels 1-2  

note:
inputs should be called inDJA and inDJB but they might not be visible in mixxx, but they seem to work just fine.  

# starting mixxx  
first run this:   
`export PA_ALSA_PLUGHW=1`  
this should create the audio devices for you. 

if you are using pulseaudio you need to disable it  
pulseaudio --kill  
or you can try  
pasuspender mixxx  

# disable pulseaudio autospawn (optional)
edit /etc/pulse/client.conf  
and set `autospawn = no`  

# changing modes  
haven't tested this yet... 

