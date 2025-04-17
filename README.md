# Projetos: excel  

# Projeto 1: Utilizando variação percentual para cálculo de beta, CAPM, desvio padrão e coeficiente de variação.

Nesse projeto realizado na faculdade, são consideradas as variações percentuais de 11 ações durante 470 dias. Cada questão na planilha representa uma etapa:  

- ### Questão 1:  

    É realizado o cálculo do retorno médio e risco de cada ação. Para isso, foi calculado a média aritmética das variações diárias, o desvio padrão e a partir dessas duas informações, é obtido o coeficiente de variação.  

- ### Questão 3:  
    Nessa questão é utilizado o beta para definir o risco das ações.
    Para fins acadêmicos, não foi utilizada a função que calcula o beta de "maneira imediata".  
  
    São calculados covariância (entre o retorno da ação e do mercado) e a variância do retorno do mercado. Dividindo a covariância pela variância, é obtido o beta do ativo.
  

$$\beta_{\text{i}} = \frac{Covariância(retorno_{i}  , retorno_{m})}{Variância(retorno_{m})}$$  

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
     

- ### Questão 5:

    Nessa questão, é feito um rebalanceamento da carteira a fim de reduzir o risco estimado pelo beta. Para isso, utiliza-se o "solver" afim de que a proporção dos ativos da carteira seja ajustada satifazendo as seguintes exigências:  
    1. O beta da carteira deve reduzir para 0,95
    2. Nenhuma ação deve ter participação menor que 2%
     
