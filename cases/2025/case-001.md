# Caso 2025-001

✶⋆.˚ 〇△□ ˙⋆✶
🚀 E aí, dev! Bora brincar de code review?

Dá uma olhada nessa classe em C#, criada em um projeto com .NET 9.0, no melhor estilo vibe coding, utilizando o modelo Claude 3.7 Sonnet.

🔍 O desafio é simples: que melhorias você faria nesse código?

Em tempos de agentes que geram código com um clique, o olhar crítico e a análise cuidadosa se tornam ainda mais essenciais.

Mesmo com a ajuda de IA, quem dita a qualidade é você. Por isso, mais do que saber usar agentes, é fundamental saber o que e por que pedir.

Vamos nessa? Deixa seu comentário! 👇

```c#
using System;

namespace FinanciamentoSAC.Models
{
    public class DadosFinanciamento
    {
        public double ValorTotal { get; set; }
        public double TaxaJurosAnual { get; set; }
        public int PrazoMeses { get; set; }

        public double TaxaJurosMensal => TaxaJurosAnual / 12 / 100;

        public override string ToString()
        {
            return $"Valor Total: {ValorTotal:C}\n" +
                   $"Taxa de Juros Anual: {TaxaJurosAnual}%\n" +
                   $"Prazo: {PrazoMeses} meses\n" +
                   $"Taxa de Juros Mensal: {TaxaJurosMensal:P2}";
        }
    }
}
```