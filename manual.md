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

För att kunna bidra till ett projekt behöver du först klona ett repositorie.
Navigera fram till godtycklig mapp där du har dina projekt:

    cd ~/Documents/code

Använd sedan kommandot git cloneför att klona repositoriet.
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

För att lägga till en fil till din commit, använd 'git add' kommandot.

Exempel:
