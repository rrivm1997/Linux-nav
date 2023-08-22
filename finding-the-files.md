# Finding Files

## locate

* works fast because it runs on internal database

```bash
sudo updatedb
locate filename
```

## find

* slower than locate, but more thorough
* uses regex

### **Sends all Permission Denied to Null**

```bash
find / -name file 2>dev/null
```

### **Finds Directories Owned by a Group**

```bash
find dir -group groupname
```

### **Find Files Owned by a User**

```bash
find / -user username 2>/dev/null
```

### **Find Files with SUID Permissions**

```bash
find / -perm -u=s -type f 2>/dev/null
```

```bash
find / -user root -perm -4000 -exec ls -ldb {} \; 2>/dev/null
```

## which

* outputs the path of the binary that you are looking for
* searches through directories defined in the $PATH variable

```bash
which bash
```

```bash
which python
```
