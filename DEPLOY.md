## ð§ Deploy (Ubuntu) / ããã­ã¤ï¼Ubuntuï¼

### 1. Installing Node.js / Node.jsãã¤ã³ã¹ãã¼ã«
```bash
curl -fsSL https://deb.nodesource.com/setup_16.x | bash -
sudo apt install -y nodejs
```

### 2. Downloading Syaberunoda / ããã¹ãã®ã ããã¦ã³ã­ã¼ã

```bash
git clone https://github.com/Tailmc/Syaberunoda.git
cd Syaberunoda
npm install
```

### 3. Creating an ENV file / ENVãã¡ã¤ã«ãä½æ

```bash
nano .env
```
Format / å½¢å¼

```
TOKEN=[TOKEN]
prefix=[PREFIX]
deepl=[DeepL API KEY]
mongodb=[MongoDB URI]
voicevox=[Su-shiki API KEY]
```

How do i get these variables? / ãããã®å¤æ°ã®å¥ææ¹æ³

[TOKEN]https://discord.com/developers

[PREFIX], for example ! , ?

[DeepL API KEY]https://www.deepl.com/docs-api

[MongoDB URI]https://www.mongodb.com/docs/atlas/

[Su-shiki API KEY]https://su-shiki.com/api/

### 4. Installing PM2 & Launch! / PM2ãã¤ã³ã¹ãã¼ã«ãã¦èµ·å
```bash
sudo npm install pm2 -g
pm2 start app.js
```
