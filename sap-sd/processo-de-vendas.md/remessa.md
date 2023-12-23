# Remessa

OBS: A criação da remessa pode estar sujeita à *Verificação de disponibilidade (ATP)*

## Transações 

- **VL01N:** Criar remessa
- **VL02N:** Modifica remessa
- **VL03N:** Visualiza a remessa

OBS: É mandatório o local de expedição e a ordem de venda para criação da remessa 


## Tabelas

- **LIKP:** Cabeçalho de remessa
- **LIPS:** Itens de remessa


## Criando remessa dentro da Ordem de Venda

1. Acessa a transação **VA02**;
2. Pesquisa sua ordem de venda;
3. Depois segue o caminho do print abaixo.   

![criando remessa](image-6.png)   

##  Criando tipo de remessa

1. Acesse a transação **SPRO**;
2. Siga o caminho abaixo:

    - *Logistics execution* **>** *Expedição* **>** *Fornecimentos* **>** *Definir tipos de remessa*;

3. Procura o tipo de remessa standard, que é o *LF* e CÓPIA;
5. Preenche os campos mandatórios e salva na request.

OBS: Na imagem abaixo, em vermelho, está marcado o tipo de categoria de documento de SD, se atentar a essa categoria, pois se for entrega ou devolução ela deve mudar de acordo com a finalidade da remessa.   

![categoria de doc remessa](image-7.png)


## Para fazer a liberação da mercadoria

1. Acessa a transação **VL02N**;
2. Pesquisa sua remessa e clica em **Registrar SM**

**Obs:** Toda Saída de mercadoria gera um documento de material, que é o documento de movimentação de estoque 
- Visualiza na **MB51**, mostra todas as movimentações

## Tabelas de material

- **MKPF:** Cabeçalho de documento de material
- **MSEG:** Item de documento de material e ver também o movimento que foi realizado


## Categoria de divisão de remessa

1. Acesse a transação **SPRO**;
2. Siga o caminho abaixo:

    - *Venda e distribuição* **>** *Venda* **>** *Documentos de vendas* **>** *Divisões de remessa*;

3. Clica em *Definir ctgs.divisão*;
4. Procura a divisão standard, que é a *CP* e CÓPIA;
5. Preenche os campos mandatórios e salva na request.


## Atribuir  categorias de divisão de remessa

1. Acesse a transação **SPRO**;
2. Siga o caminho abaixo:

    - *Venda e distribuição* **>** *Venda* **>** *Documentos de vendas* **>** *Divisões de remessa*;

3. Clica em *Atribuir categorias de divisões de remessa*;
4. Procura sua categoria de item e associa a sua categoria de divisão de remessa;
5. Salva na request.

