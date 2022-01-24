# Pulseaudio Echo/Noise Cancellation
Enable echo or noise cancellation of microphone input on linux desktop.

## Add the following line in terminal
```
sudo vim /etc/pulse/default.pa
```
or
```
sudo nano /etc/pulse/default.pa
```

## Put it after the line "Modules to allow autoloading of filters (such as echo cancellation)" 
```
load-module module-echo-cancel
```

## Reload PulseAudio on the terminal "pulseaudio -k" 
You should be able to select the new Noise Cancellation option from the Input Device Section.
