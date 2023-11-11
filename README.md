Open Project Manager

Open Project Manager nasce per tenere sotto controllo le attività quotidiane di sviluppo e per coordinare i diversi team in diversi progetti. Coinvolge clienti, collaboratori, project manager e mira a gestire tutto il ciclo di vita del progetto. Si adatta bene allo sviluppo del software, ma può essere usato in tutti gli ambiti in cui c’è un progetto ed un team da gestire. 
N.b. 
Il progetto è in continua evoluzione per cui è passibile di cambiamenti continui sia manutentivi che evolutivi. 

Tecnologie utilizzate
Il software è sviluppato in laravel 10 con Bootstrap 5. Per l’autenticazione si è scelto Spatie. Per il resto, specialmente per l’integrazione on API esterne si vedrà strada facendo. Non viene fornito con uno di quei bellissimi template per il backend perché tanto non è destinato al pubblico, ma soprattutto non mi andava di spendere 49 dollari. Non viene sviluppato con Vue ed Inertia per 2 motivi: innanzitutto non conosco abbastanza bene Vue, in secondo luogo perché bootstrap con blade è gestibile da una maggior quantità di sviluppatori che potenzialmente potrebbero entrare a far parte del progetto. Terzo motivo, anche chi non conosce bootstrap con mezza giornata è dei nostri.
Mettiamo pure che Bootstrap garantisce che il software sia responsive, quindi può essere usato alla grande anche con tablet e smartphone anche se è evidentemente fatto per il desktop.

Ruoli e Utenti
Come attori principali abbiamo quindi:
Superadmin (ha accesso a tutte le risorse, crea gli utenti,  i ruoli, i progetti)
Il Cliente
Il Project Manager
Lo o gli sviluppatori
Il project manager ascolta il cliente sulle proprie esigenze. Il progetto può essere nuovo o manutenzione di uno attualmente esistente. 
Il project manager propone una soluzione al cliente. Previa accettazione da parte del cliente (si consiglia un documento scritto con eventuale mockup controfirmato per evitare malintesi) il project manager traduce il documento in attività da assegnare agli sviluppatori.
La prima attività è sempre quella di creare un ambiente di sviluppo condiviso su cui i programmatori lavoreranno ed il PM avrà modo di controllare l’avanzamento dei lavori. Se il progetto già esiste ed è in produzione, è consigliabile clonare l’attuale web app (staging).
Una volta creato l’ambiente il PM provvede a suddividere il progetto in attività da assegnare a uno o più sviluppatori. 
Ogni sviluppatore appartenente al progetto avrà un area di lavoro in cui saranno presenti gli accessi all’ambiente di sviluppo. 
Ogni attività (task assegnato) sarà preventivato in termini di costi e tempi di ultimazione.
Una volta valutati i task in termini di tempo, il PM sarà in grado di produrre il GANTT del progetto 
Attraverso il GANTT è possibile definire anche i SAL del progetto e quindi i relativi pagamenti.
Per gestire il versioning del software dovrebbe essere utilizzato git. In questo modo quando viene assegnato un task ad uno sviluppatore, questi può lavorare indifferentemente sull’app di sviluppo o in copia locale, per poi effettuare il push sul repository. Per ogni task deve essere creato un branch su cui può lavorare lo sviluppatore. Per concedere l’accesso al branch viene usata la mail dello sviluppatore (che ovviamente deve essere registrato su github o gitlab).
Per la creazione dell’ambiente di staging quindi si procederà alla creazione di un branch staging su git e successivamente al clone git del branch appena creato.
Se occorre lavorare parallelamente su più attività verranno creati dagli sviluppatori tanti branch quante sono le attività ed al termine dello sviluppo e test si procede al merge dei vari branch (es. branch Frontend, branch Backend, branch API …) su staging. Una volta collaudato tutto si fa il merge con il branch main.
OPM terrà traccia di ogni branch creato e cancellato dai vari sviluppatori, oltre a quello di staging (integrazione on API di github etc).













