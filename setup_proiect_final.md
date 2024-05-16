# 📝 Setup Proiect Final ITF

## Obiective
- Rezumat asteptari proiect final - partea practica
- Configurare proiect Github
- Configurare virtual environment
- Instalare dependinte + creare proiect Django
- Actualizare fisier README

## 🌟 Configurare proiect github

### ✨ Creare repository github
- Creeaza un repository pe github, in care sa
adaugi proiectul tau final.
- Asigura-te ca la crearea repository-ului, respecti urmatoarele puncte:
  - repo-ul este public.
  - repo-ul are fisierul ```README.md```
  - repo-ul are fisierul ```.gitignore```
### ✨ Clonare repository github
- Dupa crearea repository-ului, acesta va fi clonat pe local,
pentru a incepe dezvoltarea proiectului:
```bash
git clone <link_proiect_github>
```
### ✨ Setup repo
- Asigura-te ca in fisierul ```.gitignore``` incluzi
folderul ```.idea``` (folder creat de Pycharm), astfel incat,
acesta sa nu fie inclus in actualizarile repo-ului remote.
- Creeaza un fisier, numit ```requirements.txt``` in care vei
salva dependintele proiectului.

## 🌟 Configurare virtual environment

### ✨ Creare virtual environment
- ⚠️ Toate dependintele proiectului trebuie izolate intr-un virtual
environment (astfel, te asiguri ca acesta nu depinde de dependinte
externe)!
```shell
python -m venv <nume_venv>
```
- **IMPORTANT**: Daca denumirea virtual environment-ului nu este
inclusa in fisierul ```.gitignore```, asigura-te ca o incluzi. 
- **IMPORTANT**: Folder-ul ce reprezinta venv-ul creat **NU** trebuie sa ajunga in repo-ul
de pe github!
- 
### ✨ Activare virtual environment
- Dupa crearea virtual environment-ului, acesta poate fi activat:
  - OSX: ```source myenv/bin/activate```
  - Windows Powershell: ```myenv/Scripts/Activate.ps1```
  - Windows cmd/Pycharm Terminal: ```myenv/Scripts/activate.bat```
- **IMPORTANT**: Virtual environment-ul se va activa de fiecare data
cand se va rula aplicatia sau cand se vor instala dependinte
ale proiectului.

### ✨ Dezactivare virtual environment
```shell
deactivate
```

## 🌟 Instalare dependinte
- Ne asiguram ca avem virtual environment-ul activat
- Instalam libraria django:
```shell
pip install django
```
- Dupa instalare, ne asiguram ca adaugam dependintele instalate
in fisierul requirements.txt:
```shell
pip freeze > requirements.txt
```

- **IMPORTANT**: Acesti pasi se vor repeta de fiecare data cand
se instaleaza dependinte noi ale aplicatiei.

## 🌟 Creare proiect Django
- creare proiect Django:
```shell
django-admin startproject <denumire_proiect>
```
- rulare proiect Django:
```shell
python manage.py runserver
```

## 🌟 Actualizare fisier README cu pasi rulare aplicatie
- Fisierul ```README.md``` trebui sa contina instructiunile
corecte de rulare ale aplicatiei.