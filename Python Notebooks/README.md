# Jupyter Notebooks dos Scripts
- pltWrapper:
> (os, numpy, pandas, regex, matplotlib.pyplot)
>
> Considera-se a simulação no Anatem com 20s e 517 pontos no total, sendo as variáveis [DELT, PACEC, PGER, QGER, VOLT, ANGL] plotadas do Anatem
> 
> Classe pltData: busca arquivos .plt (estrutura RAIZ/CASO {A}/CASO {01}/CASO{01}_{ID DA CONTINGÊNCIA}.PLT), estrutura os dados de acordo com o que é lido nos arquivos. A estrutura deve ser a padrão de saída do Anatem (v. 11.6 utilizado)
> 
> Classe Event(pltData): de pltData, é possível criar um novo evento, que irá extrair os dados com os métodos de pltData e identificar na classe de acordo com o que é lido no nome do arquivo. Com o evento construído, é possível plotar e salvar a figura plotada de acordo com o que for definido nos métodos plotEvent() e plotEventSave()
