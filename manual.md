# En supersnabb git guide.

## Hur installerar jag git?

### Linux

Skoldatorerna har det, om du vill ladda ner det hemma så kan du använda valfri pakethanterare.

Exempel:

#### Archderiverade distros

		 # pacman -S git
#### Ubuntusmaker

		 # apt-get install git

### Mac

Native git finns tillängligt på följande länk:

https://help.github.com/articles/set-up-git#platform-mac

När du väl laddat ner och installerat det är det bara 
att börja använda det från terminalemulatorn.

### Windows

Var inte löjlig.

## Hur använder jag git?

För att kunna bidra till ett projekt behöver du först klona ett repositorie.
Navigera fram till godtycklig mapp där du har dina projekt:

    cd ~/Documents/code

Använd sedan kommandot $git clone$ för att klona repositoriet.
Exempel:

    git clone https://github.com/3amice/git-exempel.git

Du kommer nu ha en lokal klon av repositoriet 3amice/git-exempel.

Använd kommandot $touch$ för att skapa en fil.
