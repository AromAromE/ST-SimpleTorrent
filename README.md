# My First P2P File Sharing Project 🚀  

This is my **first personal project**, where I’m exploring how **peer-to-peer (P2P) file sharing** works. I wanted to build something simple yet functional, inspired by how BitTorrent splits files into chunks and distributes them among peers.  

## 📌 Features  
- 📡 **Peer-to-peer file transfer** without a central server  
- 📂 **File splitting & chunk-based downloading** for efficiency  
- 🔗 **Basic peer discovery** using a tracker server  
- ⏸ **Resumable downloads** so you don’t lose progress  

## 🛠 How It Works  
1. A **tracker server** keeps a list of peers with available files.  
2. Peers can **register** with the tracker and share file chunks.  
3. When a peer requests a file, the tracker helps it **find other peers**.  
4. The file is downloaded **in chunks from multiple peers**, then reassembled.  

## 🎯 Why I Built This  
I’ve always been curious about how P2P networks work, so I decided to **learn by doing**! This project helped me understand **networking, sockets, and file transfer** in Python. It's far from perfect, but it's a start!  

## 🔧 Setup & Usage  
### **1️⃣ Clone the Repository**  
```bash
git clone https://github.com/yourusername/ST-SimpleTorrent.git  
cd ST-SimpleTorrent  
