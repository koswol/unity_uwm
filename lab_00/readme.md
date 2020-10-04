# Lab 00 - Instalacja i konfiguracja środowiska UNITY

## 1. Instalacja UNITY

Unity występuje w kilku wersjach (więcej pod adresem https://unity3d.com/unity/faq) w zależności od wielkości organizacji i przychodów, które osiąga w danym roku. Wersja, która będzie wykorzystywana w trakcie zajęć to edycja Personal. 
Możliwa jest instalacja wielu wersji UNITY na jednym koncie użytkownika systemu operacyjnego i dlatego zarządzanie wersjami oraz projektami UNITY odbywa się poprzez dodatkowe oprogramowanie - **Unity Hub**. 

Aby korzystać w pełni z oprogramowania Unity należy założyć konto na portalu unity.com i założenie tzw. **Unity ID**.

Wersję Personal pobieramy przechodząc kolejno na stronę https://unity.com/, następnie "GET STARTED", zakładka "Individual" i ponownie przycisk "Get Started" wersji Personal. Środowisko można pobrać z gotowymi projektami mikro gier, ale tym razem wybieramy opcję "Returning users". Projekty mikro gier można pobrać w dowolnym momencie po zainstalowaniu środowiska. Po przejściu na kolejną stronę zgadzamy się (lub nie :) ) na warunki świadczenia usług i pobieramy Unity Hub. Po jego instalacji i uruchomieniu możemy wybrać jedną z czterech kategorii: 
* Projects
* Learn
* Community
* Installs

Opcję dostępne w **Projects** pozwalają przeglądać istniejące peojekty, dodawać nowe lub zmienić wersję środowiska UNITY istniejącego projektu (tutaj nie zawsze wszystko musi pójść zgodnie z planem).

Część **Learn** pozwala na dodanie istniejących projektów gier, stworzonych w celach edukacyjnych. Wystarczy wybrać projekt i opcję "DOWNLOAD PROJECT". Warto zwrócić uwagę na wersję Unity, dla której projekt został stworzony, będzie to gwarancja kompatybilności.

**Community** to zbiór przydatnych linków do materiałów dla i od społeczności zgromadzonej wokół Unity.

Ostatnia, ale nie najmniej ważna opcja, to **Installs** gdzie możemy pobrać i zainstalować kolejne wersje środowiska, odinstalować istniejące lub zarządzać modułami dla konkretnej zainstalowanej wersji.

W trakcie zajęć wykorzystywana będzie wersja 2019.4.** LTS. Jest to wersja o długim wsparciu technicznym. Pobranie i instalacja wymaga sporo czasu (dużo zależy od szybkości łącza internetowego) i miejsca dyskowego więc należy wybrać miejsce z wystarczająco dużą ilością wolnego miejsca. Moduły, które wybieramy na początku to:
* **Windows Build support**, **Linux build support** lub **Mac build support** w zależności od używanego systemeu operacyjnego,
* **Microsoft Visual Studio 2019 Community**,
* **Documentation**.

API Unity napisane jest w języku C# i można wybrać inny edytor niż **Visual Studio 2019 Community**, ale to rozwiązanie ze względu na oficjalne wsparcie wydaje się dobrym połączeniem na start i będzie wykorzystywane w trakcie zajęć. Jendak używanie MonoDevelop czy też Visual Studio Code nie powinno powodować większych problemów. 


## 2. Konfiguracja systemu Git dla projektu Unity

Jeżeli nie pracowałeś/-ał wcześniej z systemem Git, możesz zapoznać się z informacjami i konfiguracji oraz podstawowych poleceniach przedstawionych w dokumencie [konfiguracja_git](konfiguracja_git.md).

Korzystanie z systemów kontroli wersji jest w dzisiejszych czasach absolutnym standardem. Unity w trkacie naszej pracy nad projektem "produkuje" wiele plików tymczasowych, plików binarnych, których ani nie będziemy potrzebować w gotowej już grze, ani nie chcemy marnować czasu na ich synchronizację ze zdalnym repozytorium. Dlatego w naszych projektach (mimo, że docelowo może nie pojawić się wiele dużych plików) wykorzystamy wersję Git LFS (Large File Storage), która została stworzona specjalnie dla takich sytuacji. Wersję dla systemy Windows i krótką instrukcję instalacji znajdziemy pod adresem [https://git-lfs.github.com/](https://git-lfs.github.com/). Dodatkowo wykorzystamy plugin GitHub for Unity, który ułatwi nam pracę z Unity i Git-em oraz utworzy odpowiedni plik **.gitignore**, który usprawni i przyspieszy pracę z repozytorium poprzez redukcję ilości plików zarządzanych przez system Git.

* Krok 1 - pobranie i instalacja Git LFS, ale nie musimy jeszcze konfigurować naszego repozytorium.
* Krok 2 - pobieramy plugin GitHub for Unity - więcej informacji tutaj [https://unity.github.com/](https://unity.github.com/)
* Krok 3 - utworzenie projektu i inicjalizacja repozytorium.

Alternatywnie można też wykorzystać wskazów z poniższego artykułu [https://thoughtbot.com/blog/how-to-git-with-unity](https://thoughtbot.com/blog/how-to-git-with-unity).
