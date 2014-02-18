# En supersnabb git guide.

## Hur installerar jag git?

### Linux

Skoldatorerna har det, om du vill ladda ner det hemma så kan du använda valfri pakethanterare.

### Mac

Native git finns tillängligt på följande länk:

https://help.github.com/articles/set-up-git#platform-mac

### Windows

Var inte löjlig.

## Hur använder jag git?

För att kunna bidra till ett projekt behöver du först klona ett *repository*.
Navigera fram till den mapp där du har dina projekt:

    cd ~/Documents/code

Använd sedan kommandot git clone för att klona repositoriet.
Exempel:

    git clone https://github.com/3amice/git-exempel.git

Du kommer nu ha en lokal klon av repositoriet 3amice/git-exempel.

Använd kommandot "touch" för att skapa en fil.

		touch fil.txt

För att se hur detta påverkade repositoriet använd 'git status'-kommandot

		git status

Exempel:

		[meris@meris-stat git-exempel]$ touch fil.txt
		[meris@meris-stat git-exempel]$ git status
		On branch master
		Your branch is up-to-date with 'origin/master'.

		Untracked files:
			(use "git add <file>..." to include in what will be committed)

				fil.txt

		nothing added to commit but untracked files present (use "git add" to track)

Om du vill uppdatera repositoriet som ligger på servern måste du skicka
dina uppdateringar i en *commit*.
En commit är ett paket som innehåller ett log-meddelande samt deltan, alltså endast skillnader
gentemot den senaste commiten du har lagrad på ditt lokala repositorie.
För att lägga till en fil till din commit, använd 'git add' kommandot.

Exempel:

		[meris@meris-stat git-exempel]$ git add fil.txt 
		[meris@meris-stat git-exempel]$ git status
		On branch master
		Your branch is up-to-date with 'origin/master'.

		Changes to be committed:
			(use "git reset HEAD <file>..." to unstage)

				new file:   fil.txt

För att nu skapa en commit och ge den ett meddelande kan du exempelvis göra såhär:

Exempel:

		[meris@meris-stat git-exempel]$ git commit fil.txt -m "Hejsan! Idag har jag lärt mig använda git! vad kul."
		[master 7698a98] Hejsan! Idag har jag lärt mig använda git! vad kul.
		 1 file changed, 0 insertions(+), 0 deletions(-)
		create mode 100644 fil.txt

Använder du nu 'git status' kommandot kommer det se ut som såhär:

		[meris@meris-stat git-exempel]$ git status
		On branch master
		Your branch is ahead of 'origin/master' by 1 commit.
		(use "git push" to publish your local commits)

För att synkronisera dina andringar mot servern (så att andra har tillgång till dina bidrag) får du *pusha* upp dina commits.
Lämpligt nog finns ett kommando som heter git push.

Exempel:

		git push origin master

eller bara:

		git push

Du kan även synkronisera servern mot dig, detta innebär att du ibland får merge-konflikter.
Dessa är oftast triviala och git sköter det själv. I det fallet att git inte vågar sköta konflikten
så får du ta kontakt med den som senast ändrade filen.

Exempel på git pull:

		git pull

Du kan kolla commit-loggen såhär:

		git log
	
#Frågor? Hit me.

