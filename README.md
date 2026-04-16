# menu-com-operacoes-matematicas

Realizei esse código com o objetivo de exercitar o uso de `if`'s dentro do `switch case`. 
O usuário deve escolhar qual operação matemática o código deve realizar, e a partir da escolha, o `switch case` vai definir qual `if` irá realizar a operação desejada.

## Tecnologias usadas:

**Operadores de decisão:**

- `if`
- `Scanner`
- `Switch case`
- `default`

**Operadores para comparar e definir ranges:**

- `==`
- `||`
- `>`
- `<`

## Código

    Scanner leitor = new Scanner(System.in);
     int soma = 1;
     int sub = 2;
     int mult = 3;
     int div = 4;
     
    int operacao = 0;
        System.out.println("Escolha qual operacao deseja realizar");
       
        System.out.println("Digite (1) para soma");
         System.out.println("Digite (2) para subtração");
          System.out.println("Digite (3) para multiplicação");
           System.out.println("Digite (4) para divisão");
       
        System.out.println("Digite o numero da escolha: ");
         int escolha = leitor.nextInt();
           if(escolha > 4 || escolha < 1){
             System.out.println("Escolha invalida. Tente novamente");
              
          }
          
    
    switch(escolha) {
        case 1:
         if(escolha == 1){
            System.out.println("Digite o valor a ser somado: ");
              operacao = leitor.nextInt();
                System.out.println("Digite o segundo valor a ser somado: ");
                  operacao = operacao + leitor.nextInt();
                    System.out.println("Resultado: " + operacao);
               
        }
        case 2:
         if(escolha == 2){
           System.out.println("Digite o valor a ser subtraido: ");
             operacao = leitor.nextInt();
               System.out.println("Digite o segundo valor a ser subtraido: ");
                 operacao = operacao - leitor.nextInt();
                   System.out.println("Resultado: " + operacao);
               
        }
        case 3:
         if(escolha == 3){
           System.out.println("Digite o valor a ser multiplicado: ");
             operacao = leitor.nextInt();
               System.out.println("Digite o valor de quantas vezes o numero deve ser multiplicado: ");
                 operacao = operacao * leitor.nextInt();
                   System.out.println("Resultado: " + operacao);
               
        }
         case 4:
          if(escolha == 4){
           System.out.println("Digite o valor a ser dividido: ");
             operacao = leitor.nextInt();
               System.out.println("Digite o valor de quantas vezes o numero deve ser dividido: ");
                 operacao = operacao / leitor.nextInt();
                   System.out.println("Resultado: " + operacao);
               
        }
         default:
             System.out.println("");
            
        
    }
