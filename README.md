🚗 Projeto Carro – Cadastro simples em Java

Um projetinho bem direto onde aprendo a criar objetos, trabalhar com atributos e interagir com o usuário pelo console usando Java.

🚀 O que faz?

Este projeto cadastra um carro a partir de informações digitadas pelo usuário (marca, modelo e ano).
Depois, ele exibe os dados organizados na tela.
É um exercício simples para praticar POO, entradas via Scanner e criação de métodos.

🔧 Como funciona

Tecnicamente, o projeto funciona assim:

A classe Carro representa um objeto real, com atributos privados: marca, modelo e ano.

Essa classe tem getters e setters e um método que monta uma string com os dados do carro.

No Main, o programa usa Scanner para pedir as informações ao usuário.

Quando o usuário digita tudo, o programa cria uma instância de Carro e imprime as informações usando o método da classe.

📌 Exemplo de código
Classe Carro
public class Carro {
    private String marca;
    private String modelo;
    private String ano;

    public String getMarca() {
        return marca;
    }

    public void setMarca(String marca) {
        this.marca = marca;
    }

    public String getModelo() {
        return modelo;
    }

    public void setModelo(String modelo) {
        this.modelo = modelo;
    }

    public String getAno() {
        return ano;
    }

    public void setAno(String ano) {
        this.ano = ano;
    }

    public String getDadosCarro(){
        return "Marca: " + marca + "\n" + 
               "Modelo: " + modelo + "\n" + 
               "Ano: " + ano;
    }
}

Main
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner carro1 = new Scanner(System.in);

        Carro total = new Carro();

        System.out.println("Digite a marca: ");
        total.setMarca(carro1.nextLine());

        System.out.println("Digite o modelo: ");
        total.setModelo(carro1.nextLine());

        System.out.println("Digite o ano:");
        total.setAno(carro1.nextLine());

        System.out.println("Seu Carro");
        System.out.println(total.getDadosCarro());
    }
}

🛠️ Funcionalidades

Criação de objetos da classe Carro

Entrada de dados via teclado

Impressão formatada das informações

Uso de getters e setters

Estrutura simples de POO

🖥️ Tecnologias

Java 17+

Scanner para input

POO (Programação Orientada a Objetos)

📚 Como usar

Baixe ou clone o repositório

Abra o projeto em sua IDE (IntelliJ, VSCode, Eclipse etc.)

Compile as classes

Rode o arquivo Main.java

Digite os dados solicitados no console

Veja as informações do seu carro impressas na tela

🎓 O que aprendi

Como criar uma classe com atributos privados

Como usar getters e setters

Como construir um método para organizar dados (getDadosCarro)

Como interagir com o usuário usando Scanner

Como instanciar objetos e acessar métodos

Prática inicial de modularização e organização de código

👤 Autor

Weid

⭐ Gostou?

Se esse projetinho te ajudou, deixe uma estrela no repositório!
