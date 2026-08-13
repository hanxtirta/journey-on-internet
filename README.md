Hybrid Bug Bounty Hunting Two Viewpoint With Caido AI Agent

kombinasi antara 
Caido sebagai Proxy interceptor + ai agent claude + kode editor cursor

1. Clone repository
Buka terminal, lalu clone repo caido-mcp-server versi v1.1.0:
`git clone --branch v1.1.0 https://github.com/c0tton-fluff/caido-mcp-server.git`

2. Masuk ke folder proyek
Pindah ke direktori hasil clone:
`cd caido-mcp-server`

3. Compile server
Butuh Go terinstall. Di macOS/Linux jalankan
`go build -o caido-mcp-server .`
— di Windows jalankan
`go build -o caido-mcp-server.exe .`

4. Jalankan Caido & login server
Pastikan Caido sudah berjalan (default di http://127.0.0.1:8080),
lalu jalankan
`caido-mcp-server login -u http://127.0.0.1:8080`
(Windows: `./caido-mcp-server.exe login -u http://127.0.0.1:8080`).
Ini akan membuka dialog OAuth di Caido — klik tombol Allow untuk mengotorisasi server.

5. Konfigurasi MCP client (Claude CLI)
