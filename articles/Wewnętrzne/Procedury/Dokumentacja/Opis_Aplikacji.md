# DOKUMENTACJA W FORMIE PUBLICZNEJ - DOCFX, AZURE PIPELINES, GITHUB PAGES #

Poniższa dokumentacja dotyczy przykładowego rozwiązania znajdującego się pod adresem: <https://soneta.github.io/docfx-soneta/>

### FlowChart aplikacji ###

![Alt](Images/diagram1.png "Diagram1")

### Opis schematu ###

1. Tworzymy nowy projekt dokumentacji z wykorzystaniem DocFX. 
2. Za pomocą Visual Studio Code dokonujemy w nim wszelkich zmian. Inicjujemy lokalne repozytorium.
3. Następnie wykonujemy push do Github na branch master (na nim bedzie historia zmian zwiazana z zawartoscia artykułów). 
4. Po wykonaniu commita zostaje automatycznie uruchomiony pipeline na Azure DevOps, który pobiera kod z naszego repozytorium na github, buduje go generując statyczne strony dokumentacji
5. Następnie publikuje tj. wykonuje commit powrotny do naszego repozytorium na github z tym że tym razem commit dotyczy brancha gh-pages (branch który jest źródłem dla GitHub Pages). 
6. W momencie poprawnego zakończenia pracy pipeline'a oraz wykonaniu commita, strona prezentująca naszą dokumentację (GitHub Pages) zostaje uzupełniona o zmiany przez nas dokonane.

### Wskazówki ###

***DocFX***

1. Zapoznać się z dokumentacją: <https://dotnet.github.io/docfx/>
2. Stworzyć własny projekt zgodnie z instrukcją w dokumentacji

***Visual Studio Code***

1. Dostosować utworzony standardowo projekt według swoich indywidualnych preferencji i potrzeb.

    Dodatek do VSC pomagąjący w pracy z DocFX:

   * <https://marketplace.visualstudio.com/items?itemName=tintoy.docfx-assistant>

    Dodatek wspomagający pracę z plikami md:

    * <https://marketplace.visualstudio.com/items?itemName=DavidAnson.vscode-markdownlint>

    Kod źródłowy dokumentacji DocFX (przykładowy kod):

    * <https://github.com/dotnet/docfx>

    Krótkie kursy tutoriale użytkowników:

   * <https://www.youtube.com/watch?v=R4zLtuTbsBM>
   * <http://www.hardkoded.com/blog/creating-docfx-site>
  

2. Gotowy projekt zainicjować jako repozytorium git (w terminalu Visual Studio Code), a następnie zgodnie z instrukcją: <https://help.github.com/en/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line> utworzyć nowe repozytorium na GitHub oraz dostarczyć tam swój projekt.

***Github***

1. Na nowo utworzonym repozytorium na Github powinny znajdować się min. 2 branche: master (tworzony automatycznie) oraz "czysty" branch gh-pages (instrukcja utworzenia: <https://gist.github.com/ramnathv/2227408>)

2. Kolejnym krokiem powinno być skonfigurowanie Github Pages. W tym celu należy podążać zgodnie ze wskazówkami wskazanymi w dokumentacjach:
   * <https://pages.github.com/>
   * <https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site>
  
3. Następnie do github należy "podpiąć" dwie aplikacje:
   * Azure Pipelines (aplikacja umożliwiająca połączenie z Azure DevOps) 
     * <https://github.com/marketplace/azure-pipelines>
  
   * utterances (aplikacja umożliwiająca skorelowanie komentarzy artykułów na GitHub Pages z issue na GitHub)
      * <https://github.com/apps/utterances>
      * <https://utteranc.es/>

<https://developer.github.com/apps/installing-github-apps/>

***Azure DevOps***

1. W pierszym kroku należy utworzyć projekt na Azure DevOps
   * <https://docs.microsoft.com/en-us/azure/devops/organizations/projects/create-project?view=azure-devops&tabs=preview-page>

2. Następnie w zakładce pipelines tworzymy nowy pipeline oraz korelujemy go z naszym repozytorium na GitHub
   * <https://docs.microsoft.com/en-us/azure/devops/pipelines/repos/github?view=azure-devops&tabs=yaml>
   * <https://www.azuredevopslabs.com/labs/azuredevops/github-integration/>
   * <https://www.azuredevopslabs.com/labs/vstsextend/github-azurepipelines/>
  
3. W utworzonym pipeline należy wykorzystać dwa taski:
    * Budowa statycznego contentu z którego będzię korzystał GitHub Pages: <https://marketplace.visualstudio.com/items?itemName=chrismason.vsts-docfxtasks>
    * Publikacja w/w contentu powrotnie do repozytorium na github a tym samym zasilenie GitHub Pages: <https://marketplace.visualstudio.com/items?itemName=AccidentalFish.githubpages-publish>


4. W ustawieniach pipeline w zakładce Triggers ustawić automatyczne triggerowanie w przypadku pojawienia się nowego commita na branchu master.
