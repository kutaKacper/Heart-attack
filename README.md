# Dokumentacja projektu

## Opis struktury projektu
Projekt składa z dwóch plików:
1. heart_2022_with_nans.csv – Plik danych w formacie CSV, który zawiera 445132 wierszy z informacjami dotyczącymi zdrowia Amerykanów pozyskanymi w wyniku ankiet. Dane pobrane zostały z: [https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease)
2. heart_attack_prediction.ipynb – Notatnik Jupyter Notebook, który zawiera cały proces analizy danych.

Pliki projektowe działają na wersji Python==3.10.6.
W celu zainstalowania potrzebnych bibliotek, wykorzystaj kod `pip install -r requirements.txt`


## Opis kolumn
1. State (Stan) – Stan, w którym znajduje się respondent, oznaczony kodem FIPS.
2. Sex (Płeć) – Zadeklarowana płeć respondenta (mężczyzna lub kobieta).
3. GeneralHealth (Ogólny stan zdrowia) – Subiektywna ocena ogólnego stanu zdrowia respondenta.
4. PhysicalHealthDays (Dni złego stanu fizycznego) – Liczba dni w ciągu ostatnich 30, w których stan fizyczny respondenta był zły.
5. MentalHealthDays (Dni złego stanu psychicznego) – Liczba dni w ciągu ostatnich 30, w których stan psychiczny respondenta był zły.
6. LastCheckupTime (Ostatnia wizyta kontrolna) – Czas, jaki upłynął od ostatniej rutynowej wizyty u lekarza.
7. PhysicalActivities (Aktywność fizyczna) – Czy respondent podejmował aktywność fizyczną poza pracą w ciągu ostatniego miesiąca.
8. SleepHours (Godziny snu) – Średnia liczba godzin snu na dobę.
9. RemovedTeeth (Usunięte zęby) – Liczba zębów usuniętych z powodu próchnicy lub choroby dziąseł (nie licząc urazów lub leczenia ortodontycznego).
10. HadHeartAttack (Przebyte zawały serca) – Czy respondent kiedykolwiek miał zawał serca (zdiagnozowany przez lekarza).
11. HadAngina (Dławica piersiowa) – Czy respondent kiedykolwiek miał dławicę piersiową lub chorobę wieńcową.
12. HadStroke (Przebyte udary) – Czy respondent kiedykolwiek przeszedł udar.
13. HadAsthma (Astma) – Czy respondent kiedykolwiek miał zdiagnozowaną astmę.
14. HadSkinCancer (Rak skóry) – Czy respondent kiedykolwiek miał zdiagnozowany rak skóry.
15. HadCOPD (POChP) – Czy respondent kiedykolwiek miał przewlekłą obturacyjną chorobę płuc (POChP), rozedmę lub przewlekłe zapalenie oskrzeli.
16. HadDepressiveDisorder (Zaburzenia depresyjne) – Czy respondent kiedykolwiek miał zdiagnozowane zaburzenie depresyjne.
17. HadKidneyDisease (Choroba nerek) – Czy respondent kiedykolwiek miał zdiagnozowaną chorobę nerek (nie licząc kamieni nerkowych, infekcji pęcherza lub nietrzymania moczu).
18. HadArthritis (Zapalenie stawów) – Czy respondent kiedykolwiek miał zdiagnozowane zapalenie stawów, w tym reumatoidalne zapalenie stawów, toczeń lub fibromialgię.
19. HadDiabetes (Cukrzyca) – Czy respondent kiedykolwiek miał zdiagnozowaną cukrzycę.
20. DeafOrHardOfHearing (Niedosłuch lub głuchota) – Czy respondent jest głuchy lub ma poważne trudności ze słuchem.
21. BlindOrVisionDifficulty (Problemy ze wzrokiem) – Czy respondent jest niewidomy lub ma poważne trudności ze wzrokiem, nawet w okularach.
22. DifficultyConcentrating (Trudności z koncentracją) – Czy respondent ma poważne trudności z koncentracją, zapamiętywaniem lub podejmowaniem decyzji z powodu fizycznej, psychicznej lub emocjonalnej kondycji.
23. DifficultyWalking (Trudności w chodzeniu) – Czy respondent ma poważne trudności z chodzeniem lub wchodzeniem po schodach.
24. DifficultyDressingBathing (Trudności w ubieraniu i kąpieli) – Czy respondent ma trudności z ubieraniem się lub kąpielą.
25. DifficultyErrands (Trudności w samodzielnym wykonywaniu obowiązków) – Czy respondent ma trudności z samodzielnym wykonywaniem codziennych obowiązków, takich jak wizyty u lekarza czy zakupy, z powodu fizycznych, psychicznych lub emocjonalnych problemów.
26. SmokerStatus (Status palenia) – Status palenia respondenta (codzienny palacz, okazjonalny palacz, były palacz, osoba niepaląca).
27. ECigaretteUsage (Używanie e-papierosów) – Historia używania e-papierosów przez respondenta i jego aktualny status.
28. ChestScan (Prześwietlenie klatki piersiowej) – Czy respondent kiedykolwiek miał wykonane badanie tomografii komputerowej (CT/CAT) klatki piersiowej.
29. RaceEthnicityCategory (Kategoria rasowo-etniczna) – Deklarowana przynależność rasowa lub etniczna respondenta.
30.AgeCategory (Kategoria wiekowa) – Przypisana kategoria wiekowa respondenta na podstawie ustalonej klasyfikacji.
31. HeightInMeters (Wzrost w metrach) – Zadeklarowany wzrost respondenta w metrach.
32. WeightInKilograms (Waga w kilogramach) – Zadeklarowana waga respondenta w kilogramach.
33. BMI (Indeks masy ciała - BMI) – Wskaźnik masy ciała (BMI) obliczony na podstawie wzrostu i wagi.
34. AlcoholDrinkers (Spożywanie alkoholu) – Czy respondent spożywał alkohol w ciągu ostatnich 30 dni.
35. HIVTesting (Test na HIV) – Czy respondent kiedykolwiek był testowany na obecność wirusa HIV.
36. FluVaxLast12 (Szczepienie na grypę w ostatnim roku) – Czy respondent otrzymał szczepionkę na grypę w ciągu ostatnich 12 miesięcy.
37. PneumoVaxEver (Szczepienie na zapalenie płuc) – Czy respondent kiedykolwiek otrzymał szczepionkę przeciwko pneumokokom (zapalenie płuc).
38. TetanusLast10Tdap (Szczepienie przeciw tężcowi w ostatnich 10 latach) – Czy respondent otrzymał szczepienie przeciwko tężcowi w ciągu ostatnich 10 lat i czy było to Tdap (szczepionka przeciwko tężcowi, błonicy i krztuścowi).
39. HighRiskLastYear (Zachowania wysokiego ryzyka w ostatnim roku) – Czy respondent w ciągu ostatniego roku angażował się w zachowania wysokiego ryzyka zakażenia HIV (np. używanie narkotyków dożylnie, leczenie chorób przenoszonych drogą płciową, wymiana pieniędzy lub narkotyków za seks).
40. CovidPos (Pozytywny wynik testu na COVID-19) – Czy respondent kiedykolwiek miał pozytywny wynik testu na COVID-19 potwierdzony przez lekarza lub innego pracownika medycznego.
