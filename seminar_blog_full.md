S e min arB l og:
 
Int r oduct ion
 
W i th th e gro w th of sma rt t el esco pes ca pa bl e o f E l ect ron i ca ll y Assi st ed Ast ro no my (E AA), 
a st ron o my i s beco mi n g mo re a ccessi bl e to h o bby i st s a n d th e 
pu bli c
. Yet , det ect in g f ai nt 
ga l a xi es, n ebu l a e an d cl u st ers in l i gh t
-
pol lu t ed ski es rema in s a persi st en t cha ll en ge. Th e 
pa per 
"Deep Sky Objects Detectio n w ith Deep Lea rn in g f o r El ectro n ical l y Assisted 
Astro n o my "
 
by Pa ri sot & Ja zi ri t a ckl es th i s h ea d
-
on
ô
craf ti n g deep l ea rni n g (DL) so l ut ion s 
t ha t 
h el p i n 
real
-
ti me det ect io n of cel est ia l wo n ders
.
 
I n t hi s blo g,
 
w e di scov er a nd expl o re a ra n ge o f deep l ea rn in g t echn iqu es dev el o ped fo r 
det ect i n g Deep Sky Obj ect s (DSOs) in i ma ges capt u red by sma rt t el esco pes
 
a n d 
pro vi de
 
a 
gl i mpsei nt o ho w ea ch t echn i qu ewo rk
s
 
a n dref l ect o n t h ei rpo ssi bl erea l
-
wo rl da pp li cat io n s
.
 
B a ck gr oun d: Fr om Ey epiec esto A lgor it h ms
 
St a rga zi n gh a sl on g been a pu rsu it o f pat i en cea nd persev era n ce. Hi sto ri ca ll y , ev en vi ewi n g 
w el l
-
kn ow n deep sky o bj ect s li ke t h e An dro meda Ga l a xy o r Ori on Nebu la deman ded cl ea r 
ski es, remo t e l o cat io n s, a nd ho u rs of man u al set u p. Observ ers h a d t o con t en d wi
th col d 
n i ght s, l i ght po ll u ti on a n d co mpl ex equi pmen t
ô
mo u nt s, ey epi eces, fi lt ers
 
a n d t ra ckin g 
sy st ems
ô
a l l o f w hi ch requ i red expert i se to o perat e.
 
E n t er 
E l ect ro ni cal l y Assi st ed Ast rono my (E AA)
,
 
t
h i s mo dern app roa ch revo lu ti on i zed 
a st ron o my by repl a cin g th e ey epi ece w it h a di gita l sen so r. E AA
-
en a bl ed sma rt t el esco pes 
l i ke St ell in a a n d Vespera a ll ow u sers t o ca pt u re a n d 
sta ck i ma ges o f n ebu la e an d gal a xi es 
i n real
-
ti me, ev en f rom u rban sett in gs.
 
Bu t despit e th i s l ea p f o rwa rd, a n ew pro bl em emerged
 
w h il e sma rt t el esco pes pro du ce 
st u n nin g i ma ges, th ey do
 
n ot 
t ell yo u wh at y ou
 
ar
e l o o kin g at . Fo r th e u nt rai n ed ey e, a fa in t 
bl u r mi ght be a gal a xy
 
o r j u st n oi se. Th e t a sk of i den t if yi n g Deep Sky Obj ect s (DSOs) wi th in 
ca pt u red f rames st il l requ i res a st ro no mi ca l kn ow l edge o r ma n ua l cro ss
-
ref eren ci n g wi th 
st a r cha rt s.
 

Cur r ent Limit at ion s in Elec tr onic a lly A ssist ed A st r on omy
 
Despi t e ma kin g st a rga zin g mo rea ccessi bl e a nd vi su a ll y en ga gin g, E AA sti ll f a ces key 
ch a ll en ges
ô
especi a l l y in au to mat ed Deep Sky Obj ect (DSO) i den ti fi cat io n :
 
1.
 
Im a g e A m big ui ty
 
 
Fa in t DSOso ft en bl en di nt o th e ba ckgro un d, pa rti cu la rl y u n derl i gh t
-
pol lu t edo r 
mo on li t ski es, ma ki n gt h emha rd to di st in gu i sh f ro m st a rso rn oi se.
 
2.
 
N o Re a l
-
Tim e F ee dba ck
 
 
Mo st sma rt t el esco pes do
 
n
o
t con fi rmi f t h et a rget wa s ca ptu red, requ i ri n g ma nu al 
ch ecks o r po st
-
pro cessi n g, w hi ch redu ces in t eract i vi t y an d ma y l ea dt o mi ssed 
o bj ect s.
 
3.
 
E n v iro n me n ta lS e n siti v ity
 
W ea t h er, li gh t pol l ut ion an d sea son al f a cto rs h eav i ly inf l u en cei ma ge qua li ty . 
W i th o ut real
-
ti me det ect io n, u sers ma y u n kno wi ngl y ca pt u re u nu sa bl e da ta .
 
4.
 
L a ck o f Obje ct A n no ta tio n
 
Co n su mer t el esco pes ra rely la bel o ri dent if y captu red o bj ect s, li mit in g sci en tif i c 
v a l u ea nd u ser u n dersta n di n g
 
Th ese i ssu es u n dersco re t h en eed f o r in t ell i gent , rea l
-
t i me DSO det ect io n an d an no ta ti on 
u si n g deep l ea rni n gt o i mprov e ef fi ci en cy an du ser experi en ce.
 
H igh
-
Lev el Implemen t a t ion ofDeep Lea r n in g in DSO 
Det ec t ion
 
Th i sdia gra mo u tl in est h econ cept u al fl ow of ho w deepl ea rn in gt u rn sra w t el esco pei ma gery 
i nt o a cti on a bl e in si ght s
, 
a ccessi bl e ev en to n on
-
expert s.
 
 

S tep 1: R aw Tel esc opeI m ag e
 
Sma rt t el esco pes ca pt u re l on g
-
expo su re, st a cked i ma ges o f th e n i gh t sky . Th ese f ra mes 
ma y in cl u de st a rs, ga la xi es, n ebul a e a nd n oi se du e to li gh t po ll u ti on o r at mo sph eri c 
i nt erf eren ce.
 

 
Fo rma t: 
Ty pi cal l y,
 
in RGBo r FITS fo rmat
 

 
Ch a ll en ge: DSOs a reo ft en f ai nt a n d 
in di sti n ct ; sta rs do mi na t et h ef ra me
 
 
S tep 2: D eep L ear ning Model
 
At ra in eddeepl ea rni n gmo del
 
su ch a sa YOLOdetect o r, ResNet cl a ssi fi er, o rGANgen era to r
, 
a na l y zest h ei ma get oi den ti f yw h eth era n yDeepSky Obj ect sa represen ta n dwh ereth eya re 
l o cat ed.
 
Int er n a lly ,t h i s i n vo lv es :
 

 
F e a ture e x tra ctio n
: Lea rni n gt o di ff eren ti at epat tern sl i kespi ral a rms, di ff u sen ebu la 
gl o w o r gal a xy co res
 

 
L o ca liza tio n
: Dra wi n gbo un din g bo xes o r crea ti ng h ea t ma ps a ro u nd DSOs
 

 
Cla s s ifi ca tio n
: La beli n gt h et y peo f 
o bj ect (e. g. , "ga l a xy" , "n ebu la " , et c. )
 
S tep 3: D etect edD S Os+A nnotat ions
 
Th e o ut pu t i sa n an no ta t edi ma ge:
 

 
Bo u n di n g bo xes a rou n d reco gn i zedo bj ect s
 

 
+ \Ù : XÙ '2:2 Ùe+ : Ù2e\Ùß ß àÙ 
P Ù
ó
 
2 Ù + —–  ý
 

 
Hea t ma psh i gh li gh tin g hi gh
-
co nfi den ce regi on s
 
Th i s ma kes i t i mmedia t ely cl ea r wh at th e i ma ge co nt ai n s
.
 
 
S tep 4: A c c essib l eUnd er st and ing
 
No w ,
 
y ou can ea sil y u n dersta n d
 

 
Wha t o bje cts th e y ca ptur e d
 

 
Whe r e tho s e o bje cts a re in th e fra m e
 

 
Why th e m o de lm a de th o se pr e dictio n s
 
(i f u sing X AI to ol s li ke X RAI )
 

Th i s bri dges t h e ga p bet w een dat a a n d u nderst a ndi n g
, h el pi n gt h eu ser u n derst an d da ta .
 
D at aC oll ect ion: Gr ou nd Tr u thf r omthe B ac ky ar d S ky
 
Th et rai ni n gda ta u sedin th i sstu dy wa sca pt u redu si n gcon su mer
-
gra desma rt t el esco pes
ô
speci f i cal l y th e 
Stel l in a
 
a nd 
Vespera
ô
i n rea l
-
w o rldco n di ti on sa cro ssLu xembo u rg, Fran ce, 
a n d Bel gi u m. Ov er 50 , 00 0 ra w FI TS i ma ges an d nea rl y 5 , 00 0 po st
-
pro cessed JP E G i ma ges 
w ere ga th ered du ri n g th ese sessi o n s, of t en un der li ght
-
po ll u t ed ski esa n d va ria bl e w eat h er. 
Th i sda ta set , f ea tu rin gmo
ret ha n 2 5 0dif f erent t a rget sv i si bl ef ro mth eNo rt h ern Hemi sph ere
.
 
 
D iv ing intotheD etect ion Tech niq u es
 
No w t ha tw e
 
ha
v eesta bli sh edt h emo ti v at ion an dt h eda ta behi n dth i sresea rch ,w e
 
wi
ll di v e 
i nt o t h efo u r 
key deepl ea rni n gt ech ni qu esi mpl emen t edto ta ckl et h echa ll en geo f DeepSky 
Obj ect det ecti on . E a ch a pproa ch bri n gs a un i qu e bl en d of speed, a ccu ra cy , an d 
i nt erpret a bi li t y. Th ese in cl u de:
 
1.
 
A 
n a iv e a ppro a ch
 
u si n g St a rNet w ith ba si c co mpu t er v i si on
 
2.
 
A 
cus to m
-
tr a ine d YOL Ov 7
 
o bj ect det ecti on mo del
 
3.
 
A 
Re s N e t5 0 cla s s ifie r com bin e dw ith X RA I
 
f o r expl a in a bl e det ecti on
 
4.
 
A 
Pix 2 Pix GA N m o de l
 
th at mi mi cs at t ent ion ma ps f o r ra pi d v i sua l f eedb a ck
 
Tec h n ique 1: Naiv e Det ec t ion Usin g St a r Net + Comput er 
Vision
 
W hat 
i
t 
i
s
?
 
Th e fi rst met ho d t est ed 
is
 
simpl e y et crea t iv e a ppro a ch: remov e di st ra ct in g sta rs f ro m th e 
i ma ge u si n g a to ol cal l ed 
Sta rNet an d
 
t h en a pp ly cl a ssi c co mpu t er v i si on (CV) t ech ni qu es
.
 

Th e i dea h ere wa s to st ri p o ut t h e st a rs fi rst a ndt hen i so la t ew ha t mi gh t be cel esti al o bj ect s 
o f i nt erest .
 
H ow I tW or ks 
ó
 
S tep b y Step
 
1.
 
A pply S ta rN e t
 
St a rNet i s a pre
-
t rai n ed deep l ea rni n g mo del desi gn ed t o remo v e st a rs f ro m 
a st ron o mi cal i ma ges. I t o ut pu t sa n i ma gewi th on ly t h eba ckgro u n dco nt en t
 
t y pi cal ly 
n ebu la e, 
gal a xi es, o r cl u st ers.
 
2.
 
Co n v er t to Gr a y s ca le
 
Th est a r
-
remov edima gei ssi mpl if i edto a gray sca lev ersi o n, ma kin git ea si ert odet ect 
edges a n d co nt ou rs.
 
3.
 
E dg e De te ctio n w ith Ca nn y Filte r
 
A st a n da rd CV t echn i qu e (Cann y edge det ect io n) i s u sed t o f in d t h e bou n da ri es of 
o bj ect s.
 
4.
 
B o un ding Bo x Ca lcula tio n
 
An y di sti n ct n on
-
st el la r f eat u re i den tif i ed in t he i ma ge i s bo xed u si n g Open CV 
f u n ct io n s.
 
5.
 
Ov e r la y Re sults
 
Th ese bo un din g bo xes a re t h en dra wn ba ck o nt o th e o ri gin al i ma ge, hi ghl i gh ti n g 
w h ere DSOs w ere 
f ou n d.
 
Re s ults :
 
 
L im ita tions
 

 
N o is e
-
se n s itiv e
: Resi dua l ha lo s f ro m l a rge st a rs o r bri ght a rea s o ft en conf u se t h e 
edge det ect o r.
 


 
F a in t DS Os m is s e d
: Su bt l e o bj ect s ma y be l ost du ri n g th e st a r remo va l o r go 
u n det ect ed ent i rel y .
 

 
F a ls e pos iti v es
: Sta r 
a rti fa ct s o r n oi se bl o bs may be w ro n gly fl a gged a s ga la xi es o r 
n ebu la e.
 
Despi t e bein g fa st a nd requ i ri n g no t rai ni n g dat a , t hi s t ech ni qu e h a
s
 
l i mi t ed preci sio n an d 
reca l l , ma kin g it un su it a bl e fo r mo re n ua n cedo r 
resea rch 
a pp li cat io n s.
 
W hen
 
Is
 
It
 
Usef u l
?
 
Th i s meth o d ma y be h el pf u l f o r qu i ck demo s o r ro u gh f il t erin g, especi al l y if co mput at io na l 
reso u rces a re l i mi t ed. Ho w ev er, i t l a cks th e robu st n ess a n d i nt erpret a bi li t y n eeded f o r 
bro a der u se
 
ma ki n gi t a goo d 
ba sel in e 
to co mpa re a ga in st sma rt er mo del s.
 
Tec h n ique 2: Objec t Det ect ion wit h a Cust om YOLOv7 
Model
 
Wh
at itis
?
 
" YOLO" st a nds f o r Yo u Onl y Loo k On ce, a deep l ea rni n g a rch it ect u re desi gn ed f o r real
-
ti me 
o bj ect det ect ion . YOLO mo del s sca n an i ma ge in o n e pa ss, i dent if y in g bo th t h e presen ce 
a n d 
po sit io n o f o bj ect s w it h bo un din g bo xes. I t
 
is
 
fa st , a ccu ra t e a n d w el l
 
su i t ed t o 
a pp li ca tio n s w h ere bot h speed an d spa ti al a wa ren ess ma tt er
 
li ke i den ti fy in g ga la xi es an d 
n ebu la e in t el esco pe i ma ges.
 
H ow I tW as I m pl emented
 
The Y OLOv7 p ip eline t ak es a t elescop e im age a s inp ut and out p ut s b ound ing b ox es id ent if ying Deep 
Sk y Ob ject s ( DSOs) in r ea l t im e.
 
1.
 
Da ta se t Cr ea tio n
 
ó
 
DeepSpa ceYol o Da ta set
 

Th e a ut ho rs co mpil ed a dat a set o f 4 , 69 6 a nno t at ed ima ges, draw n f ro m rea l 
t el esco pe sessi o n s u si n g Vespera a nd 
St ell in a in st rum ent s. E a ch i ma ge h a d
 
t o be 
ma n ua ll y l a bel l eda n d
 
bo un di n g bo xes 
h a dt o bedra w n a ro u nd DSOs.
 
2.
 
Tr a n s fe r L ea r nin g fo r YOL Ov7
 
I n st ead of t rai nin g f ro m scrat ch , t h e mo del wa s bu i lt u sin g t ran sf er l ea rn in g
 
st a rt in g 
f ro m a pre
-
t rai n ed YOLOv 7 mo del an d fi n e
-
t un in g it o n t h e cu sto m dat a set . Thi s 
si gn if i can tl yredu cedt rai ni n gti mewh il ei mprov ingco nv ergen cea n dperfo rman ceo n 
a st ron o my
-
speci f i cf ea tu res.
 
3.
 
Tr a in ing Par a me te rs
 
a.
 
Ba t ch si ze: 4
 
b.
 
I ma ge si ze: 6 0 8× 6 08 pi xel s
 
c.
 
E po ch s: 2 00
 
d.
 
Opt i mi zer: Ada m
 
e.
 
Fra mew o rk: Py To rch wi th YOLOv 7 of fi cia l i mpl emen t at io n
 
R esu l ts&Per f or m anc e
 

 
Pr e cis io n
: 0. 7 9
 

 
Re ca ll
: 0 . 51
 

 
F1
-
S co r e
: ~0 . 62
 
Th i s wa s th e 
best
-
perf o rmin g model a mon g a ll a pp ro a ch es t est ed, deli v erin g cl ean 
bo u n di n gbo xes a rou n d DSOs
 
ev en in mo derat ely no i sy , li gh t
-
po ll u t edi ma ges.
 
Re s ult:
 
 
A w i de
-
f i eld i ma ge o f 
Messi er 4 9 
(a gal a xy i n t he Vi rgo cl u st er) sh ow ed cl ea r, a nno t at ed 
bo xeso v ert h epri ma ry ta rget an dsu rro un din gga la xi es
ô
v i si bl eev en t o n on
-
expert v i ew ers.
 
 

S tr eng ths
 

 
F a s t Infe r e n ce
: Rea l
-
t i me perfo rman ce du rin g 
sta rga zin g 
sessi o n s.
 

 
Re lia ble o n Com mo n Tar g e ts
: P a rt i cul a rl y a ccura t e wi th bri ght gal a xi es, n ebul a e, 
a n d cl u st ers f ro m cat al o gs li ke Messi er o r NGC.
 

 
S ca la ble
: Ca n be ret ra in edf o ro th er sky regi on s or t el esco pe t y pes.
 
 
L im ita tions
 

 
S m a ll DS Os S till Ch a lle ng in g
: YOLO mo del s ma y mi ss ext remel y f ain t o r smal l 
o bj ect s wi th j u st a f ew pi xel s of a ppa rent si ze.
 

 
Tr a in ing Da ta s e tRe quir e d
: Th i sa ppro a ch n eedsw el l
-
an no ta t edi ma ges
 
fo rt rain in g 
a n di t so n eo f th e fa ct o rsa ff ect in gi t s F1 sco re
.
 
Tec h n ique 3: DSO Cla ssific at ion wit h R esNet5 0 a n d 
Ex pla in a ble A I (XR A I)
 
 +Ù} V Ù—+ \Ù e Ù \U: ee2 Ù\à Ù e Ùe \Ù +'Ù Ù 
'Ù —
 
y ou get bo un di n g bo xes, 
bu t no i n si gh t in to 
ho w 
t h e mo del a rriv ed at th at resu l t . Th i s i s wh ere E xpl ai na bl e AI (X AI ) 
co mes i n . In thi s t echn i qu e, a deep l ea rn in g cl a ssi f i er det ect s w h et h er a DSO i s present in 
a n i ma ge, a n dth en X RAI (apo st
-
h o cexpla in a bi li tyt oo l )gen era t esa h eat ma psh ow in gwh i ch 
pa rt
s of t h ei ma ge con t ri but ed mo st to th at deci sio n .
 
H ow I tW or ks
 
 
Thispipel in ecl a ssifiestel esco peima gesu sin gResNet5 0 an d,ifa DSOisdetected,pro v ides 
a n in terpreta bl e expl an a tion fo ra ccessibl e u n dersta n din g.
 
1.
 
B in a ry Clas s ifi ca tio n w ith Re sN e t50
 
I ma ges a re f i rst f ed int o a 
Re s N e t5 0
 
mo del
ô
a pow erf ul co n vo lu ti on al n eu ral 
n et wo rk th at l ea rn s t o an sw er a si mpl e qu esti on : 
I s a DSO presen t in this ima ge?
 

 
Th e dat a set u sed h ere wa s ba la n ced betw een ima ges w i th a nd wi th ou t DSOs, w it h 
ca ref u l l abel in g to a v oi d bi a s.
 
2.
 
E x pla ina bility
 
w ith X RA I
 
Ù e Ù 1:+ Ù+ \\ \Ù2 Ù Ù \Ù 
Ù\2 e à  Ù
X RA I
 
(a t echni qu e ba sed on 
I nt egra t ed Gra di ent s) ki cks i n t o hi gh li ght 
w here
 
i n t h e i ma ge t h e mo st in fl u ent ia l 
f ea t u res a re. Th ese sh o w u p a s a 
h e a tm a p o ve r la y
à Ù}+2 Ù e Ù 
e e2 e :2 Ù ‘: 2\Ù
t h e mo del f o cu sed on .
 
W o rki n g:
 
1.
 
Inte g ra te d Gr a die n ts a s a Fo un da tio n
 
X RAI bu il ds on a t echn i qu e ca ll ed 
I nt egra t ed Gradi en t s
, w hi ch esti mat es h ow mu ch 
 Ù U —+ Ù: 2ej e\Ù e :Ù eÙ 1:+ 
\Ù 2+Ù : je Uj eß ÙeÙ\Ù e  \ÙÙ: 1 X 2 Ù e Ù+Ù
 Ù e :ÙÙ 
 \+2 Ù üe – ++ –ÙÙ'Ù 1 Ù X\2 e 2 Ù \'– Ù'X: j 2Ù2Ù
mea su ri n gh ow predi ctio n scha n gea sth ei ma gemo rph sf ro mt h e 
ba sel in eto t h ereal 
i n put .
 
2.
 
Re g io n S e gm e n ta tion
 
I n st ead o f a na l y zin g pi xel s i n di vi du al ly , X RAI groups pi xel s i n to 
su perpi xel s
 
co h eren t 
regi o n s of t h ei ma ge
ô
li ke t h e bri ght co reo f a gala xy o r th e w i spy edges o f a n ebu la .
 
3.
 
A ttr ibuti o n S co r in g
 
I t th en a ssi gn s 
i mpo rta n cesco rest o t h eseregi o nsba sedo n ho w mu ch th ey cha n ged 
t h e mo del 's con fi den ce du ri n gt h ei nt egra ti on process.
 
4.
 
He a tma p Ge n e ra tion
 
Th e regi on s w it h t h e 
hi gh est cu mu la ti v e co nt ribu t io n a re ov erl ai d a s h eat ma ps, 
 ++ :2 Ù – : j Ù e :Ù } \j +Ù Ù eÙ 1:+ Ù 
+ :: ' Ù 2 Ùe Ù e e Ù ÙÙ \Ù
presen t .
 
So , w h en yo u see a bri ght 
bl u e
 
blo b o n a n X RAI ma p, y ou
 
a
re essen t ia ll y seei n g 
w h ere t h e 
mo del f o cu sed it s at t en ti on
 
th e mo st in fl u ent ia l pi xel s in th e 
deci sio n
-
ma ki n g
 
pro cess.
 
R esu l ts&Per f or m anc e
 

 
A ccur a cy
 
(cl a ssif i ca ti on ): ~ 9 7% on val i da ti on set
 

 
Pr e cis io n/ Re ca ll
 
(v ia h ea tma p bo un din g bo xes):
 
o
 
P reci si on : ~0 . 68
 
o
 
Reca l l : ~ 0 .4 1
 
o
 
F1
-
Sco re: ~ 0 .5 1
 

W h il e sli ght l y l ess preci se t ha n YOLOv 7, i t pro v i des so met hi n g 
YOLO ca nn ot :
 
v i sua l 
expl a in a bi li ty .
 
L im ita tions
 

 
N o t Re a l
-
Tim e
á ÙÙ: 1Ujee: 2Ù \Ù \+:XÙe  2 Ù
\Ùe Ùee: 2ß
 

 
N e e ds Mor e Po w er
: Run ni n gh eat ma pso n la rge ima ges (l i ke 3 58 4 ×3 5 84 px) 
requ i res di vi din g th em in to pa t ch esa n d st it chi n gresu l t s.
 

 
N o La be ls o r B o un din g B o xe s by 
De fault
: You get 
w here
, bu t n ot 
wh at
ô
wi th o ut 
f u rth er cl a ssif i ca ti on l a y ers.
 
B estUseC as es
 

 
Re s e a r ch 
a n do utr ea ch
á Ùe Ù : XÙ—U+22 Ù : Ù Ù 
e 2 '\ Ùj e Ù \e X:2:+ Ù
i ma ges.
 

 
Mo de l de v e lo pm e n t
: I dent if yi n gf ai lu re poi nt s and ref in in g det ecti on 
st rat egi es.
 
 

 
Th e 
co re of Messi er 1 3
 
(gl o bu la r cl u st er)
 
 


 
Th e fa in t gl ow of 
Me ss ie r 7 6 (L ittle Dum bbe ll N ebula )
 
T e c hni que 4 : F as tDSO Hi ghli ghti ngwi thP i x2 Pi xGAN
 
W hy aGA N ?
 
Th e th i rd t ech ni qu e (ResNet 50 + X RAI ) gav e u s incredi bl y u sefu l h eat ma ps sho wi n g w hi ch 
regi o n s of t h e i ma ge co nt ai n ed Deep Sky Obj ect s. Bu t th ere
 
is
 
a ca t ch : X RAI i s sl ow , 
especi a l l y o n l a rge
 
an d
 
hi gh
-
reso l ut io n i ma ges. 
I t beco mes 
a pro bl em wh en y ou w ant t o 
pro v i de rea l
-
ti me f eedb a ck
.
 
To o v erco me th i s, th e a u th o rs t u rn ed t o Gen era t iv e Adv ersa ri al Net wo rks (GANs
) 
speci f i cal l y, t h e Pi x2 Pi x a rch it ect u re
ô
t o gen era te si mi la rh i ghl i gh t ma ps mu ch fa st er.
 
H ow I tW or ks
 
P i x2 Pi xi saco ndit io na l GAN
 
t rai n edf o ri ma ge
-
to
-
ima get ran sl at io n. In st ea do f cl a ssif yi n go r 
det ect i n g o bj ect s di rectl y , it l ea rn s to 
tra n sf o rm on e ima ge in to 
an ot h er
ô
i n th i s ca se, f ro m 
ra w t el esco pe i ma ges t o h eat ma pst ha t mi mi c X RAI o ut pu t s.
 
I nsid etheGA N : Gener at or v s. D isc r im inat or
 
A Gen era t i v e Adv ersa ria l Net wo rk (GAN) i s ma de o f tw o n eu ral n etw o rks t ha t pl ay a kin d of 
ga me a gai n st ea ch o th er:
 
1. The Gener at or : " TheA r tis t"
 
Th eGen era to ri sli kea n a rt i st t ra in edt o t a kean inpu t i ma ge(i n o u rca se, a t el esco peph ot o ) 
a n d gen erat e a n ew i ma ge (t h e predi ct ed DSO hea t ma p). I t s goa l i s to ma ke th e h ea t ma p 
l oo k a s rea li st i c an d i nf o rma ti v e a s po ssi bl e
ô
i dea ll y , so co n vin ci n g th at 
 e 
\Ù
i n di st in gu i sh a bl e f ro mo n e ma de by t h e mo re deta il ed, but slo w er X RAI t echn i qu e.
 

 
Input
: RGB 
a st ro no mi ca l i ma ge
 

 
Output
: Sy n th et i c h eat ma p sh ow in g wh ere t h e DSO i s l i kely lo cat ed
 

 
Go a l
á Ù:: + ÙeÙ \ 1 2 e: XÙ2 e: Ùe  2 '2 Ù e \Ù :j e Uj e Ù \Ù
 +
 

2. TheD isc r im inat or : " TheC r itic "
 
Th e 
Di scri mi na to r 
i sa bi na ry cl a ssif i er t ra in edt o 
di st in gu i sh rea l v s. f a ke h ea t ma ps.
 
It sees 
pa i rs of :
 

 
Ù e+\:Ù Ùm ÙÙ + Ù Ùe UÙ ü X: 1Ù e X22 Ùe ýÙ„ Ù \: j +Ù ++ Ùe  \Ù \Ù

 + 
 

 
Ù e+\:Ù Ùm ÙÙ 2 e e UÙ ü X: 1Ù eÙ2 e: XýÙ „ Ù \ : j+++ Ù e \Ù
 \Ù 
  '
 
I t s jo bi s to crit i qu e th e Gen era to ra n d 
ca ll o u t any in a ccu ra ci es o ro dd it i esi
n t h ef a ke 
h ea t ma ps.
 

 
Input
: A pai r (i ma ge + h ea t ma p)
 

 
Output
: Rea l (1 )o r Fa ke (0 )
 

 
Go a l
: Nev er get f oo l ed
 
The Tr aining L oop : A L ear ning Tu g
-
of
-
W ar
 

 
Th e Gen era to rl ea rn sf ro m th e Di scri mi na to r's f eedb a ck a n d get s bet t era t fa ki n gi t.
 

 
Th e Di scri mi na to r sees bet t er an d bett er fa kes a nd get s sma rt er at spot ti n gt h em.
 

 
Th i s ba ck
-
a n d
-
fo rth con ti n u es un ti l th e Gen era to r beco mes so go o d th at it s ou t put 
beco mes n ea rl y in di sti n gui sha bl ef ro m th e rea l t hi n g.
 
Fo r exa mpl e, a n i ma ge of Messi er 1 7 (Omega Nebu l a ) pro cessed w i th Pi x2 Pi x pro du ced a 
v i vi dh i ghl i gh t of th e emi ssi on zo n e, cl o sely mi rro ri n g wha t X RAI w o ul dh a v e sh ow n
ô
but in 
a f ra cti on of t h et i me.
 
S tr eng ths
 

 
Ra pid fe e dba ck
: I deal f o rl iv e demo s o r a ut o ma ted o bserv a ti on sessi o n s.
 

 
L o w co m pute r e quire m en ts
: Great f o rl apto ps, Ra spb erry P i, o r embedd ed 
t el esco pe so ft wa re.
 

 
Us e r 
e ng ag e me n t
: Gi v es u sers i mmedia t e vi su al cu es a bo u t wh ere t o l oo k.
 
L im ita tions
 

 
S lig h tly les s pr e cise
: No t a sa na l yt i ca ll y a ccu rate a s t rue X RAI , especi al l y u nder 
n oi sy o r lo w
-
co nt ra st con dit io n s.
 


 
N o o bje ct la be ling
: I t sh ow s 
w here
 
t h e DSO i s, bu t no t 
w ha t
 
i t i s.
 
 
S u m m ar y
 
E a ch deep l ea rni n g t ech ni qu e expl o red i n thi s st u dy brin gs di stin ct st ren gt h s ta il o red to 
di ff eren t u seca sesi n El ect ron i cal ly Assi st edAst ro no my . Th e 
S ta rN e t+ CV
 
a pp roa ch o ff ers 
a qui ck an d si mpl e ba sel in e but st ruggl es w it h accu ra cy an d n oi se. 
YOL Ov 7
 
st an ds o u t a s 
t h e mo st ro bu st a nd bal an ced mo del , del iv eri ng h i gh preci sio n an d rea l
-
ti me det ecti on 
ma ki n g it i deal fo r bo th a ut omat io n an d o ut rea ch. 
Re s N e t5 0 + X RA I
 
t ra des speed f o r deep 
i nt erpret a bi li t y, o ff eri n g ri ch v i sua l in si ght s in to model rea soni n g,
 
w hi ch i s especi al ly 
v a l ua bl e f o r edu cat io na l a n d sci ent if i c t ran sparen cy . Fi na ll y , t h e 
Pix 2 Pix GA N
 
cl ev erl y 
mi mi cs X RAI 's o ut put s a t a f ra ct ion of t h e co st , pro v i di n g f a st v i sua l f eedb a ck f o r u ser
-
f ri en dl y a ppl i cat ion s. To geth er, th ese mo del s represen t a pow erf ul t oo l kit , ca pa bl e of 
t ra n sf o rmi n g sma rt t el esco pes f ro m pa ssi v e i ma gi n g devi ces i nt o in t ell
i gen t , in t era ct i v e 
o bserv a to ri es.
 
 
A s pe c t
 
YOLOv 7
 
R e s Ne t+ XR A I
 
Pix 2 Pix GA N
 
Goa l
 
D e te ctan d 
l o cal i ze D SO 
w i th bo un d in g 
b o xe s
 
 
C l a ssi fypr e se n ce o fD SO 
+ 
e xp la in vi a XAI
 
 
Ge n er a te h ea tma p
-
l i ke 
vi su al e xpl an a tio n
 

Output
 
Bo u nd in gb o xe s 
a r ou nd D SOs
 
Bi n a r ycla ss+ XR AI 
h ea tm ap
 
 
An n o ta te d im a ge ( XR AI
-
styl e o ver l a y)
 
A r c hite c tur e
 
On e
-
sta ge 
o b je ctd e te cto r
 
D e ep C N N + Po st
-
h o c 
XAI
 
C o nd i tio na l GAN ( U
-
Ne t+ 
Pa tch GAN )
 
Spe e d
 
Fa st( r ea l
-
ti m e 
ca pa b le )
 
Sl o w ( XR AIi ssl o w )
 
Fa st( si n gle p a ss,mu ch 
fa ste r tha n XR AI)
 
Ex pla ina bil ity
 
N o ( bl a ck
-
bo x)
 
Ye s( XR AI)
 
Ap p ro xi ma te ( vi su al l y 
si m i la r to XR AI)
 
F1 Sc or e
 
0 .6 2 ( Be st)
 
0 .5 1
 
N o td i re ctl ycom pa ra b le 
( PSN R > 3 8 )
 
A pplic a t ion s of Deep Lea rn in g in EA A
 
Deepl ea rn in gi sno t ju st an a dd
-
on to E AA
ô
it
 
i
sa f o rcemu lt i pl i erth at u nl o cksn ew l ev el so f 
a u to no my , scal a bi li ty , an d a ccessi bil it y . Here a re so me i mpa ct fu l wa y s DL en ha n ces t h e 
pra ct i ceo f a st ro no my :
 
1. S m ar tOb ject D etect ion
 
DL mo del s l i ke 
YOL Ov 7
 
an d 
Re sN e t50
 
empow er sma rt t el esco pes t o a ut o ma ti cal ly det ect 
Deep Sky Obj ect s (DSOs) a s i ma ges a re bein g ca pt u red. Thi s i s especi al l y pow erf ul f o r:
 
u
n at t ended t el esco pes
 
a n d
 
d
yn a mi c o bserv a tio n w o rkf lo w s, w h ere t el esco pes a dj u st 
expo su re t i mes o r swi t ch ta rget s ba sedo n det ecti on con fi den ce
 
2. Post
-
C ap tur eI m ag eFil ter ing and A nnotat ion
 
W i th t ho u san dsof i ma gesgen era t eddu rin go bserv a ti on sessi on s, ma n ua ll y revi ewi n gt h em 
i s i mpra ct i ca l. DL
-
ba sed fi lt erin g:
 


 
Ta gs o r di sca rds lo w
-
qu al it y f ra mes, sa v in g ti mea n d 
st o ra ge
 

 
I den ti fi es u n expect ed ta rget s su ch a s co met s, supern o va e
 
o r sat ell it e t ra il s
 

 
Su pp o rt s co ll a bo rat iv e ima ge sta cki n g, en su ri ng t ha t o nl y hi gh
-
si gna l f ra mes a re 
merged f o r fi na l pro cessi n g
 
3. Ex p l ainab il ity w ithX A I (X R AI )
 
Deepl ea rn in gmo del sa reo ft en crit i ci zeda s" bl a ckbo xes, " bu t 
E xpl ai na bl eAI to ol sl i keX RAI
 
ch a n ge th at na rra ti v e. By sh o win g 
w h y 
a mo del det ect ed a cert a in regi on a s co nt ai nin g a 
DSO, t h ese v i su al i za ti on s
 
h el p i n bui ldin g u ser t rust an d edu cat e begi n n ers u n dersta n d 
a st ron o my 
 
Limit a t ion s of Deep Lear n in g in EA A
 
W h il e deep l ea rn in g bri n gs si gn if i ca nt a dva n cemen t s t o sma rt a st ron o my , it 's no t wi th ou t 
co n st rain t s. U n derst an di n gt h ese li mit at io n si s cruci al fo r deplo yi n g mo del s eff ect iv el y an d 
i mpro vi n gth em f u rt h er.
 
1. D at as etS c ope&Gener al ization
 
Th e model s dev elo ped in t hi s resea rch w ere t ra ined o n da ta ca pt u red u sin g speci fi c sma rt 
t el esco pes (e. g. , St ell in a an d Vespera wi th 50
ó
8 0 mm a pert u res). As a resu lt :
 

 
Gen era l i zi n g to diff eren t t el esco pe 
set u ps
ô
w it h o th er a pert u res, sen so rs, o r fo cal 
l en gth s
ô
ma y requi re co ll ect in g n ew dat a an d retra in in g.
 

 
P erf o rma n ce ma y dro p if a ppl i ed to in st rum ent s w i th va st ly dif f eren t o pti cs, su ch a s 
DSLR
-
ba sed ri gs o r prof essi o na l o bserv at o ri es.
 
2. C omp u ta tional C onst raints
 
Adv a n ced expl ai na bil it y meth o ds li ke X RAI , wh il e po w erf ul , a re co mput at ion al l y i nt en si v e, 
pa rti cu la rl y on la rge, hi gh
-
reso l ut io n a st ro no mi cal i ma ges
 

 
Rea l
-
t i me a pp li ca tio n s may requ i re brea ki n g i ma ges i n to sma ll er pa t ch es, w hi ch 
a dd s co mpl exi t y.
 

 
Dev i cesw i th o ut GPU s(e. g. , embedd edsy st emso rRa spb erry P i )may st ruggl eu nl ess 
o pti mi zedo r pa i red wi th l i gh t er mo del s li ke P i x2P ix.
 

3. D etect ionC hal l eng es&A m b ig u ities
 
Despi t e st ron g resu l t s, certa in a st ron o mi cal f ea tu res rema i n h a rd to di st in gu i sh:
 

 
Bri gh t st a rs wi th l a rge ha lo s can be mi scl a ssif i eda s co mpa ct gal a xi es.
 

 
Fa i nt DSOs wi th v ery lo w co nt ra st a re of t en mi ssed by obj ect det ect o rs.
 

 
I n bo rderli n e ca ses, h u ma n expert v al i da ti on sti ll o ut perfo rms AI , especi al l y w h en 
di ff eren ti at in g n ua n ced st ru ct u res
.
 
4. L ac kofB enc hm ar king S ta nd ar d s
 
Th ere i s cu rren tl y n o u ni v ersa ll y a ccept ed ben chma rk f o r ev al u at in g deep l ea rn in g model s 
o n sma rtt el esco pe da ta
 
w hi ch 
ma kesi t ha rdt o co mpa remet ho dsa cro ss resea rch gro u ps.
 
P erf o rma n cemet ri csca n va ry 
si gni fi can tl y ba sedo n dat a set qua li ty , prepro cessi n gch oi ces, 
a n d eva lu at io n cri t eria .
 
F ut ur e W ork : 
 
W h il e th e cu rrent t ech ni qu es sh ow pro mi se, th ere
 
is
 
a mpl e roo m f o r i mpro v ement . Fut u re 
ef f o rt s can f o cu s on bo th ref in in g exi sti n g mo dels a n d expa ndin g th ei r ca pa bil it i es t o meet 
t h e deman ds of mo re div erse u se ca ses.
 
I m p r ov ing Techniq u e3: R esN et50 +X RA I
 
To en ha n ce bot h cl a ssi fi cat io n a ccu ra cy a nd i nt erpret a bi li t y, sev era l u pgra des a re 
en v i sio n ed:
 

 
Mo de l F in e
-
Tun ing
 
Adj u st in g pa ra met ers su ch a s l ea rn in g rat e, ba t ch si ze, a n d o pt i mi zer set ti n gs can 
o pti mi zet rai ni n g co n v ergen ce an da ccu ra cy .
 

 
A r ch ite ctur a lE n ha n ce m en ts
 
E xpl o ri n g deeper o r mo re ef fi ci ent n et w o rks li ke 
ResNet 1 0 1 o r E ffi ci ent Net 
may 
i mpro v ef eat u re ext ra cti on , especi a ll y f o r su bt l eor 
di ff u se DSOs.
 

 
Da ta se t Re fin em e n t
 
Remo v in g mi sl a bel ed o r lo w
-
qu al it y sa mpl es a n d en su ri n g cl a ss bal an ce w i ll 
i n crea se t ra in in g si gna l cl a ri ty an d redu ce fa l se po si ti v es.
 

 
A dv a n ce dE x pla ina bility To o ls
 

I n co rpo rat in g 
at t en ti on
-
ba sed X AI met ho ds li ke 
Gra d
-
CAM+ + 
co ul d of f er sha rper, 
mo re lo cal i zed h eat ma ps, fu rth er i mpro vi n g mo del t ra n spa ren cy an d DSO 
pi n po in ti n g.
 
I m p r ov ing Techniq u e2: Y OL Ov 7Ob ject D etect ion
 
Fo r rea l
-
ti me o bj ect det ect io n , th e n ext st eps i n clu de:
 

 
Multi
-
Cla s s Tr a in in g
 
Ra t h er t ha n t rea ti n g a ll DSOs a s a sin gl e cl a ss, f u t u re mo del s ca n di sti n gui sh 
bet w een 
gal a xi es, cl u st ers, an dn ebu la e,
 
o ff eri n gri ch eran no ta ti on san dedu ca ti on al 
v a l u e.
 

 
Da ta A ug me n ta tio n
 
I nt ro du ci n gva ria ti on s(e. g. , bl u rri n g, n oi sein j ecti on , bri gh tn esssh i ft s)du ri n gt ra ini n g 
ca n h el p model s gen era li ze bet t er
ô
especi a ll y i n n oi sy o r u n derexpo sed co n di ti on s 
co mmo n in u rba n o r sho rt
-
expo su re set u ps.
 
By a dva n ci n g bot h cl a ssif i ca ti on an d det ecti on pa th w ay s, f ut u re sy st ems w il l n ot on ly be 
f a st er a n d mo re a ccu ra t e but al so mo re in fo rma ti v e, i nt erpret a bl e, an d resi li ent a cro ss 
di v erse sky
-
w a t chi n g scena rio s.
 
Conc lusion
 
Deep l ea rni n g i s t ran sf o rmi n g E l ect ro ni cal ly Assi st ed Ast ro no my (E AA) f ro m a pa ssi v e 
i ma gin g experi en ce in to an in t el li gen t , in t era ct iv e pro cess. Th i s wo rk 
sh ow s th a t ev en 
co n su mer
-
gra de t el esco pes, wh en pai red wi th mo del s l i ke YOLOv7 , ResNet 5 0 + X RAI, a n d 
P i x2 Pi x GAN can det ect , hi gh li ght an d expla in Deep Sky Obj ect s i n real
-
ti me o r n ea r
-
rea l
-
t i me.
 
E a ch t echn iqu e bri n gs u ni qu e v al u e
ô
YOLOv 7 l ea ds i n det ecti on perf o rma n ce, ResNet 5 0 
a dd s in t erpret abil it y a n d P i x2P i x o ff ers speed f o r i mmedi at e u ser f eedb a ck. To get h er, t h ey 
f o rma di v erse t oo l kit f o r sma rt st a rga zi n g.
 
W i th i mpro v ement sin mo del gen era li zat io n ,dat aset di v ersi ty a n dco mput at io na l ef fi ci en cy, 
t h e pa th f o rw a rd i s cl ea r: deep l ea rn in g wi ll n ot o nl y h elp u s l oo k at t h e st a rs, bu t t rul y 
u n derst an dt h em
.
 

R efer en c es for B log on Deep Sky Objec t Det ect ion in EAA
 
R esear c hPa p er s&A r ticl es
 
1.
 
Pa r iso t, O. & J a zir i, M. (2 0 24 ).
 
Deep Sky Obj ects D etec tio n w ith 
Deep Lea rn in g f or E l ectron ica l ly Assisted 
Astro n o my .
 
Astro n o my , 3 (2 ),
 
122
ó
13 8 .
 
 
DOI : 1 0 . 33 9 0 /a st ron o my 3 02 0 00 9
 
 
Li n kt o pa per
 
2.
 
Ra m o s , L . T. & Riva s
æ
E ch e v er r ía , F . (20 25 ).
 
Deep sky o bject d ete ctio n in a stro no mica l ima gery u sin g YOLO mo del s: a 
co mpa ra tiv e a ssessm en t.
 
 
Neu ra l C o mpu tin g a n d App l ica tion s.
 
 
DOI : 1 0 . 10 0 7 /s00 5 21
-
025
-
11 2 23
-
4
 
 
Li n kt o pa per
 
3.
 
B a ro n , D. (2 01 9 ).
 
 
Ma chin e Lea rn in g in Astro no my : a pra ctica l ov erv iew .
 
 
a rXi v : 
1 9 0 4. 0 72 48
 
 
Li n kt o pa per
 
 
D at as ets&C odeR esou rc es
 

 
De e pS pa ce Yo lo Da ta s e t
 
ó
 
~4 , 69 6 an no ta t ed RGB i ma ges ca pt u red by sma rt 
t el esco pes.
 
 
Access Da t a set
 

 
A ug m en te d
æ
De e pS pa ce Yo lo
 
ó
 
E xpa n ded to ~ 8 , 42 1 i ma ges w i th rea li st i c 
a u gmen ta ti on s f o r mo del ro bu stn ess.
 
 
Gi t Hu b Repo sit o ry
 
R el at edC ontex t
 

 
A s tr o in fo rm a tics Ov e r v iew
 
 
I nt ro t o dat a sci en ce a n d AI in a st ro no my.
 
 
W i ki pedi a : 
Ast ro inf o rma ti cs
 


 
YOL O Obje ct De te ctio n in A s tr o no m y
 
 
Fo u n da ti on al app roa ch fo r real
-
t i me obj ect det ect i on a ppl i ed t o sky i ma gery .
 
 
A&A YOLO St u dy
 
 
Ori gi na l YOLO Pa per (a rXi v )
 
 

