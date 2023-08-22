# Linux Important Files

## Useful User Information

```bash
user/passwd
```

## User Password Hashes

```bash
/etc/shadow (Unshadowing tool + JohntheRipper or Hashcat)
```

## Important Log Files

```bash
/var/logs (failed sudo goes here)
```

## Sudo Config File

* used to control the sudo permissions of every user on the system

```bash
/etc/sudoers
```

### **Certain Machines You Cannot Edit Sudoers File Without an Interactive Shell. Here is a Workaround**

```bash
echo "username ALL=(ALL) ALL" >> /etc/sudoers
```

## All Processes Stored in Proc

```bash
/proc/[pid]
```

## Place to Install Custom Tools from Github etc.

```bash
/opt
```
