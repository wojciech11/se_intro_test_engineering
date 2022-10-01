# Podstawy Python do ćwiczeń

1. Przygotujemy nasz projekt:

   ```bash
   # jeśli pracujemy na współdzielonej maszynie
   mkdir -p GIT_USERNAME/nauka_pythona
   cd GIT_USERNAME/nauka_pythona
   ```

   ```bash
   # a jeśli na twoim komputerze:
   mkdir -p workspace/nauka_pythona 
   cd workspace/nauka_pythona
   ```

2. Przygotuj swoje środowisko pracy - atom do edycji (pozamykaj wszystkie niepotrzebne okna), poniżej konsola do uruchomienia naszego programu :
 
    ```bash
    atom .
    ```

    Jeśli `atom` nie jest zainstalowany, wykonaj następującą komendę (na podstawie [dokumentacji](https://snapcraft.io/install/atom/ubuntu)): `sudo snap install atom --classic`.

3. Utwórz plik main.py:

    ```python
    print("Hello World!)
    ```

    W konsoli uruchom swój pierwszy program:

    ```bash
    python3 main.py
    ```

4. Typy Danych

   1. Wprowadzenie do zmiennych 1:

      ```python
      imie = "Natalia"
      print("Hello World!" + imie)
      ```

   2. Wprowadzenie do zmiennych 2
   
      ```python
      imie = "Wiktoria"
      ilosc_ksiazek = 10
      srednia = 4.5
   
      print("Hello World!" + imie)
      print("Ma " + str(ilosc_ksiazek))
      print("Srednia: " + str(srednia))
      ```
   
      Zmodyfikuj powyższy program, aby był o czymś innym, np:, samochodach, samolotach.
   
      Pamiętaj o nazewnictwie zmiennych: **snake_case**, a nie camelCase.

3. Funkcje string:

   ```python
   marka = "Pegout"
   ilosc_drzwi = 5
   pojemność = 1.3
   
   marka_up = marka.upper()
   
   print("Samochod " + marka + " ma " + str(ilosc_drzwi) + " dzwi")
   print(marka_up)
   print("Pojemnosc po zmianach: {0}".format(pojemnosc * 2))
   ```
   
   Korzystając z dokumentacji, znajdź funkcję, która zmieni wszystkie litery w nazwie samochodu na małe litery.

   Wykorzystaj dodatkowo dowolną funkcję, którą znajdziesz w dokumentacji.

4. Własne funkcje.

5. Bezpieczna instalacja bibliotek z wirtualnym środowiskiem Pythona:

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   # powinna się pojawić w nawiasach
   # nazwa wirtualnego srodowiska:
   # (.venv) $
   pip install -U behave
   ```

   ```bash
   deactivate
   # zauważ, że nie ma (.venv) w prompt
   ```

   ```bash
   # upenij się, że jesteś w katalogu projektu
   pwd
   ls

   source venv/bin/activate
   # jest (.venv) w prompt
   ```
