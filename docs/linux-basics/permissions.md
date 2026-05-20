1️⃣ drwxrwxr-x (Permission Format)

👉 Shows type + permissions (user, group, others)

d = directory (- = file)
rwx = read, write, execute

Breakdown:

drwxrwxr-x
│ │ │ │ │ │ │ │ │
│ │ │ └──── group (rwx)
│ └──────── user (rwx)
└────────── type (d = directory)
2️⃣ ls

👉 Lists files and directories.

Syntax:

ls

Example:

ls
3️⃣ ls -l

👉 Shows detailed file info (permissions, owner, size).

Syntax:

ls -l

Example:

ls -l
4️⃣ chmod

👉 Changes file permissions.

Syntax:

chmod [permissions] file

Example:

chmod 755 script.sh
chmod 766 <file.name>
5️⃣ umask

👉 Sets default permission for new files.

Syntax:

umask [value]

Example:

umask 022
6️⃣ chown

👉 Changes file owner.

Syntax:

chown user file

Example:

sudo chown krishna file.txt
7️⃣ chgrp

👉 Changes group ownership.

Syntax:

chgrp group file

Example:

chgrp dev file.txt
8️⃣ zip

👉 Compress files into .zip.

Syntax:

zip file.zip file

Example:

zip files.zip file1.txt file2.txt
9️⃣ tar

👉 Archive/compress files.

Syntax:

tar [options] file.tar files

Example:

tar -cvf archive.tar folder/
🔟 scp

👉 Securely copy files between systems.

Syntax:

scp file user@host:path

Example:

scp file.txt user@192.168.1.1:/home/user/
1️⃣1️⃣ rsync

👉 Fast file transfer & sync (efficient).

Syntax:

rsync [options] source destination

Example:

rsync -av folder/ user@host:/backup/
