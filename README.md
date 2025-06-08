## Push logs manually
```
sudo systemctl start sawc-git-log-commit.service
# Debug
sudo journalctl -u git-log-commit.service -f
```

## Check timer status
```
sudo systemctl status sawc-git-log-commit.timer
sudo systemctl list-timers sawc-git-log-commit.timer
```

## Change timer
```
sudo vim /etc/systemd/system/sawc-git-log-commit.timer
sudo systemctl daemon-reload
```

