# 📊 Sistema de Auditoria de Vendas Semanais

## 📝 Descrição do Projeto
Este projeto consiste em um algoritmo de monitoramento e auditoria financeira desenvolvido para automatizar a validação de transações comerciais. O objetivo principal é assegurar a integridade dos dados e identificar anomalias operacionais, como vendas que fogem do padrão estatístico ou que ultrapassam limites de segurança preestabelecidos.

Desenvolvido por **Kayky**, estudante do primeiro ano de **Engenharia de Software** na **Unicid**, o sistema processa entradas de valores em tempo real, realizando cálculos de média aritmética e aplicando flags de segurança baseadas em regras de negócio dinâmicas.

![Figura 1: Representação da lógica de auditoria e controle de limites](http://googleusercontent.com/image_generation_content/0)
*Figura 1: Fluxo de decisão do sistema, incluindo estados de Quarentena e Revisão Manual.*

## 🚀 Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Conceitos:** Manipulação de variáveis globais, casting de tipos primitivos e lógica condicional avançada
* **Ferramentas:** Google Colab

## 📊 Regras de Negócio e Aprendizados
O sistema foi estruturado para atuar em três frentes de proteção financeira:
* **Controle de Segurança Adaptável:** Utiliza o parâmetro `LIMITE_SEGURANCA` (inicialmente R$ 10.000,00), permitindo que o gestor atualize o teto operacional sem interromper a execução do código.
* **Protocolo de Quarentena:** Aciona automaticamente o estado de "SISTEMA EM QUARENTENA" se a média das vendas exceder o limite de segurança definido.
* **Identificação de Discrepâncias:** O sistema sinaliza "REVISÃO MANUAL" caso qualquer venda individual seja 2x maior que a média do período, prevenindo erros de entrada ou fraudes.
* **Precisão de Dados:** Implementação de casting rigoroso para `float` e inspeção de tipos (`type()`) para garantir a confiabilidade dos resultados finais.

## 🔧 Como Executar
1. Clone o repositório para o seu ambiente local.
2. Certifique-se de ter o Python instalado.
3. Execute o comando: 
   ```bash
   python algoritmo_de_auditoria_de_dados.py