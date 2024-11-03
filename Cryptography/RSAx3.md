RSAx3 from US Cyber Flag Fest
Authors: GabeG888, Tokonuts.


<img width="487" alt="image" src="https://github.com/user-attachments/assets/89d341ac-2fe7-4df7-ba42-957aff4676f6">

Before attempting to decrypt the RSA message, it is important to understand how RSA encrypts messages. The simplified RSA process is as follows:
Generate the priv/pub key pair
1. Generate two prime numbers p and q
2. Calculate n, which is the value of p∗q
3. Calculate values d and e such that d∗e≡1mod(p−1)(q−1) 
4. The public key consists of n and e and the private key consists of d, p, and q
⚠️
What will make the decryption attack possible later is the use of small prime numbers in step 1. These must be large numbers for the encryption process to be secure. 
Encrypt the message
5. Convert the plaintext message into an integer, m
6. Encrypt the message to obtain the ciphertext c, where c≡me(modn)
Decrypt the message
7. Calculate the plaintext message m, where is m=cd(modn)

Factorization-based Tools: Msieve, YAFU, Prime95
RSA Exploit Tools: RsaCtfTool, factordb.com, Cado-NFS
Web Tools: https://www.tausquared.net/pages/ctf/rsa.html#Encryption_and_decryption![image]

The tausquared.net "Broadcast Attack" worked. Msieve couldn't factor numbers that large, YAFU
Was a headache for formatting and I couldn't get it right. Thankfully a google search yielded a nice tool.!

N = 29344003884020109293900502779569204030120750503791412759020283955887065250590362369074858994176128319582299284176118085419286488829797011716085756081953701055477571511754162027165009407465590453032463531242642071658831173638841439076879153059738291676199882331547721785055191653900765061780143392236861301595192110878687674954525518388259134528118662243183546970551338885699952387672848161260138295693170188122868190855995888434539953354983694854289588397094903873855941269824509222550147688779458100562275459010533231521822105543223030145353570847985679285467159994825901243021109321863580166334319736052864951886773
C = 114095791005918998690306745132574132578849665048375868797138758131231938411900159245580393131058249957737629782944908070387530659077069676862319537303581751010786369424697507473696762248523539304141699964341205735013

N = 13572455977905325447484013645070346500059069453281172185367491784068842917973725973617570042971251002368826311391601266085596995631596848864959900277887843090923435104704940267256197384370144065810364093614054303816896383905283941352323820382934790444600869354337965050383154078361948874838033092079162857210804093607073927301246267283131460775917260190417681618692586780402300567258579732133370092629704042601877395445015855229801684498136499453338024062283948344136587144949685859512035161227992082295471091084482124996739130771367103159097141804862300809110078147882763198937057861715397158942072050052780835807957
C = 114095791005918998690306745132574132578849665048375868797138758131231938411900159245580393131058249957737629782944908070387530659077069676862319537303581751010786369424697507473696762248523539304141699964341205735013

N = 11163583008850028774321078295232809033882576850883532833996625446447349385805862089309438012064462649537621386374892682249606251295274254787595438019869529140957955716276006699222518835952610944063820301732611096833089250671691575619661911467748383565394885958961678712916161748074610994930948095034109291129629173700274243148938067210585446638903105262635282391024179557513691119766803747289183369872420057685043948701610595515180753309243759741105968039434884466294738233248104153447374739900402307948062522126797345342926270109931804412585321352204782411033947363397651038754088094684405528129844182714693597981331
C = 114095791005918998690306745132574132578849665048375868797138758131231938411900159245580393131058249957737629782944908070387530659077069676862319537303581751010786369424697507473696762248523539304141699964341205735013

<img width="649" alt="image" src="https://github.com/user-attachments/assets/f67a7132-10be-46c5-acad-ad0f4404d21a">
<img width="654" alt="image" src="https://github.com/user-attachments/assets/3c1349b0-6920-42eb-a696-0e654e13f2fa">

<img width="566" alt="image" src="https://github.com/user-attachments/assets/bf85d100-db98-472f-ad55-a2b441076068">
<img width="597" alt="image" src="https://github.com/user-attachments/assets/edd312cc-ce79-46f3-a05a-04f049b60423">