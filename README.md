# curator-elasticsearch
Remove elasticsearch indices using curator


1) Install Python pip
```
sudo apt-get install python-pip
```

2) Install Curator
```
sudo pip install elasticsearch-curator
```

3.) Create new directory for config-files
```
mkdir curator
cd curator
touch config.yml
```

dry-run
```
curator --config /root/curator/config.yml --dry-run /root/curator/actions.yml
```

run
```
0 2 */2 * * curator --config /root/curator/config.yml /root/curator/actions.yml
```
