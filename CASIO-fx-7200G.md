# CASIO fx-7200G

Prog 0\
Fix 0\
Mcl\
749685.32→A\
Ran#→R\
R<.5⇒1→M\
R≥.5⇒1→N\
100→D[M]\
200(Ran#+.001)+100→D[N]\
D[0]▴\
D[1]▴\
D[M]÷D[N]→B\
M=0⇒Int √BA→H▴\
M=0⇒Int (√BA÷B)→W▴\
N=0⇒Int (√BA÷B)→H▴\
N=0⇒Int √BA→W▴\
Fix 1\
.5H▴\
.5W▴\
Fix 0\
Prog 1

Prog 1\
Int 4Ran#→R\
R=0⇒"TL"\
R=1⇒"TR"\
R=2⇒"BL"\
R=3⇒"BR"\
Prog 2\
W→S\
Prog 4\
Prog 2\
H→S\
Prog 4\
H÷12▴\
Prog 2\
Prog 4\
Prog 2\
Prog 4\
Prog 3

Prog 2\
Int 2Ran#→R\
R=0⇒"L"\
R=1⇒"R"\
(Int 4Ran#+1)÷4→T

Prog 3\
Int 4Ran#→R\
R=0⇒"T"\
R=1⇒"L"\
R=2⇒"R"\
R=3⇒"B"

Prog 4\
Int (.5S sin T)▴

---

Prog 0\
Fix 0\
?→H\
?→W\
.5(W-H÷6)→U\
.2H→P\
.3H→Q\
Int (3(Ran#+.001)+1)→A▴\
Lbl 0\
12(Ran#+.001)+12→I▴\
H÷I▴\
W÷I▴\
Prog 1\
Dsz A\
A>0⇒Goto 0\
Int (108(Ran#+.001)+36)→S▴\
0→A\
0→B\
Lbl 1\
1→C\
1→D\
Ran#<.5⇒-1→C\
Ran#<.5⇒-1→D\
.5WC(Ran#+.001)→X\
.5HD(Ran#+.001)→Y\
X<U⇒X>-U⇒Y<P⇒Y>-Q⇒Prog 2\
C=0⇒Goto 2\
Isz A\
X▴\
Y▴\
Norm\
.5Int 3Ran#▴\
Fix 0\
Lbl 2\
A<S⇒Goto 1\
"END"

Prog 1\
1→B\
1→C\
Ran#<.4⇒-1→B\
Ran#<.5⇒-1→C\
.5C((W-H÷6)(Ran#+.001))→X▴\
B=-1⇒B(.2H(Ran#+.001)+.3H)→Y▴\
B=1⇒.3H(Ran#+.001)+.2H→Y▴\
Prog 2

Prog 2\
Isz B\
Frac .5B≠0⇒0→C

(c) Michael Scott 1991

