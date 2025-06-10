 # 🧠 Dria Node Setup Guide (Ollama/Gemini)

## ✅ Pre-requirements

➡️ Minimum requirement to run this node:
8vCPU & 16 GB RAM

➡️ You can use GCP VPS to run this node.
Check this guide [how to setup Google Cloud VPS](https://github.com/rdkrr731/GCP-VPS-Setup.git)

## 🔹 Install Ollama (Choose your OS)

Download from:  
👉 [https://ollama.com/download/linux](https://ollama.com/download/linux)

![image](https://github.com/user-attachments/assets/5f53f1e0-b113-417b-b4a6-10cebbc6a6be)


## 🔹Download For Linux
```
curl -fsSL https://ollama.com/install.sh | sh
```

![image](https://github.com/user-attachments/assets/550ae3d3-c47a-4084-a3f5-fa30a61900ba)


## 🔹Verify Installation
```
ollama --version
```


## 🔹Launch Dria 
[You will need to open another terminal or restart your same terminal after launch dria step]
```
curl -fsSL https://dria.co/launcher | bash
```
Image
![image](https://github.com/user-attachments/assets/d3f6d489-4273-431d-a154-e8da6b0f204b)



## 🔹Start your Node
(You'll be prompted to enter your EVM private key (without 0x) and choose the model.)
```
dkn-compute-launcher start
```
Image
![image](https://github.com/user-attachments/assets/eb0b4786-6d87-4b7c-a41d-83eb344976d3)



## 🤖Select your model accordinly🤖

![image](https://github.com/user-attachments/assets/a8a6667e-816a-418e-9604-f69cf2dea30f)

Select Model with Spacebar key & Enter key to confirm or back
You can check here which model is suitable for your system. 👇

https://node-guide.dria.co/selecting-models

![image](https://github.com/user-attachments/assets/c5da7706-3b73-49d0-a099-235fff6a2f9b)


### 📊 Check Node Status & Points

👉 Check your node status [https://dria.co/edge-ai/my-node]

![image](https://github.com/user-attachments/assets/19d433c7-3001-4c36-9832-f069ba14aa00)

### 📝 Join Discord Server & Fill this Form to Get Discord Role

Discord: https://discord.gg/DAkhTKDD

👉 [https://form.typeform.com/to/Eav42hR3?typeform-source=www.google.com]


## 🔄 Switching from Ollama to Gemini API
Recommended for devices not capable of running Ollama or if Ollama is not working.

1. Stop your node if it's running
   Press Ctrl+C
3. Delete your Dria directory:
```
sudo rm -rf .dria
```
3. Reinstall the Dria launcher
(Use installation commands from above depending on your OS)

4. Start your node
```
dkn-compute-launcher start
```
5. Select Gemini instead of Ollama
   
6. Choose a Model:
  - gemini-1.5-flash

  - gemini-1.5-pro

7. Enter your Gemini API Key
👉 Get it from:
https://aistudio.google.com/app/apikey


## TIPS ⚒️⭐

1. Install tmux on your VPS:
```
sudo apt update
sudo apt install tmux
```
2. Start a new tmux session:
```
tmux new -s mynode
```
3. Run your node inside the tmux session
(Download dria, launch dria & start running node)

4. Once your node is active & running, Detach from tmux (leave the session running):
```Press Ctrl+B, then D```

5. Return back to tmux session
   ```
   tmux attach -t mynode
   ```
