# Git Muistio

![GitLab, kuva](https://images.unsplash.com/photo-1531030874896-fdef6826f2f7?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2670&q=80)


## Komennot;

### Peruskomennot:
> #### git add
> 
>>Lisää määritellyt tiedostot indeksiin.
 
> #### git commit -m "Commit viesti"
>
>>Committaa indeksissä sijaitsevat tiedostot.

> #### git status
>
>>Palauttaa tiedon nykyisen 'työalueen' tilasta.

> #### git push
>
>>Heittää commitoidut tiedostot remote repositorioon.

> #### git remote add origin
>
>> Yhdistää repositorion palvelimelle.

> #### git branch
>
>Palauttaa tiedon *brancheista*.

### Perumiset:

> #### git checkout [hash]
>
>> Siirryt 'työalueessa' sinne missä se oli kyseisen *hashin* aikana.

> #### git revert [hash]
>
>>Kumoaa tietyn committauksen.

> #### git reset
>
>> Resettaa 'työalueen' annettuun aikaan.

## GitHubin käyttäminen

### Paikallisen Git työhakemiston yhdistäminen GitHubiin

1. Tee [GitHubissa](https://github.com/) repositorio.
2. Avaa Git Bash -ohjelma
3. Navigoi itsesi projektisi hakemistoon
4. Kopioi juuri tekemäsi GitHub repositorion .git URL.
  
 ![Esimerkki, kuva](/Sieppaa.PNG)
 
 5. Syötä komentokehotteeseen

> git remote add origin <.git URL>

Lisää annetun GitHub repositorion paikallisen työhakemiston *remote repositorioksi*.

### Tietojen lähetys paikallisesta hakemistosta GitHubiin

> git push origin main

Lähettää paikallisen työhakemiston annettuun GitHub repositorioon.

### Tietojen saanti GitHubista paikalliseen hakemistoon {#ohjeet-id}

>git pull

Päivittää tiedot ajan tasalle, joten paikallinen hakemisto on samassa vauhdissa GitHub repositorion kanssa.

---

## Forkkaus

Forkin voit tehdä simppelisti painamalla halutussa GitHub repositoriossa *Fork* nappia.

![Fork, nappi](/Fork.PNG)

Tämän forkin voit vapaasti *pullata* paikalliseen hakemistoon normaalisti
> git pull

komennolla

## Upstream

Upstream branchin voi helposti tehdä lisäämällä

  --set-upstream
  
  kun teet *git pushin*. Lopputulos siis näyttää seuraavalta:

> git push --set-upstream origin (branch)
