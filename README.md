# Diagrama UML do iPhone

```mermaid

classDiagram
    Iphone <|.. ReprodutorMusical
    Iphone <|.. AparelhoTelefonico
    Iphone <|.. NavegadorNaInternet

class Iphone{
    + String cor
    + String modelo 
    + int bateria
    + int armazenamento
    +ligar()
    +desligar()
}
   
class AparelhoTelefonico{
    +realizarLigacao(String numero)
    +atender()
    +iniciarCorreioDeVoz()
    +encerrarLigacao
}
class ReprodutorMusical{
    +tocar()
    +pausar()
    + selecionarMusica(String musica)
}

class NavegadorNaInternet{
    +exibirPaginaURL(String URL)
    +adicionarNovaAba()
    +atualizarPagina()
    +fecharPagina()
}

