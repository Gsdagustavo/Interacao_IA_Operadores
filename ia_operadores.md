### **1. O que acontece se eu comparar valores de tipos diferentes usando operadores relacionais em Dart?**  
Se você comparar valores de **tipos diferentes** usando operadores relacionais (`<`, `>`, `<=`, `>=`), o Dart lançará um **erro em tempo de execução**, pois esses operadores só podem ser usados entre valores comparáveis do mesmo tipo. Já os operadores de igualdade (`==` e `!=`) podem ser usados entre diferentes tipos, mas geralmente retornam `false`, a menos que haja uma conversão interna ou implementação personalizada de `==`.  

---

### **2. Qual a diferença entre os operadores de divisão `/` e `~/`?**  
- `/` → Realiza uma divisão normal e retorna um **número de ponto flutuante** (`double`).  
- `~/` → Faz uma **divisão inteira**, descartando a parte decimal e retornando um **inteiro** (`int`).  

---

### **3. Como verifico se uma variável é de um determinado tipo em Dart?**  
Para verificar o tipo de uma variável, use o operador `is`. Se precisar garantir que ela **não** é de um determinado tipo, use `is!`.  

---

### **4. Qual a função do operador `?` em testes de tipo?**  
O operador `?` pode ser usado em conjunto com `as` (`as?`) para conversão de tipos de forma segura. Ele evita exceções caso a conversão falhe, retornando `null` em vez de lançar um erro.  

---

### **5. Quando usar os operadores de valores opcionais e valores requeridos em uma função Dart?**  
- **Valores opcionais** → Quando um parâmetro pode ser omitido, tornando a função mais flexível.  
- **Valores requeridos** → Quando um parâmetro é essencial para a função e deve ser sempre fornecido, garantindo segurança no código.  

---

### **6. Quais são os operadores de atribuição compostos e como eles funcionam?**  
Os operadores de atribuição compostos combinam atribuição (`=`) com operações matemáticas. Eles modificam o valor da variável e já atribuem o novo valor. Alguns exemplos:  
- `+=` → Soma e atribui  
- `-=` → Subtrai e atribui  
- `*=` → Multiplica e atribui  
- `/=` → Divide e atribui  
- `~/=` → Divide e atribui o valor inteiro  
- `%=` → Calcula o módulo e atribui  

---

### **7. Como uso os operadores `&&` e `||` para combinar condições?**  
- `&&` (E lógico) → Retorna `true` somente se **ambas** as condições forem verdadeiras.  
- `||` (OU lógico) → Retorna `true` se **pelo menos uma** das condições for verdadeira.  
Esses operadores são usados para construir expressões condicionais mais complexas.  

---

### **8. Qual a diferença entre usar `if-else` e expressões condicionais?**  
- **`if-else`** → Usado para controle de fluxo quando há múltiplas instruções a serem executadas com base na condição.  
- **Expressão condicional (`condition ? value1 : value2`)** → Retorna um valor com base na condição e é útil para expressões mais concisas.  

---

### **9. Em quais situações a notação em cascata pode tornar o código mais legível?**  
A notação em cascata (`..`) melhora a legibilidade quando se precisa chamar múltiplos métodos ou modificar várias propriedades de um objeto em sequência, sem precisar armazenar o objeto repetidamente em uma variável temporária.  

---

### **10. Qual a diferença entre usar a notação em cascata e chamar métodos separadamente?**  
- **Notação em cascata (`..`)** → Permite chamar múltiplos métodos ou definir propriedades sem precisar referenciar a variável várias vezes.  
- **Chamada separada** → Exige atribuir o resultado a uma variável ou chamar métodos individualmente, podendo tornar o código mais verboso.  

---

### **11. Como a notação em cascata pode ser usada para modificar um objeto após realizar testes de tipo?**  
Se um objeto for de um tipo específico (`is`), a notação em cascata permite modificar suas propriedades ou chamar métodos diretamente sem precisar armazenar a conversão em uma variável separada. Isso facilita a manipulação do objeto de maneira fluida após garantir seu tipo.
