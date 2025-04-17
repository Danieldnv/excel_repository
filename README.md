# Projetos: excel  

# Projeto 1: Utilizando variação percentual para cálculo de beta, CAPM, desvio padrão e coeficiente de variação.

Nesse projeto realizado na faculdade, é utilizada uma base de dados contendo as variações percentuais de 11 ações durante 470 dias. São utilizadas diferentes funções do excel e ferramentas como "solver" para atingir o objetivo de cada questão.  

- ### Questão 1:  

    É realizado o cálculo do retorno médio e risco de cada ação. Para isso, foi calculado a média aritmética das variações diárias, o desvio padrão (=DESVPAD.A) e a partir dessas duas informações, é obtido o coeficiente de variação.
  <p align="center">
  <img src="imagens/questão 1.png" width="70%"> 
</p>    

- ### Questão 3:  
    Nessa questão é utilizado o beta para definir o risco das ações.
    Para fins acadêmicos, não foi utilizada a função do excel que calcula o beta de "maneira imediata", mas sim o método matemático tradicional.  
  
    São calculados covariância (entre o retorno da ação e do mercado) (=COVARIAÇÃO.S(matriz1;matriz2)) e a variância (=VAR.A) do retorno do mercado. Dividindo a covariância pela variância, é obtido o beta do ativo.
  

$$\beta_{\text{i}} = \frac{Covariância(retorno_{i}  , retorno_{m})}{Variância(retorno_{m})}$$  
<p align="center">
  <img src="imagens/questão 3.png" width="70%"> 
</p>   

- ### Questão 4:  
    É utilizado o CAPM (Capital Asset Pricing Model) para calcular a taxa de retorno esperada do portfólio de ações. 
    Na planilha, foi considerada uma taxa selic de 14,25% e expectativa de retorno do mercado de 18%.  
    Para obter o resultado do CAPM:
    
     1. É calculado o beta da carteira, multiplicando o beta de cada ativo por sua proporção no portfolio e somando os produtos. 
     2. Em seguida, as informações são aplicadas na fórmula do CAPM: É somada à taxa SELIC o beta da carteira multiplicado pela diferença entre o retorno esperado do mercado e a taxa SELIC. Resultado: 18,19%  

$$ER_i = R_f + \beta_i(ER_m - R_f)$$  
     $ER_i =$ retorno esperado do investimento  
     $R_f =$ taxa livre de risco (nesse caso, a SELIC)  
     $\beta_i =$ beta do investimento (carteira)  
     $ER_m =$ retorno esperado do mercado  
     
 <p align="center">
  <img src="imagens/questão 4.png" width="70%"> 
</p>   
     

- ### Questão 5:

    Nessa questão, é feito um rebalanceamento da carteira a fim de reduzir o risco estimado pelo beta. Para isso, utiliza-se o "solver" afim de que a proporção dos ativos da carteira seja ajustada satifazendo as seguintes exigências:  
    1. O beta da carteira deve reduzir para 0,95
    2. Nenhuma ação deve ter participação menor que 2%
   <p align="center">
  <img src="imagens/questão 5.png" width="70%"> 
</p>   
     
     
