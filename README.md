1. Start socat. It is used for emulation of transport disconnects

`socat -d TCP-LISTEN:8001,fork,reuseaddr TCP:localhost:8000`

2. start `ResumeFileTransfer.main`

3. terminate/start socat periodically for session resumption

`ResumeFileTransfer` output is nil
