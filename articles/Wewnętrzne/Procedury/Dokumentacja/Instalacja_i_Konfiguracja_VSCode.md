# Visual 1Studio Code Instalacja i konfiguracja #

## Opis narzędzia ##
Visual Studio Code jest zaawansowanym i przyjaznym użytkownikowi edytorem plików tekstowych, który dzięki bogatemu zestawowi rozszerzeń potrafi zaspokoić potrzeby praktycznie każdego użytkownika.

## Co znajdziesz w tym dokumencie ##

1. [Instalacja VS Code](##Instalacja-VS-Code##)

1. [Instalacja sprawdzania pisowni](##Instalacja-dodatku-sprawdzania-języka-polskiego##)

1. [Instalacja Git for Windows](##Instalacja-Git-for-Windows)

1. [Podłączenie do repozytorium dokumentacji](##Podłączenie-do-repozytorium-dokumentacji-git##)

1. [Instalacja rozszerzenia do pracy z Azure Dev Ops](##Połączenie-i-Praca-z-Azure-Devops##)

## Instalacja VS Code ##

1. W przeglądarce przechodzimy do [strony](https://code.visualstudio.com/download) i wybieramy User Instaler x64 Dla Windows

    ![Pobranie instaltora VS Code](Images/instaltaorVSC.png)

1. Uruchamiamy instaltor i zostawiamy język Angielski

    ![Instalacja krok 2](Images/VSCInstallStep1.png)

1. Akceptujemy licencję

    ![Instalacja krok 2](Images/VSCInstallStep2.png)

1. Wybieramy folder instalacji

    ![Instalacja krok 3](Images/VSCInstallStep3.png)

1. Wybieramy nazwę w Menu Start

    ![Instalacja krok 4](Images/VSCInstallStep4.png)

1. Wybieramy dodatkowe parametry

    ![Instalacja krok 5](Images/VSCInstallStep5.png)

1. Przeprowadzamy instalcje

    ![Instalacja krok 6](Images/VSCInstallStep6.png)

1. Gotowe - uruchamiamy VS Code w celu dalszej konfiguracji

    ![Instalacja krok 7](Images/VSCInstallStep6.png)

## Instalacja dodatku sprawdzania języka polskiego ##

1. Aby przejść do zarządzania rozszerzeniami używamy sktóru ctrl+shift+x albo klikamy na lewym pasu ikonę

    ![Ikona rozszerzeń](Images/extentions_icon.png)

1. Wpiszujamy wyraz *polish* i w znalezionym rozszerzeniu *Polish Support for LenguageTool* klikamy VSCInstallStep1

    ![Polish Support](Images/polish_ex.png)

1. Musimy jeszcze zainstalować (może już być zainstalowany) dodatek *LanguageTool for Visual Studio Code* więc wpisujemy jego nazwę do wyszukiwania

    ![LanguageTool](Images/ln_tool.png)

1. Przechodzimy do ustawień za pomocą skrótu ctrl+, bądź korzystająć z ikony zarządzania na lewym pasu i wybierając opcje Settings

    ![LanguageToolcfg](Images/settings.png)

1. W wyszukiwaniu wpisujemy *languageTool* Ustawiamy język na pl - gotowe.

    ![LanguageToolcfg2](Images/lan_tool_set.png)

1. Jeżeli na komputrzenie nie ma zainstalowanej Java (min wersja 8.0) należy doinstalować -> [Instaltor](https://javadl.oracle.com/webapps/download/AutoDL?BundleId=239827_230deb18db3e4014bb8e3e8324f81b43)

## Instalacja Git for Windows ##

1. Instalujemy na komputerze [Git for Windows](https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/Git-2.23.0-64-bit.exe) 

1. Akceptujemy licencje

    ![GitInstallSetp1](Images/gitinstallstep1.png)

1. Wybieramy katalog instalacji

    ![GitInstallSetp2](Images/gitinstallstep2.png)

1. Zostawiamy domyślnie zaznaczone opcje

    ![GitInstallSetp3](Images/gitinstallstep3.png)

1. Wybieramy folder w menu start

    ![GitInstallSetp4](Images/gitinstallstep4.png)

1. Wybieramy VS Code jako domyślny edytor dla Git

    ![GitInstallSetp5](Images/gitinstallstep5.png)

1. Zostawiamy domyślną opcje używania git w lini poleceń

    ![GitInstallSetp6](Images/gitinstallstep6.png)

1. Zostawiamy domyślną opcje dla protokołu HTTPS

    ![GitInstallSetp7](Images/gitinstallstep7.png)

1. Zostawiamy domyślną opcje konwersji końca lini

    ![GitInstallSetp8](Images/gitinstallstep8.png)

1. Ustawiamy linie poleceń widnows

    ![GitInstallSetp9](Images/gitinstallstep9.png)

1. Dodatkowe opcje zostawiamy domyślne

    ![GitInstallSetp10](Images/gitinstallstep10.png)

1. Nie włączamy eksperymentalnych opcji i instalujemy i gotowe.

    ![GitInstallSetp11](Images/gitinstallstep10.png)


## Podłączenie do repozytorium dokumentacji git ##

1. Przechodzimy w przeglądarce do [witryny](https://dev.azure.com/soneta/Soneta/_git/dokumentacja.git)

1. Używamy przycisku *Colne* w prawej sekcji witryny i klikamy przycisk Clone in VS Code

    ![Clone](Images/clone.png)

1. Potwierdzamy otwarcie VS Code

1. Zezwalamy na otwarcie url

    ![AllowVSC](Images/allowVSC.png)

1. Wyniremalu folder trzymania repozytorium np. *D:\repos\dokumentacja* i klikamy przycisk *select reposytory lokalization*

1. Nastąpi krótkotrwały proces klonowania repozytorium po jego zakończeniu wybieramy opcję Open

    ![openrepo](Images/openrepo.png)

1. Gotowe - możemy pracować na repozytorium

    ![repo](Images/openrepo.png)



1. Uruchamiamy VS Code i z Menu Terminal uruchamiamy NewTerminal można zastosować sktót ctrl+shift+`

    ![Terminal](Images/terminal.png)

1. 

## Połączenie i Praca z Azure DevOps ##

1. Instalujemy rozszerzenie *Azure Repos*

    ![AzureReposEx](Images/azurereposex.png)


