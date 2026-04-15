1️⃣ grep

👉 Searches for a pattern in file/content.

Syntax:

grep [options] "pattern" file

Example:

grep "error" log.txt

👉 Finds lines containing "error"

🔹 Common options
grep -i "error" file.txt   # ignore case
grep -n "error" file.txt   # show line number
grep -r "error" /path      # search recursively
grep -v "error" file.txt   # exclude pattern
2️⃣ egrep (Extended grep)

👉 Supports advanced patterns (regex like |, +, ?)

Syntax:

egrep "pattern" file

Example:

egrep "error|fail" log.txt

👉 Matches "error" OR "fail"

⚠️ Important

👉 egrep = same as:

grep -E

✔ Modern usage:

grep -E "error|fail" log.txt
3️⃣ fgrep

👉 Searches exact string (no regex)

Syntax:

fgrep "text" file

👉 Modern:

grep -F "text" file
4️⃣ grep -c

👉 Counts matching lines

Example:

grep -c "error" log.txt
5️⃣ grep -l

👉 Shows file names containing match

grep -l "error" *.log
6️⃣ grep -w

👉 Matches whole word only

grep -w "error" file.txt
7️⃣ grep -A / -B / -C

👉 Shows context lines

grep -A 2 "error" log.txt   # after
grep -B 2 "error" log.txt   # before
grep -C 2 "error" log.txt   # both
8️⃣ Pipe with grep (VERY IMPORTANT 🔥)

👉 Combine with other commands

ps aux | grep nginx
cat log.txt | grep error
9️⃣ Regex examples
grep "^a" file.txt   # starts with 'a'
grep "end$" file.txt # ends with 'end'
grep "[0-9]" file.txt # numbers
🔥 Pro Notes (Must Know)
grep = basic search
grep -E = advanced (replace egrep)
grep -F = exact match
Pipes (|) = real DevOps usage

Logs check:
tail -f app.log | grep error
Process check:
ps aux | grep docker
File search:
grep -r "password" /etc