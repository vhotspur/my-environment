# My mini scripts

Add path to this directory to `$PATH`.


## `absfilename`

Print absolute file path (pass as parameter).

## `baterka`

Print battery percentage from `upower -d`.

## `eclo`

Open files given as arguments in Eclipse.

## `gs-embed-fonts`

Embed all used fonts into PDF via GhostScript (useful for PDF
publications at ACM or IEEE).

## `opdf`

Run `atril` in background with given file.


## `vagrant-ansible-playbook`

Run given Ansible playbook on given Vagrant machine.


## `proxy-switcher-server`

```
mkdir -p ~/.config/systemd/user/
cat <<EOF >~/.config/systemd/user/proxy-switcher.service
[Unit]
Description=Smart proxy switcher server

[Service]
ExecStart=$PWD/proxy-switcher-server start

[Install]
WantedBy=default.target

EOF
systemctl --user daemon-reload
systemctl --user start proxy-switcher.service
systemctl --user enable proxy-switcher.service
systemctl --user status proxy-switcher.service
```
