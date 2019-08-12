# fet
Future Engineers' Training

Baseline commit id c5e913e043b46e491e6ddf7e1ac93fbc5481270c

Find populated wiki.md
```
(find -L . -maxdepth 2 -type f | grep wiki.md  | xargs grep https) 2>/dev/null | grep ":The following" | awk -F':' '{print $1}'
```

Find unique topics
```
ls | tr '[A-Z]' '[a-z]' | tr -d '\-_' | sort -u
```
```
ls | tr '[A-Z]' '[a-z]' | tr -d '\-_' | sort -u | awk '/[^s]$/ {$x=$1; print $x "s";next};/./ {print $0}' | sort > a.txt
ls | tr '[A-Z]' '[a-z]' | tr -d '\-_' | sort -u | awk '/[^s]$/ {$x=$1; print $x "s";next};/./ {print $0}' | sort -u > b.txt
diff a.txt b.txt | grep "<" | cut -d' ' -f2
diff a.txt b.txt | grep "<" | cut -d' ' -f2 | wc -l
```

Find all refs to a topic
```
export topic="calculus"; find -L ../refs -type d 2>/dev/null | grep -i $topic | awk -F'/' '{print $4}' | sort -u
```

Clean up wiki.md
```
cat wiki.md | awk 'BEGIN {s=0; e=0};/^Jump_to/ {if (e==0) s=1; next};/./ {if (s==1 && e==0) {e=1; next} else {if (s==1 && e==1) print $0}}' | tr -s '*' | sed 's/â/-/g; s/i\.e\./that is/g; s/e\.g\./for example/g; s/et\ al\./et\ al/g; s/etc\./etc/g; s/\.)/)./g; s/\.\}/\}\./g; s/\.\]/\]\./g; s/\.\"/\"\./g; s/vs\./vs/g; s/\.\.\./~~~/g; s/[0-9]\./~/g; s/\[[0-9]*\]//g; s/\*\ /.\n~ /g; s/[^[:print:]]//g' | tr '\n' ' ' | awk -F'.' '/./ {for (i=1; i<=NF; i++) print $i"."}' | tr -s ' ' | sed 's/^\ //g; s/^\.$//g; s/\ \././g; s/\[edit\]//g; s/:\./ - /g; s/\*\./-/g; s/~~~/.../g' | grep -e '[a-z]' | awk '/^~\ Refer/ {exit};/./ {print}' | tr '_:~' ' \-\-' | perl -p -e 's/[^[:ascii:]]//g' | sed 's/&#x005E;/^/g; s/&#x00A8;/\"/g; s/&#x00D7;/\*/g; s/&#x02D9;/\`/g; s/&#x0393;/__Gamma/g; s/&#x03A8;/__Psi/g; s/&#x03B1;/__alpha/g; s/&#x03B2;/__beta/g; s/&#x03B3;/__gamma/g; s/&#x03B4;/__delta/g; s/&#x03B6;/__zeta/g; s/&#x03B8;/__theta/g; s/&#x03BC;/__mu/g; s/&#x03BE;/__xi/g; s/&#x03C4;/__tau/g; s/&#x03C6;/__chi/g; s/&#x03C9;/__omega/g; s/&#x03D5;/__Phi/g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g;' | less
```

Create plain text wiki mashup
```
srija@srija-Vostro-3446:~/gate2020/fet/topics$ for n in $(find . | grep wiki.md); do cat $n | awk 'BEGIN {s=0; e=0};/^Jump_to/ {if (e==0) s=1; next};/./ {if (s==1 && e==0) {e=1; next} else {if (s==1 && e==1) print $0}}' | tr -s '*' | sed 's/â/-/g; s/i\.e\./that is/g; s/e\.g\./for example/g; s/et\ al\./et\ al/g; s/etc\./etc/g; s/\.)/)./g; s/\.\}/\}\./g; s/\.\]/\]\./g; s/\.\"/\"\./g; s/vs\./vs/g; s/\.\.\./~~~/g; s/[0-9]\./~/g; s/\[[0-9]*\]//g; s/\*\ /.\n~ /g; s/[^[:print:]]//g' | tr '\n' ' ' | awk -F'.' '/./ {for (i=1; i<=NF; i++) print $i"."}' | tr -s ' ' | sed 's/^\ //g; s/^\.$//g; s/\ \././g; s/\[edit\]//g; s/:\./ - /g; s/\*\./-/g; s/~~~/.../g' | grep -e '[a-z]' | awk '/^~\ Refer/ {exit};/./ {print}' | tr '_:~' ' \-\-' | perl -p -e 's/[^[:ascii:]]//g' | sed 's/&#x005E;/^/g; s/&#x00A8;/\"/g; s/&#x00D7;/\*/g; s/&#x02D9;/\`/g; s/&#x0393;/__Gamma/g; s/&#x03A8;/__Psi/g; s/&#x03B1;/__alpha/g; s/&#x03B2;/__beta/g; s/&#x03B3;/__gamma/g; s/&#x03B4;/__delta/g; s/&#x03B6;/__zeta/g; s/&#x03B8;/__theta/g; s/&#x03BC;/__mu/g; s/&#x03BE;/__xi/g; s/&#x03C4;/__tau/g; s/&#x03C6;/__chi/g; s/&#x03C9;/__omega/g; s/&#x03D5;/__Phi/g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g; s/&#x210F//g;' >> plain.md; echo Processed $n; done
```

Some word counting commands
```
cat plain.md | tr '\$\(\)\{\}\[\]\<\>\/\\\+\-\.,;:\|\=\&\#\*\@\?\%\!\^\"' '                           ' | tr ' ' '\n' | tr 'A-Z' 'a-z' | tr -d '0-9' | awk -F"'" '{print $1}' | sort -u | less
```

