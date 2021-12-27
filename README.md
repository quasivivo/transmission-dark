# transmission-dark
An alternate dark theme for the transmission torrent client

# Installation

Find/update your transmission installation's web UI folder in the command below. Typically: /usr/share/transmission/web/

```
cd /usr/share/transmission/web/ &&
wget https://raw.githubusercontent.com/quasivivo/transmission-dark/main/common.css -O /tmp/transdark.css &&
mv /tmp/transdark.css ./style/transmission/dark.css &&
sed -i 's/common.css/dark.css/' ./index.html
```

sudo if necessary.

To revert:

```
cd /usr/share/transmission/web/ &&
rm ./style/transmission/dark.css &&
sed -i 's/dark.css/common.css/' ./index.html
```
