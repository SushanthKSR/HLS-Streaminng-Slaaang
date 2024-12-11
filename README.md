#Adaptive Bit Rate (ABR) Streaming
Adaptive Bit Rate (ABR) streaming is a technique used in video delivery that dynamically adjusts the quality of the video stream based on the user’s network conditions and device capabilities. It ensures smooth playback and optimizes the viewer's experience by balancing quality and loading speed.

<img width="573" alt="Screenshot 2024-12-12 at 3 36 58 AM" src="https://github.com/user-attachments/assets/f6cb4076-a465-4151-9f75-04d95b415947" />

##How It Works
1. Video Encoding
The source video is encoded into multiple versions, each at a different quality and bitrate.
Common encoding resolutions: 240p, 360p, 480p, 720p, 1080p, etc.

2. Segmenting
Each version of the video is divided into small chunks or segments (e.g., 2-10 seconds each).
These segments are stored on a streaming server, ready for delivery.
<img width="228" alt="Screenshot 2024-12-12 at 3 36 05 AM" src="https://github.com/user-attachments/assets/3e8fa39c-cf5d-427f-bca8-e0de6bff5168" />

4. Manifest Files
A manifest file (e.g., M3U8 or MPD) is generated, listing all available streams and their corresponding bitrates and resolutions.
The player uses this manifest to determine available video options.

5. Client-Side Adaptation
The video player starts streaming at the optimal quality based on initial network conditions.
If the network improves, the player seamlessly switches to a higher-quality stream.
If the network deteriorates, the player switches to a lower-quality stream to prevent buffering.

6. Seamless Playback
By switching between streams dynamically, the user experiences continuous playback with minimal interruptions, even under fluctuating network conditions.
