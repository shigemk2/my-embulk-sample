# my-embulk-sample
## Install

```sh
curl --create-dirs -o ~/.embulk/bin/embulk -L "http://dl.embulk.org/embulk-latest.jar"
chmod +x ~/.embulk/bin/embulk
echo 'export PATH="$HOME/.embulk/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## Fist

```sh
embulk example ./try1
embulk guess   ./try1/seed.yml -o config.yml
embulk preview config.yml
embulk run     config.yml
```
