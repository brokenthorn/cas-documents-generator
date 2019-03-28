# Generator de cereri de înregistrare a certificatelor digitale la C.A.S.
Acest generator folosește template-urile oficiale ale caselor de asigurări de sănătate în format Microsoft Word și certificate digitale publice exporate în format [DER encoded](https://en.wikipedia.org/wiki/X.690#DER_encoding) pentru a genera cereri completate cu toate datele cerute.

# CAS-TL
În folderul CAS-TL se află generatorul pentru C.A.S. Tulcea.

Numele, prenumele și CNP-ul trebuiesc completate direct în scriptul Python. Datele se află într-un array de tuples, de forma `[("prenume", "nume", "cnp"),...]`.

Numele și prenumele trebuie să fie în forma exactă prezentă în certificat pentru a fi găsite. Scriptul va genera câte un fișier în folderul creat automat numit `output`, pentru fiecare fișier `.cer` din folderul `input`.

Nu uitați să instalați toate dependențele cu `pipenv install`.
