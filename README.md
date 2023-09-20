# operacaocachimbo
Repositório documentando a base e etapas de análise da base de pessoas detidas durante a operação cachimbo realizada na cracolândia em São Paulo em 2022 como parte da disciplina "Fundamentos e ética do jornalismo de dados" do curso Jornalismo de dados no Insper. 

A base de dados foi liberada através de um pedido de LAI para a Defensoria Pública do Estado de São Paulo, tendo como refferência o material "Operação Cachimbo - relatório das detenções em massa realizadas na cracolândia". Com base na base bruta foi elaborado o seguinte roteiro de análise:

1# Qual a faixa etária das pessoas presas na Cracolândia? Média de 36 anos. Para chegar neste resultado, somamos as 641 linhas da coluna idade (=somaA2:A641), onde obtivemos a soma 23235. Dividimos isso pela 641 linhas para obter a média, que é de 36,2. 

2# Qual o grau de ensino dos detidos? No registro de 641 pessoas presas, não há informação sobre a escolaridade. Depois, o que mais aparece é o Fundamental Incompleto, com 129 registros. Outros registros são:  Sabe ler e escrever (38 registros), Fundamental Completo (6 registros), Médio Completo (2 registros) e Analfabeto (1 registro). Para chegar a este resultado, aplicamos filtros na planilha excel na coluna “Grau de instrução”. 
 
3# Há um encaminhamento de saúde para as pessoas presas na Cracolândia? Sim, 495 foram encaminhadas a unidades do CAPSe também ao UPA Vergueiro. Constam 10 registros de encaminhamentos para o CAPS de forma genérica. Outros 244 foram encaminhados para o CAPS IV, duas pessoas para o CAPS V, 239 pessoas para a UPA Vergueiro. Em 109 casos, não há informação sobre o encaminhamento do detido para uma unidade de saúde. Uma pessoa não teve interesse em ir à uma unidade de saúde. Em 36 casos houve orientação genérica para buscar serviços de saúde. Para chegar a este resultado, aplicamos filtros na planilha excel na coluna “Houve algum encaminhamento de saúde da pessoa detida?”. 

4# Quem são as testemunhas que constam nas prisões? A Polícia Civil (442 registros), Polícia Militar (66 registros) e Guarda Civil Metropolitana (69 registros). Em 64 casos, não há informação sobre testemunha. Para chegarmos neste resultados,  aplicamos filtros na planilha excel na coluna “Testemunha 1”. 

5# Houve prisão todos os dias? Não. Houve prisão em 48 dias /  Qual dia mais pessoas foram presas? 19/10/2022 (31 presos). Para chegar nesses resultados realizamos uma tabela dinâmica a partir da coluna “Data do fato” e selecionamos a opção “Counta” para mostrar quantas entradas haviam para cada data. A partir disso foi simples identificar que não não haviam ocorrências todos os dias. Em seguida, colocamos para que os resultados estivessem na ordem decrescente, a fim de identificar a data com mais pessoas presas.

6# Qual a substância que as pessoas presas mais tinham? Crack aparece 65 vezes na base, mas com quantidades baixas, de 0,1 g. A droga com maior quantidade apreendida, mesmo que em menor frequência, é a maconha - foram 8,81 gramas apreendidas ao todo. Filtramos a coluna “foram apreendidas drogas?”. Nela, selecionamos as opções “espaços em branco”; “apenas resquícios e sujidades”; “não”; “sim, apenas resquícios e sujidades”. Depois disso, olhamos para a coluna “Se constarem drogas apreendidas (diferente de resquícios e sujidades) incluir observação com a quantidade” para entender a quantidade de droga apreendida com cada pessoa presa. Foram encontrados 76 registros. A partir daí, somamos os resultados abaixo em tabela dinâmica: “se constarem drogas apreendidas” + count. Fizemos uma segunda agregação para somar quantos gramas forma apreendidos por droga. 

7# Qual o principal motivo da prisão? Resquícios e sujidades de droga. Não havia especificamente uma coluna com o motivo da prisão, mas para chegar nesse resultado optamos por fazer tabela dinâmica a partir da coluna “Foram apreendidas drogas?”.

8# Qual era a profissão das pessoas? A maioria não tinha profissão ou não havia sido informado às autoridades. Apenas 8 registros de 641 tinham alguma profissão.  Para obter esse resultado fizemos uma tabela dinâmica a partir da coluna “Profissão” e identificamos as poucas entradas que constavam nesse campo. 

9# As pessoas presas foram soltas depois? Não é possível responder pela base

10# Onde ocorreram as prisões? Rua Helvetia, Alameda Dino Bueno, Alameda Glete, Avenida São João e Rua Amaral Gurgel. Para chegar nesse resultado fizemos uma tabela dinâmica apenas na coluna “Local da ocorrência” para identificar as ruas em comuns; mesmo assim, foi necessário fazer um trabalho manual, já que haviam entradas diferentes para o mesmo endereço. Juntamos manualmente e chegamos nas ruas onde ocorrerão as prisões.

A elaboração do roteiro e criação de pauta foi realizada por: Caê Vatiero, Gabriela Cassoli, Heloísa Vasconcelos, Marcela Villar, Rute Damascena e Valmerson Barbosa. 
