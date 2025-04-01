# ST-SimpleTorrent 🚀  

This is my **first personal project**, where I’m exploring how **peer-to-peer (P2P) file sharing** works. I wanted to build something simple yet functional, inspired by how BitTorrent splits files into chunks and distributes them among peers.  

## 📌 Features  
- 📡 **Peer-to-peer file transfer** without a central server  
- 📂 **File splitting & chunk-based downloading** for efficiency  
- 🔗 **Basic peer discovery** using a tracker server  
- ⏸ **Resumable downloads** so you don’t lose progress  

## 🛠 How It Works  
1. A **tracker server** keeps a list of peers with available files.  
2. Peers **register** with the tracker and share file chunks.  
3. When a peer requests a file, the tracker helps it **find other peers**.  
4. The file is downloaded **in chunks from multiple peers**, then reassembled.  

## 🎯 Why I Built This  
I’ve always been curious about how P2P networks work, so I decided to **learn by doing**! This project helped me understand **networking, sockets, and file transfer** in Python. It's far from perfect, but it's a start!  

## 🚀 Next Steps  
- Add **better error handling** (e.g., handling disconnects)  
- Improve **peer discovery** (maybe try decentralized discovery like DHT)  
- Optimize **chunk request strategies** for faster downloads  

## 🔧 Setup & Usage  
### **1️⃣ Install Dependencies**  
Ensure you have Python 3 installed, then install required libraries (if any):  
```bash  
pip install -r requirements.txt  
```  

### **2️⃣ Clone the Repository**  
```bash  
git clone https://github.com/yourusername/ST-SimpleTorrent.git  
cd ST-SimpleTorrent  
```  

### **3️⃣ Start the Tracker Server**  
The tracker keeps track of available peers. Run this first:  
```bash  
python tracker.py  
```  

### **4️⃣ Start a Peer (Downloader/Seeder)**  
Peers can upload and download files. Open multiple peers in different terminals:  
```bash  
python peer.py --share example.txt  # Share a file  
python peer.py --download example.txt  # Download a file  
```  

### **5️⃣ Enjoy File Sharing!**  
Once peers are running, they will start exchanging file chunks automatically.  

## 📜 License  
This project is for **learning purposes only**. Feel free to use and improve it!  

