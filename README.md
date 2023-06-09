# AulaJava

Dupla: Eloá Vasconcelos de Macedo e Laura Cristine Silva 




# TIPOS DE DADOS EM JAVA 
  
> Tipos primitivos: byte, short, int, long, boolean, char, float, double (Tipos básicos).

- BYTE: Inteiro de 8 bits;
- SHORT: Inteiro de 16 bits;
- INT: Inteiro de 32 bits, número interiro sem decimais;
- LONG: Inteiro 64 bits;
- BOOLEAN: Valor true ou false (Verdadeiro ou Falso);
- CHAR: Caracter em notação Unicode de 16 bits;
- FLOAT: Números em notação de ponto flutuante, 32 bits, números quebrados ou com vírgula;
- DOUBLE: Números em notação de ponto flutuante, 64 bits;


> Tipos de dados por referência: string, array/matriz; (Tipos utilizados para armazenar as localizações dos objetos da memória do computador).
>
> - ARRAY: Responsável por guardar uma variedade de valores, são como vetores; 
Ex: intArray = {2,5,46,12,34}; - guarda múltiplos valores de inteiros;
> - STRING: Caracteres formando um texto/conjunto de palavras, por exemplo "Programar é top". É um tipo mais complexo, possuindo métodos, sendo um deles o length() que nos diz quantos caracteres contêm aquela string;



# ESTRUTURAL CONDICIONAL EM JAVA

> Estrutura que possibilitam ao programa a tomar decisões e alterar seu fluxo de execução.
>
> *Estruturas condicionais permitem criar possibilidades diferentes em um sistema, determinado um comando específico e criando novos caminhos por meio das estruturas condicionais.*
>
> **Existem 2 principais, são elas : If/Else e Switch/Case**

- ## If/Else

> If = se  
> Else = Senao 
>
> Tipo booleano que analisa a questão do verdadeiro ou falso, quando a condição dentro do IF for verdadeira será executada, já o ELSE será utilizado para definir o que irá acontecer se o If for falso. 

**Exemplo utilizando o  IF**

Int idade =23\
   If (idade > 18) {\
 System.out.println("A entrada é permitida");\
}

**ANALISANDO O CÓDIGO**

Analisando o código vemos que o valor da variável idade é igual a 23;
Portanto, se o número que o usuário digital for maior que 18 o sistema irá apresentar a seguinte mensagem (" entrada é permitida"), caso a condição não for atendida nada irá acontecer.

**Exemplo utilizando IF e ELSE** 

Int idade =23 \
   If (idade > 18) { \
    System.out.println("A entrada é permitida");\
}\
  else {\
System.out.println("Entrada negada");\
}

**ANALISANDO O CÓDIGO**

A mesma linha de raciocínio, no entanto se a idade digitado do usuário foi menor que 18,a seguinte mensagem será apresentada ("Entrada Negada")


 - ## Switch/Case

> Switch = Troca
> Case = Caso
>
> Ela vem como alternativa para "susbtituir os IF/ELSE", em grandes quantidades, "opções de escolha". 
>
> Usa-se o Switch/Case para substituir múltiplos if/elses, e de certa forma deixando o código mais organizado 

 **Exemplo utilizando o SWITCH CASE** 

 Int   mes = 3

 Switch (mes) {

 Case 1 :
  System.out.println (" O mês é janeiro);
 Break;

 Case 2 :
 System.out.println (" O mês é fevereiro);
 Break;

 Case 3 :
 System.out.println (" O mês é março);
 Break;

 Case 4 :
 System.out.println (" O mês é abril );
 Break;
       
 default:
  System.out.println(“Mês inválido”);
  break;
 }

 **ANALISANDO O CÓDIGO**

O Switch case irá testar o valor contido na variável, comparando com cada uma das opções, determinadas pelo Case, assim quando o o valor corresponden ao valor da variável o sistema irá executar, caso nenhuma se relaciona, o último blobo (default) irá ser executado.

> ***Obs: Cada Case precisa de uma "terminação", sendo determinada pelo palavra Break***


# ESTRUTURA DE REPETIÇÃO

> Estruturas que permitem repetir uma série de operações. Simplesmente repetir uma operação até que uma condição seja executada, também conhecidas como loops.
>
> - FOR: estrutura na qual seu ciclo será executado por um tempo determinado, em quantidade determinada por nós.
> - WHILE: diferente do FOR, o while é utilizado quando não sabemos de forma firme quantas vezes o código será repetido.


- ## LOOPING FOR

> For = para.

**ESTRUTURA DO FOR**

for (variavel de controle, analise da variavel, incremento) { \
    //código determinado \
}

**Exemplo utilizando o FOR**

 public class ExemploUtilizacao {

	    public static void main(String[] args) {
        for (int i = 0; i <= 10; i++) {
            System.out.println(“A variável i agora vale “ + i);
        }
    }
	
 
**ANALISANDO O CÓDIGO**

O exemplo acima retrata a situação de que "A variável i vale 0, A variável i vale 1, A variável i vale 2, A variável i vale 3..." e assim até parar na variável i valendo 10. Isso acontece porque o i tem como valor inicial 0, e logo depois foi determinado que o "limite" seria 10, quando chega no 10, a repetição para. 

*A parte "i++" significa que no fim de cada execução é incrementado, somado 1.*


- ## LOOPING WHILE
 
 > While = enquanto
 
**ESTRUTURA DO WHILE**
 
 While (<condicao>) {
 //trecho a ser repetido
 }
 
**Exemplo utilizando o WHILE**
 
 import java.util.Scanner;

public class Exemplo {
	
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int numero = -1;
        while (numero != 10) { 
// enquanto a variável não for 10, o trecho de código será repetido
            System.out.println(“Digite um número: “);
            numero = in.nextInt();
            if (numero == 10) {
                System.out.println(“Você acertou!“);
            } else {
                System.out.println(“Você errou :(“);
            }
        }
    }
								   
}

**ANALISANDO O CÓDIGO**

O exemplo representado, é pedido para que o usuário tente advinhar o número. Enquanto não acerta, é pedido ao usuário que digite qual número ele acha que é. Este trecho sempre será repetido, até que o usuário acerte. 


# TIPOS DE ELEMENTOS VISUAIS NO ANDROIDSTUDIO

> Existem diversos tipos de elementos visuais presentes no AndroidStudio, cada um com uma função e características diferentes. Dentre muitos, existem os principais, são eles:

### TIPO TEXT 
> - ### EditText
> É uma extensão do TextView, que permite que o usuário "entre" com seu teclado no campo de texto, assim podendo ser feitas alterações no mesmo.
> - ### TextView
> Utilizado como caixa de texto. Componente extremamente importante, tendo como principal utilizade exibir um texto no Android. Uma tarefa simples, a classe TextView contém uma lógica complexa que permite criarmos textos formatdados, hyperlinks, números de telefone, e-mails e outros.
>
**Exemplo:**

<TextView \
    > android:text="Olá Androideiro!" \
    > android:background="@android:color/darker_gray" \
    > android:layout_width="150dp" \
    > android:layout_height="75dp" />


### TIPO BUTTON 
> - ### Button:
> O Button é um dos controles mais básicos e conhecidos do AndroidStudio, sendo usado como um botão de ação (determinamos o que ele irá realizar), respondendo a cliques do usuário. 
>
**Exemplo:**

<Button \
     android:layout_height="wrap_content" \
     android:layout_width="wrap_content" \
     android:text="Meu Botão" \
     android:onClick="clicar" />


> - ### ImageButton:
> Já o ImageButton é combinação de Button com uma ImageView, aonde ao clicarmos, uma imagem aparecerá na tela.
>
**Exemplo:**

<ImageButton \
    android:id="@+id/imageButton" 
    android:layout_width="wrap_content" \
    android:layout_height="wrap_content" \
    android:src="@drawable/imagem" />

### TIPO WIDGET 
> - ### View
> Widgets são as visualizações de aplicativos em miniatura, visualizações rápidas. Como por exemplo, a exibição da previsão do tempo, aonde vemos ela de forma menor e resumida, porém quando clicamos, a mesma abre o aplicativo e nos fornece informações de forma mais detalhada.
>
> - ### ImageView
> Ele tem como obejtivo exibir imagens na tela. Isso pode ser usado para a exibição de recursos armazenados no aplicativo ou para a exibição de imagens que são baixadas da internet.
>
> - ### ListView
> Usada para exibir uma coleção de itens de forma linear em uma única coluna.
>
*As Android Views são os principais componentes empregados para desenvolver, criar as interfaces dos aplicativos Android. Além de serem responsáveis pela maior parte da interação entre o usuário e o aplicativo, elas têm um grande papel em definir o design, para que ele seja agradável e com uma alta usabilidade.*

### TIPO LAYOUT 
> - ### ConstraintLayout
> O layout define a organização de uma interface do usuário no aplicativo, como acontece na atividade. A ConstraintLayout permite posicionar, trabalhar com Widgets de maneira mais flexível.  
>
> - ### LinearLayout 
> Esse tipo de layout permite organizar outras exibições horizontalmente em uma única coluna ou de forma vertical em uma linha única.
>
> - ### FrameLayout
> Tem a função de bloquear uma área na tela.

### TIPO CONTAINERS 
> - ### Spinner
> Representa uma ComboBox no VS
> O Spinner permite selecionar um valor de um conjunto de dados. É um controle giratório que apresenta um menu suspenso. De inico irá apresentar o primeiro valor determinado, mas ao tocar no controle giratório as demais opções irão aparecer, semdo um menu suspenso.

**Exemplo**: 

<resources> \
    <string-array name="planets_array"> \
        <item>Mercury</item> \
        <item>Venus</item> \
        <item>Earth</item> \
        <item>Mars</item> \
        <item>Jupiter</item> \
        <item>Saturn</item> \
        <item>Uranus</item> \
        <item>Neptune</item> \
    </string-array> \
</resources>

*O nome dado ao menu é "planets" e logo em baixo são os nomes dos planetas(os outros valores), que estarão/serão apresentados no menu suspenso em caso de 'click', esses valores irão aparecer na Spinner.*

### TIPO HELPERS 
> - ### Group
> Essa classe controla a visibilidade de um conjunto de widgets referenciados. Widgets são referenciados por serem adicionados a uma lista separada por vírgulas de ids.

### TIPO GOOGLE 
> - ### Adview (Exibição de Anúncios)
> Banner - Anúncio digital 
> São usados para colocar Banners/Anúncios na parte superior ou inferior da tela do dispositivo.
> Para inserir um banner na tela utiliza-se o Adview 
>
>Criação de frame Layout - Mondura 

**Exemplo:** 

private FrameLayout adContainerView; \
private AdView adView; \

@Override \
protected void onCreate(Bundle savedInstanceState) { \
  super.onCreate(savedInstanceState); \
  setContentView(R.layout.activity_main); \

  //Call the function to initialize AdMob SDK \
  MobileAds.initialize(this, new OnInitializationCompleteListener() { \
     @Override \
     public void onInitializationComplete(InitializationStatus initializationStatus) { \
     } \
  });

  //get the reference to your FrameLayout
  adContainerView = findViewById(R.id.adView_container);

  //Create an AdView and put it into your FrameLayout
  adView = new AdView(this);
  adContainerView.addView(adView);
}

### TIPO LEGACY 
> - ### Gridlayout
> É usado para exibir elementos e visualizações na forma de uma grade retangular, permitindo a definição do número de linhas e colunas para a grade, além de definir como o elementos devem ser orientados. GridLayout pode conter várias exibições. 
> Em outras palavras: Divide a área do container 
> Em cada área um elemento pode ser adicionado 

# REFERÊNCIAS 

AdView  |  Firebase. Firebase. Disponível em: https://firebase.google.com/docs/reference/android/com/google/android/gms/ads/AdView. Acesso em: 4 abr. 2023.

Anúncios em banner. Google Developers. Disponível em: <https://developers.google.com/admob/android/banner?hl=pt-br>. Acesso em: 4 abr. 2023.

ConstraintLayout  |  Android Developers. Android Developers. Disponível em: https://developer.android.com/reference/androidx/constraintlayout/widget/ConstraintLayout. Acesso em: 5 abr. 2023.

CORDEIRO, Fillipe. Saiba como usar as Android Views da forma correta | AndroidPro. AndroidPro. Disponível em: https://www.androidpro.com.br/blog/desenvolvimento-android/android-views-intro/#:~:text=A%20principal%20utilidade%20do%20TextView,mails%20e%20outras%20funcionalidades%20%C3%BAteis. Acesso em: 5 abr. 2023.

Curso de Java - Tipos de Dados. Ufscar.br. Disponível em: https://www.dm.ufscar.br/~waldeck/curso/java/part22.html. Acesso em: 4 abr. 2023.

Estrutura de Decisão Condicional Switch em Java - Bóson Treinamentos em Ciência e Tecnologia. Bóson Treinamentos em Ciência e Tecnologia. Disponível em: http://www.bosontreinamentos.com.br/java/estrutura-de-decisao-condicional-switch-em-java/. Acesso em: 3 abr. 2023.

Estruturas condicionais e estruturas de repetição em Java. Treinaweb.com.br. Disponível em: https://www.treinaweb.com.br/blog/estruturas-condicionais-e-estruturas-de-repeticao-em-java. Acesso em: 23 mar. 2023.
GridLayout. Android Developers. Disponível em: https://developer.android.com/jetpack/androidx/releases/gridlayout?hl=pt-br. Acesso em: 4 abr. 2023.

Group  |  Android Developers. Android Developers. Disponível em: https://developer.android.com/reference/androidx/constraintlayout/widget/Group. Acesso em: 5 abr. 2023.

Integrate Adaptive Banner with Android Studio  |  Google Codelabs. Google Codelabs. Disponível em: https://codelabs.developers.google.com/codelabs/adaptive-banner-android-studio#3. Acesso em: 4 abr. 2023.

LinearLayout  |  Android Developers. Android Developers. Disponível em: https://developer.android.com/reference/android/widget/LinearLayout. Acesso em: 5 abr. 2023.

Recurso de layout. Android Developers. Disponível em: https://developer.android.com/guide/topics/resources/layout-resource?hl=pt-br. Acesso em: 5 abr. 2023.

ROGÉRIO ARAÚJO. Os tipos primitivos da Linguagem Java. Blog Gran Cursos Online | Concursos Públicos Abertos 2023. Disponível em: https://blog.grancursosonline.com.br/os-tipos-primitivos-da-linguagem-java/. Acesso em: 3 abr. 2023.

Spinner no Android com exemplo – Acervo Lima. Acervolima.com. Disponível em: https://acervolima.com/spinner-no-android-com-exemplo/. Acesso em: 4 abr. 2023.

Spinners. Android Developers. Disponível em: https://developer.android.com/develop/ui/views/components/spinner. Acesso em: 4 abr. 2023.

Switch Case Java: usando estruturas de decisão com várias condições! | Insights para te ajudar na carreira em tecnologia | Blog da Trybe. Betrybe.com. Disponível em: https://blog.betrybe.com/java/switch-case-java/. Acesso em: 23 abr. 2023.

VARALLO, Vinícius. Tipos de dados por valor e por referência em Java. DevMedia. Disponível em: https://www.devmedia.com.br/tipos-de-dados-por-valor-e-por-referencia-em-java/25293. Acesso em: 6 abr. 2023.

View  |  Android Developers. Android Developers. Disponível em: https://developer.android.com/reference/android/view/View. Acesso em: 23 mar. 2023.

VINICIUS DOS SANTOS. Estruturas condicionais (if e else), laços de repetição (while e for) em Java. Computer Science Master. Disponível em: https://www.computersciencemaster.com.br/estruturas-condicionais-if-else-lacos-de-repeticao-while-for-em-java/. Acesso em: 17 mar. 2023.

