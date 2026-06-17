# mini_project_DS02_05_26
Kurs Data Science LearnIT - DS02-05-26 — Mini Projekt

# 📚 Instrukcja wrzucania etapów Mini Projektu

> ℹ️ To repozytorium jest **osobne** od repo z pracami domowymi (`DS02_05_26_pd`). Prace domowe z lekcji nadal wrzucasz tam, zgodnie z dotychczasowym README. Tutaj, w `mini_project_DS02_05_26`, wrzucasz **wyłącznie etapy mini-projektu** opisane na zajęciach (wybór datasetu → czyszczenie → EDA → model).

## Struktura folderów

Cały Twój projekt mieszka w **jednym** folderze nazwanym według schematu:

```
literaimienia_nazwisko
```

**Przykład:** Anna Kowalska → `a_kowalska`

W środku tego folderu, w trakcie kolejnych zajęć, będą się pojawiać kolejne pliki — każdy etap to **jeden nowy plik + jeden nowy commit**, nie nowy folder.

```
projekt/
└── a_kowalska/
    ├── README.md            ← etap 1 (po wyborze datasetu)
    ├── 01_czyszczenie.ipynb ← etap 2
    ├── 02_transformacja.ipynb ← etap 3 (część EDA)
    ├── 03_eda.ipynb           ← etap 3 (część EDA)
    └── 04_model.ipynb         ← etap 4 (finał)
```

To dokładnie struktura ze slajdu „Struktura folderu projektu" z prezentacji wprowadzającej — nic więcej nie trzeba wymyślać, wystarczy trzymać się tych nazw plików.

---

## Jak to działa w praktyce — różnice względem prac domowych

| | Prace domowe (`DS02_05_26_pd`) | Mini Projekt (`mini_project_DS02_05_26`) |
|---|---|---|
| Fork + klon | Robisz **raz na początku kursu** | Robisz **raz na początku kursu** (osobny fork tego repo) |
| Folder | Nowy folder **per lekcja** | **Jeden** folder na cały projekt |
| Commity | Jeden commit = jedna praca domowa | Jeden commit = **jeden etap projektu** (kilka commitów do tego samego folderu w trakcie kursu) |
| Pull Request | Jeden PR per praca domowa | Możesz otworzyć **jeden PR na początku** (po etapie 1) i dalej dopychać kolejne commity do tej samej gałęzi — PR sam się zaktualizuje. Szczegóły poniżej. |

---

## Krok po kroku — pierwsze wejście (etap 1: wybór datasetu)

### 1. Zrób fork repozytorium

Wejdź na stronę repo i kliknij przycisk **Fork** (prawy górny róg).

```
https://github.com/michalszlapa/mini_project_DS02_05_26
```

---

### 2. Sklonuj swojego forka na komputer

```bash
git clone https://github.com/TWOJA_NAZWA/mini_project_DS02_05_26.git
cd mini_project_DS02_05_26
```

> Zamień `TWOJA_NAZWA` na swoją nazwę użytkownika GitHub.

---

### 3. Stwórz swój folder i wrzuć pierwszy plik

Utwórz swój folder według schematu `literaimienia_nazwisko`, np.:

```
a_kowalska/
```

Wrzuć tam plik `README.md` opisujący Twój dataset: link do Kaggle + 1-2 zdania o tym, co chcesz przewidywać i jaką kolumnę widzisz jako target (to ten sam opis, który wcześniej wysyłałeś do akceptacji prowadzącemu — teraz trafia też do repo).

---

### 4. Zapisz zmiany (commit i push)

```bash
git add .
git commit -m "etap 1: wybor datasetu - Anna Kowalska"
git push
```

---

### 5. Otwórz Pull Request

1. Wejdź na GitHuba na swoje repozytorium (fork)
2. Kliknij **„Compare & pull request"**
3. Sprawdź, czy zmiany wyglądają poprawnie
4. Kliknij **„Create pull request"**

Ten PR zostaje **otwarty przez cały czas trwania projektu** — nie zamykasz go po etapie 1.

---

## Krok po kroku — kolejne etapy (2, 3, 4)

Tu jest jedyna realna różnica względem prac domowych: **nie robisz forka/klonowania/PR-a od nowa**. Wracasz do tego samego folderu na dysku i dopisujesz kolejny plik.

### 1. Dodaj nowy plik do swojego folderu

Np. po zajęciach z czyszczenia danych:

```
a_kowalska/01_czyszczenie.ipynb
```

### 2. Commit i push — tak jak poprzednio

```bash
git add .
git commit -m "etap 2: czyszczenie danych - Anna Kowalska"
git push
```

### 3. Nic więcej nie trzeba robić z PR-em

Push do tej samej gałęzi **automatycznie aktualizuje** już otwarty Pull Request — nowy commit po prostu się w nim pojawi. Nie zamykasz starego PR-a i nie tworzysz nowego.

Powtarzasz to po każdym kolejnym etapie, aż wszystkie 4 pliki (`01_czyszczenie`, `02_transformacja`, `03_eda`, `04_model`) znajdą się w Twoim folderze.

---

## ✅ Checklist po każdym etapie

- [ ] Plik trafił do **tego samego** folderu `literaimienia_nazwisko` (nie tworzysz nowego folderu)
- [ ] Nazwa pliku zgodna ze strukturą z prezentacji (`README.md`, `01_czyszczenie`, `02_transformacja`, `03_eda`, `04_model`)
- [ ] Commit ma sensowny opis etapu (np. `etap 3: EDA - Imię Nazwisko`)
- [ ] Push wykonany, a Pull Request (otwarty po etapie 1) widzi nowy commit

---

## 📅 Przypomnienie — terminy zgłoszenia datasetu

Zanim cokolwiek wrzucisz do repo, dataset musi przejść akceptację: link do Kaggle + opis targetu wysłany do prowadzącego, termin **przed zajęciami z numpy i pandas**. Dopiero zaakceptowany dataset trafia jako `README.md` do etapu 1.

---

## ❓ Pytania?

Zgłoś się do prowadzącego lub napisz na kanale kursu.
