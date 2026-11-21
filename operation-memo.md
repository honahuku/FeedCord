```bash
# ※先に appsettings.json を編集しておく

# 反映
sudo systemctl restart feedcord.service
# たまに無効な json を書いちゃうことがあるので status を確認しておく
sudo systemctl status feedcord.service

# 10分前からのログを新しい順に表示
journalctl -u feedcord.service --since "10 min ago" -e


```
