1)package exercicios;

public class Exercicio {
    public static void main(String[] args)      
      Produto p1 = new Produto("bolacha",2.54);
      Produto p2 = new Produto("cerveja");
      Produto p3 = new Produto();
           p1.Exibir();    
     p1.setNome();
     p1.setPreco(2.53);
     p1.Exibir();
                                 
    }
    
}







package exercicios;

public class Produto {
 
private String Nome;
private double Preco;


public Produto(){
    
}

public Produto(String Nome){
     this.Nome = Nome;
             
  }
public Produto(String Nome,double preco){
this.Nome = Nome;
this.Preco = preco;

}


 public void Exibir(){
    System.out.println("Nome:" + Nome);
    System.out.println("Preço:" + Preco);
}
 public String getNome(){
  return this.Nome;
  
  }
 
 public void setNome(){
   this.Nome = Nome;
 }
 
  public double getPreco(){
  return this.Preco;
  
 }
public void setPreco(double Preco){
     this.Preco = Preco;
  
 }
}


2)package exercicio;

public class Produto {
 
private String Nome;
private double Preco;


public Produto(){
    
}

public Produto(String Nome){
     this.Nome = Nome;
             
  }
public Produto(String Nome,double preco){
this.Nome = Nome;
this.Preco = preco;

}


 public void Exibir(){
    System.out.println("Nome:" + Nome);
    System.out.println("Preço:" + Preco);
}
 public String getNome(){
  return this.Nome;
  
  }
 
 public void setNome(){
   this.Nome = Nome;
 }
 
  public double getPreco(){
  return this.Preco;
  
 }
public void setPreco(double Preco){
     this.Preco = Preco;
     
     if (Preco < 0){
         System.out.println("erro! o valor é menor do que o permitido.");
     } else {
    }

  
 }

}
package exercicios;

public class Exercicios {

    public static void main(String[] args) {
        
      Produto p1 = new Produto("bolacha",2.54);
      Produto p2 = new Produto("cerveja");
      Produto p3 = new Produto();
      
     p1.Exibir();
     
     p1.setNome();
     p1.setPreco(-2.53);
     p1.Exibir();
            
                
      
    }
    
}


3)package exercicios;

public class Exercicio{

    public static void main(String[] args) {

    // Public attribute for the account holder
    public String titular;

    // Private attribute for account balance
    private double saldo;

    // Constructor to initialize the account holder and balance
    public Exercicios(String titular, double saldoInicial) {
        this.titular = titular;
        this.saldo = saldoInicial;
    }

    // Method to deposit money into the account
    public void depositar(double valor) {
        if (valor > 0) {
            saldo += valor;
            System.out.println("Depósito de R$" + valor + " realizado com sucesso.");
        } else {
            System.out.println("Valor de depósito inválido.");
        }
    }

    // Method to withdraw money from the account, ensuring sufficient balance
    public void sacar(double valor) {
        if (valor <= saldo) {
            saldo -= valor;
            System.out.println("Saque de R$" + valor + " realizado com sucesso.");
        } else {
            System.out.println("Saldo insuficiente para o saque de R$" + valor);
        }
    }

    // Method to get the current balance
    public double getSaldo() {
        return saldo;
    }
}

package exercicios;

public class Produto {

    private String Nome;
    private double Preco;

    // Default constructor
    public Produto() {
    }

    // Constructor with name only
    public Produto(String Nome) {
        this.Nome = Nome;
    }

    // Constructor with name and price
    public Produto(String Nome, double preco) {
        this.Nome = Nome;
        this.Preco = preco;
    }

    // Method to display product details
    public void Exibir() {
        System.out.println("Nome: " + Nome);
        System.out.println("Preço: " + Preco);
    }

    // Getters and Setters
    public String getNome() {
        return this.Nome;
    }

    public void setNome(String Nome) {  // Fixed: added parameter to set Nome
        this.Nome = Nome;
    }

    public double getPreco() {
        return this.Preco;
    }

    public void setPreco(double Preco) {
        if (Preco < 0) {
            System.out.println("Erro! O valor é menor do que o permitido.");
        } else {
            this.Preco = Preco;  // Set price if valid
        }
    }
}


4)  // Construtor  (Veiculo)
    public Carro(int velocidadeMaxima) {
        super(velocidadeMaxima); // Inicializa o atributo velocidadeMaxima da classe Veiculo
    }


    public void exibirVelocidadeMaxima() {
        System.out.println("A velocidade máxima do carro é: " + velocidadeMaxima + " km/h");
    }
}
  // Atributo protegido (protected) que pode ser acessado nas classes filhas
    protected int velocidadeMaxima;

    // Construtor
    public Veiculo(int velocidadeMaxima) {
        this.velocidadeMaxima = velocidadeMaxima;
   
    }


5)
    classe Funcionario
        Funcionario f1 = new Funcionario("João", 2500.50);
        Funcionario f2 = new Funcionario("Maria");

        // Exibindo os dados
        f1.exibir();
        f2.setSalario(3000.75);
        f2.exibir();

        // Alterando os dados de f1
        f1.setNome("Carlos");
        f1.setSalario(2700.25);
        f1.exibir();
    }
}

       // Atributos privados
    private String nome;
    private double salario;

    // Construtores
    public funcionario() {
    }

    public funcionario(String nome) {
        this.nome = nome;
    }

    public funcionario(String nome, double salario) {
        this.nome = nome;
        this.salario = salario;
    }

    // Métodos públicos para obter e definir os valores dos atributos
    public String getNome() {
        return this.nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public double getSalario() {
        return this.salario;
    }

    public void setSalario(double salario) {
        this.salario = salario;
    }

    // Método para exibir os dados do funcionário
    public void exibir() {
        System.out.println("Nome: " + nome);
        System.out.println("Salário: " + salario);
    }
}


6)
   // Criando um usuário com login "admin" e senha "1234"
        Usuario usuario = new Usuario("admin", "1234");

        // Testando a autenticação
        if (usuario.autenticar("admin", "1234")) {
            System.out.println("Autenticação bem-sucedida!");
        } else {
            System.out.println("Autenticação falhou!");
        }

        // Testando a autenticação com dados incorretos
        if (usuario.autenticar("admin", "senhaErrada")) {
            System.out.println("Autenticação bem-sucedida!");
        } else {
            System.out.println("Autenticação falhou!");
        }
    }
}

public class Usuario {

    // Atributos privados
    private String login;
    private String senha;

    // Construtor
    public Usuario(String login, String senha) {
        this.login = login;
        this.senha = senha;
    }

    // Método para autenticar o usuário
    public boolean autenticar(String login, String senha) {
        // Verifica se o login e a senha fornecidos correspondem aos armazenados
        return this.login.equals(login) && this.senha.equals(senha);
    }
}


7)package atividedes ;

// Classe Pessoa
public class Pessoa {
    // Atributo protegido
    protected int idade;

    // Construtor
    public Pessoa(int idade) {
        this.idade = idade;
    }
}

// Classe Aluno que herda de Pessoa
public class Aluno extends Pessoa {
    
    private String login;
    private String senha;

    // Construtor
    public Aluno(int idade, String login, String senha) {
        super(idade);  // Chama o construtor da classe Pessoa
        this.login = login;
        this.senha = senha;
    }

    // Método para autenticar o usuário
    public boolean autenticar(String login, String senha) {
        // Verifica se o login e a senha fornecidos correspondem aos armazenados
        return this.login.equals(login) && this.senha.equals(senha);
    }

    // Método para definir a idade do aluno
    public void setIdade(int idade) {
        this.idade = idade;
    }

    // Método para exibir a idade do aluno
    public void exibirIdade() {
        System.out.println("Idade do aluno: " + this.idade + " anos");
    }

    // Testando a autenticação e exibição da idade
    public static void main(String[] args) {
        // Criando um aluno com login "admin", senha "1234" e idade 20
        Aluno aluno = new Aluno(20, "admin", "1234");

        // Testando a autenticação
        if (aluno.autenticar("admin", "1234")) {
            System.out.println("Autenticação bem-sucedida!");
            aluno.exibirIdade();  // Exibe a idade do aluno após autenticação
        } else {
            System.out.println("Autenticação falhou!");
        }
    }
package atividedes7;

public class Atividedes7 {

    public static void main(String[] args) {
 
            // Testando a autenticação
        if (aluno.autenticar("admin", "1234")) {
            System.out.println("Autenticação bem-sucedida!");
            aluno.exibirIdade();  // Exibe a idade do aluno após autenticação
        } else {
            System.out.println("Autenticação falhou!");
        }

        // Testando a autenticação com dados incorretos
        if (aluno.autenticar("admin", "senhaErrada")) {
            System.out.println("Autenticação bem-sucedida!");
        } else {
            System.out.println("Autenticação falhou!");
        }
    }
}


package exercicios8;
public class Exercicio1 {
   public static void main(String[] args) { // Adicionado '{' na assinatura do main
       Produto p1 = new Produto("bolacha", 2.54);
       Produto p2 = new Produto("cerveja");
       Produto p3 = new Produto();
      
       p1.exibir();   
       p1.setNome("biscoito"); // Agora recebe um argumento
       p1.setPreco(2.53);
       p1.exibir();
      
       // Testando a classe Porta
       Porta porta = new Porta();
       porta.abrir();
       porta.fechar();
   }
}
package exercicio8;
public class Produto {
   private String nome; // Variáveis agora seguem a convenção de nomenclatura
   private double preco;
   public Produto() {
   }
   public Produto(String nome) {
       this.nome = nome;
   }
   public Produto(String nome, double preco) { // Corrigido para manter o padrão de nomes
       this.nome = nome;
       this.preco = preco;
   }
   public void exibir() { // Método renomeado para seguir convenção Java
       System.out.println("Nome: " + nome);
       System.out.println("Preço: " + preco);
   }
   public String getNome() {
       return this.nome;
   }
   public void setNome(String nome) { // Agora recebe um parâmetro
       this.nome = nome;
   }
   public double getPreco() {
       return this.preco;
   }
   public void setPreco(double preco) { // Parâmetro com nome correto
       this.preco = preco;
   }
}
package exercicios;
public class Porta {
   private boolean aberta; // Variável privada, não pode ser acessada diretamente
   public Porta() {
       this.aberta = false; // A porta começa fechada
   }
   public void abrir() {
       if (!aberta) {
           aberta = true;
           System.out.println("A porta foi aberta.");
       } else {
           System.out.println("A porta já está aberta.");
       }
   }
   public void fechar() {
       if (aberta) {
           aberta = false;
           System.out.println("A porta foi fechada.");
       } else {
           System.out.println("A porta já está fechada.");
       }
   }
   public boolean isAberta() { // Método para consultar o estado da porta
       return aberta;
   }
}


9)package exercicios;
// Classe Base
class Animal {
   protected void fazerSom() {
       System.out.println("O animal faz um som.");
   }
}
// Classe Cachorro herdando de Animal
class Cachorro extends Animal {
   @Override
   protected void fazerSom() {
       System.out.println("O cachorro late: Au Au!");
   }
}
// Classe Gato herdando de Animal
class Gato extends Animal {
   @Override
   protected void fazerSom() {
       System.out.println("O gato mia: Miau!");
   }
}
// Classe Principal (Main)
public class Exercicio9 {
   public static void main(String[] args) {
       Animal meuCachorro = new Cachorro();
       Animal meuGato = new Gato();
      
       meuCachorro.fazerSom(); // Saída: O cachorro late: Au Au!
       meuGato.fazerSom();      // Saída: O gato mia: Miau!
   }
}


10)
package exercicio10;
public class Carro {
   private String marca;
   private String modelo;
   public int ano; // Mantido público conforme solicitado
   // Construtor
   public Carro(String marca, String modelo, int ano) {
       this.marca = marca;
       this.modelo = modelo;
       setAno(ano); 
   }
   // Getter para marca
   public String getMarca() {
       return marca;
   }
   // Setter para marca
   public void setMarca(String marca) {
       this.marca = marca;
   }
   // Getter para modelo
   public String getModelo() {
       return modelo;
   }
   // Setter para modelo
   public void setModelo(String modelo) {
       this.modelo = modelo;
   }
   // Setter para ano
   public void setAno(int ano) {
       if (ano >= 1886) {
           this.ano = ano;
       } else {
           System.out.println("Erro: O ano do carro não pode ser menor que 1886!");
       }
   }
   // Método para exibir informações do carro
   public void exibirInfo() {
       System.out.println("Marca: " + marca);
       System.out.println("Modelo: " + modelo);
       System.out.println("Ano: " + ano);
   }
}
package exercicios;
public class Exercicio10 {
   public static void main(String[] args) {
       Carro carro1 = new Carro("Toyota", "Corolla", 2020);
       carro1.exibirInfo();
       System.out.println("\nTentando definir um ano inválido...");
       carro1.setAno(1800); // Deve exibir uma mensagem de erro
      
       System.out.println("\nAlterando os dados...");
       carro1.setMarca("Honda");
       carro1.setModelo("Civic");
       carro1.setAno(2022);
       carro1.exibirInfo();
   }
}
