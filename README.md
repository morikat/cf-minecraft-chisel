# cloudfoundry-minecraft

## Usage

### application push
```bash
$ git clone https://github.com/morikat/cf-minecraft-chisel
$ cd cf-minecraft-chisel
$ echo 'eula=true' > eula.txt
$ cf push minecraft-app
```

### run chisel client

```bash
$ ./chisel-bin/chisel_linux_amd64 client -v --keep alive 3s http://minecraft-app.mybluemix.net 25565:127.0.0.1:25565

2015/05/10 14:58:43 client: Connecting to ws://minecraft-app.mybluemix.net:80
2015/05/10 14:58:43 client: 127.0.0.1:25565#1: Enabled
2015/05/10 14:58:44 client: Fingerprint 87:75:1e:6b:fb:e7:8a:d4:99:3c:27:25:0a:db:d4:3a
2015/05/10 14:58:44 client: Sending configurating
2015/05/10 14:58:44 client: Connected (Latency 169.971531ms)
2015/05/10 14:59:42 client: 127.0.0.1:25565#1: conn#1: Open
2015/05/10 14:59:42 client: 127.0.0.1:25565#1: conn#1: Close (sent 32 received 0)
2015/05/10 15:00:25 client: 127.0.0.1:25565#1: conn#2: Open
2015/05/10 15:02:39 client: 127.0.0.1:25565#1: conn#2: Close (sent 20753 received 0)

```
