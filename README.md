# Auxin Security Real-Time Object Detection demo

![demo](./demo.png)

This repository is a simple demo for how to use the llama server with SmolVLM 500M to get real-time object detection.

## How to setup

1. Clone the repository
   ```sh
   git clone https://github.com/Auxin-io/auxin-realtime-objectdetection
   ```
3. Host your llama server by installing [llama.cpp](https://github.com/ggml-org/llama.cpp) -- instead of building your own server from scatch run the binary for your platform. At time we have our llamma server running but not alwasy. Our server runs at https://llama-server.auxin.cloud - Best to run your server locall https://github.com/ggml-org/llama.cpp/blob/master/tools/server/README.md
4. Run `llama-server -hf ggml-org/SmolVLM-500M-Instruct-GGUF`
   Note: you may need to add `-ngl 99` to enable GPU (if you are using NVidia/AMD/Intel GPU)  
   Note (2): You can also try other models [here](https://github.com/ggml-org/llama.cpp/blob/master/docs/multimodal.md)
   Note (3): If you host a llama server, then you need to follow step #4; otherwise, you can skip it
6. Open `index.html` and replace the Base API value with the your or ours llama server URL
7. Click on "Start" and enjoy
