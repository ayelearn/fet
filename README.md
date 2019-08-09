# fet
Future Engineers' Training

Baseline commit id c5e913e043b46e491e6ddf7e1ac93fbc5481270c

Find populated wiki.md
(find -L . -maxdepth 2 -type f | grep wiki.md  | xargs grep https) 2>/dev/null | grep ":The following" | awk -F':' '{print $1}'

