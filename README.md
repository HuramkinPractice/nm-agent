Fork from https://github.com/nodequery/nq-agent


## Start

```
curl -fsSL https://raw.githubusercontent.com/HuramkinPractice/nm-agent/refs/heads/main/nm-install.sh -o nm-install.sh
chmod +x nm-install.sh
./nm-install.sh <TOKEN> https://example.com
```

## Uninstall

```
rm -rf /etc/nodemonitor && (crontab -u nodemonitor -l | grep -v "/etc/nodemonitor/nq-agent.sh") | crontab -u nodemonitor - && userdel nodemonitor
```
