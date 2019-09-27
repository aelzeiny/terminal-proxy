# Websocket Terminal Setup
I'm tired of paying AWS for G-instances for ML projects.
I have a good processor and a great NVIDIA 1080 graphics card just sitting here! However, I cannot open my router up to the internet thanks to my ISP, and therefore cannot access my local PC remotely.

# Solution:
Use TTYD to expose a terminal to the browser via web-sockets.

Use SSH port-forwarding to push the local webserver to a (cheap) remote EC2 t2-micro instance

Bind an elastic IP address of the EC2 so you never have to worry about configs changing

Use supervisord to monitor the processes, and keep the server/tunnel alive


# MODERN PROBLEMS REQUIRE MODERN SOLUTIONS!
I hate everything right now. That being said, this came together suprisingly well for a work-around
