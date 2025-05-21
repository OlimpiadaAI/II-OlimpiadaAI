# II Olimpiada Sztucznej Inteligencji / 2nd Polish AI Olympiad
<p align="center">
  <img src="logo_oai.png" alt="LogoIIOAI" width="30%">
</p>

Witamy w repozytorium z zadaniami II Olimpiady Sztucznej Inteligencji. Olimpiada ta jest skierowana do uczniów w Polsce, zarówno ze szkół średnich jak i podstawowych, którzy są zainteresowani sztuczną inteligencją. Celem jest zwiększenie zainteresowania AI i wyłonienie składów reprezentacji na olimpiady międzynarodowe [IOAI](https://ioai-official.org/) w Pekinie (2-9 sierpnia 2025) i [IAIO](https://www.iaio-official.org/) w Lublanie.

## Informacje ogólne
**Strona główna:** [Olimpiada Sztucznej Inteligencji](https://oai.cs.uni.wroc.pl/edycje/ii-oai)

Druga edycja Olimpiady odbędzie się w trzech etapach:
- Pierwszy etap, online, 17.02 - 22.03.2025. 
- Drugi etap, regionalny w 4 miastach: Kraków, Poznań, Warszawa i Wrocław, 26 - 27.04.2025 
- Trzeci etap, finał we Wrocławiu, 30.05 - 02.06.2025. 

Regulamin jest dostępny na naszej [stronie](https://oai.cs.uni.wroc.pl/regulamin).

Oficjalnym kanałem komunikacji z uczestnikami będzie platforma Discord. Dostęp do niej otrzymują uczestnicy po dokonaniu rejestracji.

## Zadania
W ramach pierwszego etapu Olimpiady uczestnicy zmierzą się z następującymi wyzwaniami:
1. **Maszynka do Liczenia Monet** - Detekcja monet z wykorzystaniem modeli wizyjnych.
1. **Wykrywanie Halucynacji** - Wykrywanie halucynacji modeli językowych w odpowiedziach na pytania.
1. **Wykrywanie Zaburzeń Sygnału EKG** - Wykrywanie anomalii w danych EKG.
1. **Zaszumienie w Etykietach Danych** - Trenowanie modeli z zaszumionymi etykietami.
1. **Ukryte Podciągi** - Identyfikacja zależności w binarnych ciągach znaków.

W drugim etapie uczestnicy rywalizowali rozwiązując nastepujące zadania:

1. **Rozkład Nienormalny** - Usuwanie i klasyfikacja różnych rodzajów szumu na obrazie.
1. **Kredytobranie** - Znajdowanie kierunków w przestrzeni danych najskuteczniej zmieniających decyzje klasyfikatora.
1. **Ekstrakcja Źródeł** - Dobór embeddingów użytecznych w wyszukiwaniu tekstów źródłowych.

## Sposób oddawania zadań
W pierwszym etapie uczestnicy rozwiązywali zadania samodzielnie i przesyłali je do Komitetu Merytorycznego za pomocą Platformy Konkursowej. Dostęp do niej jest udostępniany uczestnikom po rejestracji. Każde zadanie wymagało przesłania pliku Jupyter Notebook z rozwiązaniem. Wszystkie prace zostały oceniane automatycznie na Platformie Konkursowej.

## Środowisko
Lista dopuszczalnych pakietów znajduje się w pliku `environment.yml`, osobno dla każdego zadania. Rozwiązania były testowane przy użyciu Pythona 3.11. Na potrzeby pracy nad zadaniami, zalecamy wykorzystanie środowiska online [Google Colab](https://colab.google/). lub stworzenie środowiska lokalnego z wykorzystaniem [Anacondy](https://docs.anaconda.com/) (instrukcję instalacji środowiska z pliku YML znajdziesz [tutaj](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file)).

> Uwaga: To samo rozwiązanie uruchomione w środowisku lokalnym lub Google Colab może zwracać inne wyniki niż na Platformie Konkursowej. Ostateczna ocena Twojego zadania zostanie wyliczona na Platformie Konkursowej.

## Kryteria oceny
Oceny za zadania zostaną wyliczone na podstawie podanych w treściach zadań kryteriów. Za każde zadanie w pierwszym etapie uczestnicy mogą zdobyć maksymalnie 100 punktów.

## Licencje
Repozytorium korzysta z następujących zasobów objętych licencjami:
### 1 etap
- [**ChatGPT**](https://openai.com/policies/terms-of-use/) - obrazy w zadaniach 2, 3 i 5, pytania ze zbioru danych w zadaniu 2.
- [**OpenArt.ai**](https://openart.ai/terms/) - obraz w zadaniu 4.
- [**Flux**](https://github.com/black-forest-labs/flux/blob/main/model_licenses/LICENSE-FLUX1-dev) - obraz w zadaniu 1.
- [**Gemma**](https://github.com/google-deepmind/gemma?tab=Apache-2.0-1-ov-file) - odpowiedzi na pytania ze zbioru danych w zadaniu 2.
- [**Google Gemini**](https://ai.google.dev/gemini-api/terms) - zbiór danych w zadaniu 3, który następnie uległ modyfikacjom.
- [**MedMNIST**](https://medmnist.com/) - zbiór danych w zadaniu 4, który następnie uległ modyfikacjom.

### 2 etap
- [**ChatGPT**](https://openai.com/policies/terms-of-use/) - obrazy w zadaniach.
- [**SGPT-125M**](https://github.com/Muennighoff/sgpt/blob/main/LICENSE) - Model użyty w zadaniu Ekstrakcja Źródeł.
- [**SciFact**](https://github.com/allenai/scifact) - Zbiór danych użyty w zadaniu Ekstrakcja Źródeł. Zbiór został zmodyfikowany poprzez wybranie podzbioru zdań oraz odrzucenie dodatkowych anotacji jeśli występowała więcej niż jedna. Korpusy pochodzą ze zbioru [S2ORC](https://github.com/allenai/s2orc).

```
@article{muennighoff2022sgpt,
  title={SGPT: GPT Sentence Embeddings for Semantic Search},
  author={Muennighoff, Niklas},
  journal={arXiv preprint arXiv:2202.08904},
  year={2022}
}

@inproceedings{Wadden2020FactOF,
  title={Fact or Fiction: Verifying Scientific Claims},
  author={David Wadden and Shanchuan Lin and Kyle Lo and Lucy Lu Wang and Madeleine van Zuylen and Arman Cohan and Hannaneh Hajishirzi},
  booktitle={EMNLP},
  year={2020},
}

@inproceedings{lo-wang-2020-s2orc,
    title = "{S}2{ORC}: The Semantic Scholar Open Research Corpus",
    author = "Lo, Kyle  and Wang, Lucy Lu  and Neumann, Mark  and Kinney, Rodney  and Weld, Daniel",
    booktitle = "Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics",
    month = jul,
    year = "2020",
    address = "Online",
    publisher = "Association for Computational Linguistics",
    url = "https://www.aclweb.org/anthology/2020.acl-main.447",
    doi = "10.18653/v1/2020.acl-main.447",
    pages = "4969--4983"
}
```


## Kontakt
W razie pytań lub wątpliwości, prosimy o kontakt przez platformę Discord lub e-mail: [oai@cs.uni.wroc.pl](mailto:oai@cs.uni.wroc.pl).

Życzymy powodzenia w rozwiązywaniu zadań!

## Partnerzy instytucjonalni 

<p align="center">
  <a href="https://www.gov.pl/web/cyfryzacja" target="_blank">
    <img src="logo_mc.png" alt="Logo Ministerstwa Cyfryzacji" height="80" style="margin-right: 40px;">
  </a>
  <img src="logo_wca.png" alt="Logo Wrocławskiego Centrum Akademickiego" height="80">
</p>
