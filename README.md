[Figura 0 - Logo] 

## DESAFIO DE PROJETO 4: UTILIZANDO AI SEARCH PARA INDEXAÇÃO A CONSULTA DE DADOS

#### Laboratório sobre como criar uma aplicação de consulta a documentos indexados no Azure AI Search pelo portal da Azure

#### Propósito do projeto: Mostrar a importância dos conceitos relacionados as ferramentas apresentadas, tais como: insights, indexação e a importância do armazenamento de conhecimento. 

### Introdução

#### Antes de tudo, é necessário criar e configurar os seguintes recursos [neste portal](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html) com suas devidas configurações:

**Azure AI Search**

#### A Pesquisa Cognitiva do Azure, como também é conhecida, é um serviço de nuvem da Microsoft que fornece recursos poderosos de indexação e consulta para dados não estruturados. É permitida a criação de experiências de pesquisa avançadas e aplicativos de IA generativa que combinam grandes modelos de linguagem com seus dados corporativos.

**Azure AI Services** 

#### O Azure AI Services (já visto em [projeto](projeto)) é um conjunto de serviços de inteligência artificial (IA) em nuvem da Microsoft que fornece recursos para desenvolvedores e cientistas de dados criarem e implantarem soluções de IA inovadoras. O Azure AI Services oferece uma ampla gama de serviços, desde APIs pré-treinadas para tarefas como visão computacional e processamento de linguagem natural até ferramentas avançadas para machine learning e deep learning.

**Storage account (conta de armazenamento)**

#### Uma conta de armazenamento do Azure é um serviço em nuvem que fornece um local seguro e durável para armazenar seus dados. Podemos usar uma conta de armazenamento do Azure para guardar qualquer tipo de dado, incluindo os chamados [b]blobs, que são arquivos de qualquer tamanho, como imagens, vídeos e arquivos de texto.

### Indexação de documentos

#### É necessário submeter os documentos a indexação no AI Search no sentido de preparar e organizar documentos para que os mesmos possam ser pesquisados de forma eficiente. Seguindo o [tutorial da Microsoft], todo processo é definido e configurado para o funcionamento do mecanismo. 

[Figura 0 - Indexação]

#### Finalizado o processo, podemos explorar o índice dos documentos por meio da pesquisa instantânea no portal do Azure para testar consultas, feita pelo search explorer. 

#### Podemos perfeitamente aplicar esse conceito no gerenciador de pesquisa.

### Gerenciador de pesquisa (Search explorer)

#### Através da Search explorer podemos escrever e testar consultas, seja por query (palavra ou frase) ou por comando em formato JSON.
#### O estudo de caso analisado foi sobre a cafeteria [nome]. Deseja-se extrair informações no contexto da empresa e isso é possível através dos mecanismos de busca e extração do gerenciador de pesquisas.

#### Obs.: Como esse experimento é para fins de laboratório, a pesquisa está baseada na textos escritos em inglês. É possível utilizar outros dados em outras linguagens, desde que sejam feitas as devidas configurações de reconhecimento. 

#### No campo vazio da área de consulta, podemos usar a seguinte sintaxe:

search=locations:'Chicago'

[Foto 1 - Demonstração via query]

#### No contexto de gerenciamento de pesquisa no Azure AI Search, a query "search=locations:'Chicago'" com um índice específico significa:

* search: Esta palavra-chave indica que a consulta é uma pesquisa.

* locations: Este é o nome do campo que você está pesquisando. Neste caso, você está pesquisando no campo "locations".

* 'Chicago': Este é o valor que você está procurando no campo "locations". Está sendo procurado por documentos que contenham a palavra "Chicago" no campo "locations".

#### Observe que ao fazer a consulta, são retornados referências ao que foi pesquisado, ou seja, por meio do processamento de busca, o resultado é a saída na tela de todas as sentenças extraídas da base de dados da AI Search relacionados a essas querys solicitadas. 

#### No campo vazio da área de consulta, podemos usar as seguintes sintaxes:

```
{
"search": "sentiment:'negative'"
}

```

[Figura 2 - Demonstração via JSON query editor]

#### Fazendo uma sutil experiência, podemos trocar a palavra 'negative' por 'positive'. Veja os resultados de busca. 

### Insights

#### Na inteligência artificial, insights se referem a descobertas, conclusões ou informações valiosas obtidas a partir da análise de dados. São interpretações significativas que podem ser usadas para tomar decisões mais inteligentes, melhorar a eficiência, otimizar processos e gerar valor para uma organização.
#### É fundamental utilizar tais ferramentas, como o search explorer, no dia-dia, seja no trabalho ou em algum outro projeto envolvido, pois através de boas práticas de uso, o mesmo tem o potencial de elevar em grande escala a produtividade, ao produzir insights que pode representar decisões mais assertivas sobre um determinado contexto, o que acaba influenciando nos resultados esperados em um contexto específico.    

** Knowledge storage (armazenamento de conhecimento)**  

#### É possível enriquecer o banco de dados para a consulta pelo AI Search através de revisões e adição de novos arquivos ao armazenamento local, aumentando seu portfólio de busca e melhorando a experiência do usuário através de consultas mais assertivas. 

**Conclusão**

#### Para as empresas, os dados podem ser considerados como o "novo petróleo", uma vez que se cada vez se deseja saber como as pessoas pensam e assim atender suas necessidades, adaptando as ferramentas, como as que foram apresentadas, as necessidades das pessoas. Da mesma forma, os dados estão tendo um impacto significativo na sociedade, mudando a maneira como vivemos, trabalhamos e nos relacionamos. Por isso, o profissional de TI precisa estar atento a essa tendência  que tem sido cada dia mais uma realidade.

#### Referências

[Explorar um índice de Pesquisa de IA (UI) do Azure](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)
[Tutoriais do Azure AI Search](https://docs.microsoft.com/pt-br/azure/search/search-how-to-create-search-index)