# Rehabilitacja narządu ruchu – protokoły z kodami ICD-9 PL

Statyczna strona (jeden plik `index.html`, bez zależności i bez kroku budowania) do przeglądania protokołów rehabilitacji:
złamania leczone zachowawczo, choroby zwyrodnieniowe, stany po alloplastyce stawów i po operacyjnym leczeniu złamań.
Każde schorzenie ma fazy rehabilitacji z kinezyterapią i fizykoterapią przypisaną do kodów ICD-9 PL.

## Publikacja na GitHub Pages

**Wariant A – GitHub Actions (zalecany, plik workflow jest w repozytorium)**
1. Utwórz nowe repozytorium na GitHubie i wypchnij zawartość tego folderu na gałąź `main`:
   ```bash
   git init
   git add .
   git commit -m "Pierwsza wersja"
   git branch -M main
   git remote add origin https://github.com/<uzytkownik>/<repozytorium>.git
   git push -u origin main
   ```
2. W repozytorium: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. Po zakończeniu akcji „Deploy to GitHub Pages” strona będzie dostępna pod adresem
   `https://<uzytkownik>.github.io/<repozytorium>/`.

**Wariant B – bez Actions**
W **Settings → Pages** wybierz *Deploy from a branch*, gałąź `main`, folder `/ (root)`.

## Uruchomienie lokalne
Otwórz `index.html` w przeglądarce albo:
```bash
python3 -m http.server 8000
```

## Linki bezpośrednie
Każde schorzenie ma własny adres, np. `#tka`, `#tep-biodro`, `#gonartroza`; słownik kodów: `#slownik`.

## Zastrzeżenie
Materiał poglądowy dla fizjoterapeutów i lekarzy. Obciążanie, zakresy ruchu i terminy ustala lekarz prowadzący lub operator.
Nazwy procedur wg słownika ICD-9 PL (wersja obowiązująca od 01.01.2025). Kody 79.02, 79.15 i 79.16 przyjęto wg schematu
numeracji rozdziału 79 – przed sprawozdawaniem świadczeń sprawdź je w aktualnej wersji słownika NFZ.
