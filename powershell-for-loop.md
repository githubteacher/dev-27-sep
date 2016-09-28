for ($d=1; $d -le 6;$d++) { touch file$d.md; git add file$d.md; git commit -m "adding file$d.md";}

My SHORTER version:
1..6|%{touch file$_; git add file$_; git commit -m "added file $_";}
