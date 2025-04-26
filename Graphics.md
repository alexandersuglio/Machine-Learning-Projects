🔧 **Physical Server** (in AWS Data Center)  
│  
├── 🧠 **Hypervisor** (e.g. Nitro or Xen)  
│   ├── 💻 **EC2 Instance A** — `t3.micro`  
│   │   └── 🐧 Ubuntu OS  
│   │       └── 🐳 Docker Engine  
│   │           ├── 🌐 Web Container (NGINX)  
│   │           ├── ⚙️ App Container (Node.js)  
│   │           └── 🛢️ DB Container (PostgreSQL)  
│   ├── 💻 **EC2 Instance B** — `m5.large`  
│   └── 💻 **EC2 Instance C** — `c5.xlarge`  
