# Procedure for Automated Activation

We used a raspberryPi 4 with raspbian OS with an ethernet connection.
Invocation samples are generated using Amazon's TTS-Service Polly. 

1. Register alexa-account https://alexa.amazon.com
2. Enable `set-up mode` of the echo-device
    - We used a servo-motor attached to the echo device and controlled by the raspberryPi to press the physical button
3. Connect to the ad-hoc-wifi network
    - Add this network to 'preferred networks' to speed-up further runs
4. Follow the steps on alexa.amazon.com to set-up your echo-device
5. On the final video open the Firefox network-tab (`ctrl`+`shift`+`e`)
6. Copy the request to the `/cards`-Endpoint as "curl-command" in te next step
    - This request is used to fetch the activity-log after every run
7. Request speech samples `aws polly synthesize-speech  --text "$Invocation" --voice Salli --output-format ogg_vorbis "$Invocation.ogg"`
8. Run test
    - Play Invocation
    - Stop and Exit Skill
    - Record activity-log
