# MSCS-631-M50_PythonLab7
This lab will implement a streaming video server and client that communicate using the Real-Time Streaming Protocol (RTSP) and send data using the Real-time Transfer Protocol (RTP). Your task is to implement the RTSP protocol in the client and implement the RTP packetization in the server.

# Video Streaming Client-Server Application (RTSP/RTP)

## Overview
This project implements a video streaming application using the Real-Time Streaming Protocol (RTSP) for control messages and Real-Time Transport Protocol (RTP) for video data transfer. The client can send RTSP commands (`SETUP`, `PLAY`, `PAUSE`, `TEARDOWN`) to control video playback, while the server streams video frames as RTP packets.  

The video file used in this lab is `movie.Mjpeg`, stored as a sequence of JPEG images.

---

## Prerequisites

- **Python 3.12+**

## Running the Application
### 1. Start the server
```bash
python3 Server.py <server_port>
#EG: python3 Server.py 5544
```

### 2. Start the client
```bash
python3 ClientLauncher.py <server_host> <server_port> <RTP_port> <video_file>
#EG: python3 ClientLauncher.py localhost 5544 25000 movie.Mjpeg
```


