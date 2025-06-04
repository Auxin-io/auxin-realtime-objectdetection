# Auxin Security Real-Time Object Detection demo

![demo](./demo.png)

This repository is a simple demo for how to use llama server with SmolVLM 500M to get real-time object detection

## How to setup

1. Install [llama.cpp](https://github.com/ggml-org/llama.cpp) or you can use Auxin Security llama server(https://llama-server.auxin.cloud)
2. Run `llama-server -hf ggml-org/SmolVLM-500M-Instruct-GGUF`  
   Note: you may need to add `-ngl 99` to enable GPU (if you are using NVidia/AMD/Intel GPU)  
   Note (2): You can also try other models [here](https://github.com/ggml-org/llama.cpp/blob/master/docs/multimodal.md)
3. Open `index.html` and replace the Base API value with the Auxin Security llama server URL(https://llama-server.auxin.cloud)
4. Optionally change the instruction (for example, make it returns JSON)
5. Click on "Start" and enjoy
