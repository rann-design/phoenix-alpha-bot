# 🤖 PHOENIX BOT— Discord Crypto Research Assistant

Bot Discord yang bisa riset crypto secara otomatis — airdrop terbaru, fundraising, sentimen sosial, dan proyek trending — pakai AI agent yang manggil tool-nya sendiri.

## ✨ Fitur

- **`/alpha`** atau **`!alpha`** — cari airdrop crypto terbaru, tampil sebagai card interaktif
- **Chat bebas** — tanya apa saja soal crypto, bot otomatis riset lewat beberapa sumber data
- **Auto-update** — kirim info airdrop otomatis secara berkala (`/start` untuk aktifkan, `/stop` untuk berhenti)
- **Emoji shortcut** — kirim 🔍 📈 atau 💰 buat trigger cepat tanpa command
- **Anti-halusinasi** — semua jawaban berdasarkan data asli dari Surf API, bukan karangan AI
- **Transparansi sumber** — setiap info nyantumin link sumber, atau bilang jujur kalau sumbernya tidak tersedia

## 🛠️ Tech Stack

| Komponen | Fungsi |
|---|---|
| [discord.py](https://discordpy.readthedocs.io/) | Interface Discord bot |
| [Groq](https://groq.com/) (Llama 3.1) | AI agent — mutusin tool mana yang dipanggil |
| [Surf API](https://ask.surf) | Sumber data crypto real-time (airdrop, fundraising, sosial, dll) |

## 📦 Instalasi

### 1. Clone repo ini
```bash
git clone https://github.com/USERNAME/rann-bot-download.git
cd rann-bot-download
```

### 2. Install dependencies
```bash
pip install -U discord.py groq
```

### 3. Install Surf CLI
```bash
curl -fsSL https://downloads.asksurf.ai/cli/releases/install.sh | sh
export PATH="$HOME/.local/bin:$PATH"
surf auth --api-key SURF_API_KEY_KAMU
```

### 4. Siapkan environment variable
```bash
export DISCORD_TOKEN="token_bot_discord_kamu"
export GROQ_API_KEY="key_groq_kamu"
```

### 5. Jalankan bot
```bash
python rann-bot-discord.py
```

## ⚙️ Setup Bot Discord

1. Buat aplikasi di [discord.com/developers/applications](https://discord.com/developers/applications)
2. Tab **Bot** → aktifkan **MESSAGE CONTENT INTENT**
3. Tab **OAuth2 → URL Generator** → centang `bot` + `applications.commands`
4. Permission: `Send Messages`, `Read Message History`, `View Channels`
5. Invite bot pakai URL yang di-generate

## 📋 Command

| Command | Fungsi |
|---|---|
| `/alpha` atau `!alpha` | Cari airdrop terbaru |
| `/start` atau `!start` | Aktifkan update otomatis di channel ini |
| `/stop` atau `!stop` | Matikan update otomatis |

## ⚠️ Disclaimer

Semua data yang ditampilkan bot ini adalah agregasi dari sumber publik (Surf API) dan bersifat snapshot pada waktu tertentu — **bukan saran finansial**. Selalu DYOR (Do Your Own Research) sebelum mengambil keputusan finansial apa pun.

## 📄 Lisensi

Bebas dipakai & dimodifikasi untuk keperluan pribadi.

# MASIH TESTING 
