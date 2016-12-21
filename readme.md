# AlgebraCook Laravel

Vježba iz naprednog PHP web programiranja korištenjem aplikacijskog okvira Laravel.

## Tražene funkcionalnosti

		 - popis recepata
		 - form za unos recepta
		 - spremanje recepta u bazu
		 
		 - prikaz odabranog recepta
		 
		 - form za izmjenu odabranog recepta
		 - spremanje izmijenjenog recepta u bazu
		 
		 - registracija korisnika
		 - prijava korisnika
		 - promjena lozinke


		 
## Zavisnosti

        PHP ->=5.6.4
        laravel/framework 5.3.*
        laravelcollective/html 5.3



## Zadatak
__Sustav za autentifikaciju__ _php artisan make:auth_ __je dodan te ga ne treba dodavati.__
Općenito vrijedi da ne trebate ništa brisati, dakle u inicijalnom projektu ništa nije 'višak'.
__Paket__ _laravelcollective/html_ __je dodan i ne trebate ga dodavati!__
__

1. Odrediti potrebne modele/tablice za bazu, koncept aplikacije, organizaciju direktorija...

1. Stvoriti migracijske datoteke i modele za Recipe i Ingredient
 * urediti modele tako da je Recipe svjestan svojih Ingredient-a i korisnika koji ga je stvorio
 * urediti migracijske datoteke tako da tablice imaju sve potrebne stupce unutar tablica

1. Napraviti odgovarajuće page views:
		
		resources\views\layouts\app.blade.php - dodati potrebno
		resources\views\recipes - stvoriti potrebne views za popis, edit, dodavanje, prikaz recepata

		
1. Definirati potrebne route (route za autentifikaciju i User rute su dodane i ne treba ih mijenjati/dodavati).
		
		routes\web.php

		
1. Stvoriti odgovarajuće kontrolere za Recipe i User (php artisan make:controller) sa potrebnim metodama
		
		app\Http\Controllers
		

1. Ukoliko već niste - registrirajte se na GitHub.com, i stvorite novi repozitorij AlgebraCook.

 * podesite Vaš repozitorij da bude origin projekta:
		
		git remote set-url origin https://github.com/VASEKORISNIKOIME/AlgebraCook.git

 * dodajte datoteke u index:
		
		git add -A

 * napravite commit:
		
		git commit -m 'inicijalni commit'

 * uploadajte promjene na GitHub repo (upišite username/pass kad Vas zatraži):
		
		git push

 * provjertite status:
		
		git status
		

1. Stvorite novi _branch_ (granu), i dodajte funkcionalnost brisanja recepata
		
		git branch deleteft
		git checkout deleteft

 * napravite merge i commit na Vaš GitHub repo:
		
		git checkout master
		git merge deleteft
