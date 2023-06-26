## Readme - Gerador de Recibos de Pagamento
Este código é um exemplo de um gerador de recibos de pagamento utilizando a biblioteca pandas para ler os dados dos funcionários a partir de um arquivo CSV e a biblioteca fpdf para gerar os recibos em formato PDF.

## Pré-requisitos
1. Antes de executar o código, certifique-se de ter instalado as seguintes bibliotecas:

- pandas
- fpdf

2. Você pode instalar as bibliotecas utilizando o seguinte comando:
   ```bash
   pip install -r requirements.txt
   ```

3. Antes de executar o código, é necessário preparar o ambiente seguindo os passos abaixo:

4. Certifique-se de ter um arquivo CSV chamado "base_dados_funcionarios.csv" contendo os dados dos funcionários. O arquivo deve ter as colunas "nome", "cpf" e "salario" com as respectivas informações.

5. Defina o nome da empresa e o CNPJ da empresa nas variáveis nome_empresa e cnpj_empresa, respectivamente.

# Executando o código
- Após a configuração adequada, você pode executar o código para gerar os recibos de pagamento dos funcionários. O código realiza as seguintes etapas:

- Lê os dados dos funcionários a partir do arquivo CSV usando a biblioteca pandas.

- Itera sobre cada funcionário e cria um recibo de pagamento em formato PDF utilizando a biblioteca fpdf.

- Salva cada recibo de pagamento em um arquivo PDF na pasta "recibos" com o nome no formato "recibo_nome_funcionario.pdf".

- Certifique-se de que a pasta "recibos" exista antes de executar o código, caso contrário, os recibos não serão salvos corretamente.

# Observações
- O código utiliza a data atual para preencher a data do recibo.

- O recibo é gerado em formato PDF com o texto do recibo e a assinatura do funcionário.

- Os recibos são salvos individualmente para cada funcionário na pasta "recibos".

- Certifique-se de fornecer as informações corretas no arquivo CSV para evitar erros na geração dos recibos.

- Caso deseje personalizar o formato do recibo, você pode ajustar o código conforme suas necessidades, como o tamanho da fonte, o layout do recibo, entre outros.

- Lembre-se de respeitar as leis trabalhistas e tributárias aplicáveis ao emitir recibos de pagamento.

# Limitações
Este código é um exemplo básico e pode ser aprimorado para atender a requisitos específicos ou adicionar recursos adicionais, como cabeçalhos personalizados, rodapés, logotipos da empresa, entre outros.

O código não realiza validações detalhadas nos dados fornecidos no arquivo CSV. Certifique-se de fornecer dados corretos e formatados adequadamente para evitar erros.

A geração dos recibos é feita de forma sequencial, o que pode levar tempo se houver muitos funcionários na base de dados. Para melhorar o desempenho, você pode explorar opções como processamento paralelo ou assíncrono.

# Contribuição
Contribuições, melhorias e sugestões são bem-vindas! Sinta-se à vontade para abrir problemas (issues) e enviar pull requests para aprimorar este código.