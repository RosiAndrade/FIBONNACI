//Rosilaine
function fibonacci(n) {
  // Verificar se o número é menor ou igual a 0
  if (n <= 0) {
    console.log("Por favor, insira um número positivo.");
    return;
  }

  // Variáveis para armazenar os dois primeiros números da sequência
  let fib = [0, 1];

  // Calcular os números subsequentes da sequência
  for (let i = 2; i < n; i++) {
    fib[i] = fib[i - 1] + fib[i - 2];
  }

  // Exibir a sequência até o número de elementos solicitado
  console.log(`Os primeiros ${n} números de Fibonacci são: ${fib.slice(0, n).join(", ")}`);
}

// Exemplo de uso
let quantidadeElementos = prompt("Digite o número de elementos da sequência de Fibonacci que deseja ver:");
quantidadeElementos = parseInt(quantidadeElementos);

fibonacci(quantidadeElementos);

