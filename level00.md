# Commands Used:

### To find UID from username "flag00"

```bash
id -u flag00 # == 999
```
[find uid from username](https://kb.iu.edu/d/adwf)

### To find files linked to UID:

```bash

find <name_of_directory> -uid 999

```

[find files linked to UID](https://www.unixtutorial.org/find-files-which-belong-to-a-user-or-unix-group/)

### To find only executable files:

```bash

find -executable -type f -uid 999 # ==./flag00 running in /bin

```

### Thoughts:

- It took us ages, even though we were running the correct command, to actually notice that the "suspicious" directory was **"..."**. We now know that we shouldn't just glance over the names of the directories or files in general but must be more careful. We saw dot-dot-dot as _dot-dot_ and thought it was the folder in /home/flag00.
