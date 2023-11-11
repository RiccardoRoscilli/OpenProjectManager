<!DOCTYPE html>
<html>
<head>
	<meta http-equiv="content-type" content="text/html; charset=utf-8"/>
	<title></title>
	<meta name="generator" content="LibreOffice 7.3.7.2 (Linux)"/>
	<meta name="created" content="2023-11-06T09:52:33.072583940"/>
	<meta name="changed" content="2023-11-11T17:33:10.919511256"/>
	<style type="text/css">
		@page { size: 21cm 29.7cm; margin: 2cm }
		p { line-height: 115%; margin-bottom: 0.25cm; background: transparent }
		h1 { margin-bottom: 0.21cm; background: transparent; page-break-after: avoid }
		h1.western { font-family: "Liberation Sans", sans-serif; font-size: 18pt; font-weight: bold }
		h1.cjk { font-family: "Noto Sans CJK SC"; font-size: 18pt; font-weight: bold }
		h1.ctl { font-family: "Lohit Devanagari"; font-size: 18pt; font-weight: bold }
		a:link { color: #000080; text-decoration: underline }
		a:visited { color: #800000; text-decoration: underline }
	</style>
</head>
<body lang="it-IT" link="#000080" vlink="#800000" dir="ltr"><p align="center" style="line-height: 100%; margin-top: 0.42cm; margin-bottom: 0.21cm; page-break-after: avoid">
<font face="Liberation Sans, sans-serif"><font size="6" style="font-size: 28pt"><b>Open
Project Manager</b></font></font></p>
<p><br/>
<br/>

</p>
<p>Open Project Manager nasce per tenere sotto controllo le attività
quotidiane di sviluppo e per coordinare i diversi team in diversi
progetti. Coinvolge clienti, collaboratori, project manager e mira a
gestire tutto il ciclo di vita del progetto. Si adatta bene allo
sviluppo del software, ma può essere usato in tutti gli ambiti in
cui c’è un progetto ed un team da gestire. 
</p>
<p>N.b. 
</p>
<p>Il progetto è in continua evoluzione per cui è passibile di
cambiamenti continui sia manutentivi che evolutivi. 
</p>
<p><br/>
<br/>

</p>
<h1 class="western">Tecnologie utilizzate</h1>
<p>Il software è sviluppato in laravel 10 con Bootstrap 5. Per
l’autenticazione si è scelto Spatie. Per il resto, specialmente
per l’integrazione on API esterne si vedrà strada facendo. Non
viene fornito con uno di quei bellissimi template per il backend
perché tanto non è destinato al pubblico, ma soprattutto non mi
andava di spendere 49 dollari. Non viene sviluppato con Vue ed
Inertia per 2 motivi: innanzitutto non conosco abbastanza bene Vue,
in secondo luogo perché bootstrap con blade è gestibile da una
maggior quantità di sviluppatori che potenzialmente potrebbero
entrare a far parte del progetto. Terzo motivo, anche chi non conosce
bootstrap con mezza giornata è dei nostri.</p>
<p>Mettiamo pure che Bootstrap garantisce che il software sia
responsive, quindi può essere usato alla grande anche con tablet e
smartphone anche se è evidentemente fatto per il desktop.</p>
<p><br/>
<br/>

</p>
<h1 class="western">Ruoli e Utenti</h1>
<p>Come attori principali abbiamo quindi:</p>
<p>Superadmin (ha accesso a tutte le risorse, crea gli utenti,  i
ruoli, i progetti)</p>
<p>Il Cliente</p>
<p>Il Project Manager</p>
<p>Lo o gli sviluppatori</p>
<p>Il project manager ascolta il cliente sulle proprie esigenze. Il
progetto può essere nuovo o manutenzione di uno attualmente
esistente. 
</p>
<p>Il project manager propone una soluzione al cliente. Previa
accettazione da parte del cliente (si consiglia un documento scritto
con eventuale mockup controfirmato per evitare malintesi) il project
manager traduce il documento in attività da assegnare agli
sviluppatori.</p>
<p>La prima attività è sempre quella di creare un ambiente di
sviluppo condiviso su cui i programmatori lavoreranno ed il PM avrà
modo di controllare l’avanzamento dei lavori. Se il progetto già
esiste ed è in produzione, è consigliabile clonare l’attuale web
app (staging).</p>
<p>Una volta creato l’ambiente il PM provvede a suddividere il
progetto in attività da assegnare a uno o più sviluppatori. 
</p>
<p>Ogni sviluppatore appartenente al progetto avrà un area di lavoro
in cui saranno presenti gli accessi all’ambiente di sviluppo. 
</p>
<p>Ogni attività (task assegnato) sarà preventivato in termini di
costi e tempi di ultimazione.</p>
<p>Una volta valutati i task in termini di tempo, il PM sarà in
grado di produrre il GANTT del progetto 
</p>
<p>Attraverso il GANTT è possibile definire anche i SAL del progetto
e quindi i relativi pagamenti.</p>
<p>Per gestire il versioning del software dovrebbe essere utilizzato
git. In questo modo quando viene assegnato un task ad uno
sviluppatore, questi può lavorare indifferentemente sull’app di
sviluppo o in copia locale, per poi effettuare il push sul
repository. Per ogni task deve essere creato un branch su cui può
lavorare lo sviluppatore. Per concedere l’accesso al branch viene
usata la mail dello sviluppatore (che ovviamente deve essere
registrato su github o gitlab).</p>
<p>Per la creazione dell’ambiente di staging quindi si procederà
alla creazione di un branch staging su git e successivamente al clone
git del branch appena creato.</p>
<p>Se occorre lavorare parallelamente su più attività verranno
creati dagli sviluppatori tanti branch quante sono le attività ed al
termine dello sviluppo e test si procede al merge dei vari branch
(es. branch Frontend, branch Backend, branch API …) su staging. Una
volta collaudato tutto si fa il merge con il branch main.</p>
<p>OPM terrà traccia di ogni branch creato e cancellato dai vari
sviluppatori, oltre a quello di staging (integrazione on API di
github etc).</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
<p><br/>
<br/>

</p>
</body>
</html>
