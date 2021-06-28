# Sniffer-c-
Este fork tem como objetivo a adição do protocolo IGMPv2 a lista de protocolos reconhecidos pelo programa.
Para fazer isso foi necessário a criação do cabeçalho IGMPv2, o qual concede as informações de checksum, do tipo do IGMPv2, do MaxResponseTime e do GroupAddress. Além disso, foi adicionada uma tratativa a mais na função listPackets_ItemSelectionChanged (presente no arquivo PraisedSnifferForm.cs) para quando ele receber um pacote IGMPv2 criar o Header apropriado e executar a função MakeInformationIGMP que insere as informações do pacote a árvore mostrada.
Por fim, para conseguir visualizar qualquer protocolo de forma mais fácil, foi adicionado um filtro por tipo de protocolo.

- Informações listadas: 
- Checksum
- Tipo do IGMPv2
- MaxResponseTime
- GroupAddress
- Origem
- Destino
