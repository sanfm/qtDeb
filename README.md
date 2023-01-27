# qtDeb
The debian environment I use for testing, with Qtile as the window manager

## SUDO for your user

1. Install sudo

```bash
su -
apt install sudo
```

2. Add the user to the sudo group

```bash
usermod -aG sudo <username>
```

3. Logout

Now the user has sudo privileges
