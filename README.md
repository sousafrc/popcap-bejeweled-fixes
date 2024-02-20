Correção de problemas e bugs nos jogos Bejeweled da PopCap, como suporte para Aceleração 3D, gráficos em resolução 'Alta' e 'Ultra', suporte para GPU mais recentes, correção de falha de memória de vídeo insulficiente, correção de falha na verificação de assinaturas no registro e algumas outras correções não listadas.

Instruções para aplicação das correções:
* Escolha o jogo apropriado nas releases deste repositório (certificando-se de selecionar a edição correta do jogo e a versão apropriada. Se não houver releases disponíveis para a edição/versão que você possui do Bejeweled, você pode tentar releases de outras edições/versões e ver se elas funcionam ou criar uma "issue" com um link para a sua versão do jogo no repositório, para que eu possa dar uma olhada).
* Baixe a release escolhida e extraia o arquivo.
* Agora é hora de escolher o sufixo que você quer utilizar. Após escolhido renomeie o excutável escolhido apagando o sufixo (por exemplo: renomeie "Bejeweled3-nosig+vmem+vcard.exe" para "Bejeweled3.exe"); 
* Agora copie e substitua o executável renomeado diretamente para a pasta do jogo;

compat.cfg:
Observe que você também deve substituir o arquivo "compat.cfg" na pasta do jogo (caso ele esteja disponível para sua versão) para suporte de resolução "Alta" e "Ultra". A Aceleração 3D funcionará sem este arquivo, mas você não poderá escolher nenhuma outra resolução além de "Normal".

Execute o arquivo "Test3D-clean.reg" para a sua versão antes de executar o jogo modificado! Isso eliminará quaisquer entradas de registro que possam estar impedindo a correção de funcionar.

Explicações dos sufixos:
* original -> Arquivo não alterado (sem correções)
* nosig -> Evita erros de falha na verificação de assinatura
* vmem -> Correção para 'Falha: Memória de vídeo insuficiente' no registro
* vcard -> Correção para 'Aviso: Placa de vídeo não suportada: %s' no registro

/experimental:
A pasta "experimental", como o nome sugere, é para uso experimental e não é uma solução de correção final. No entanto, você pode tentar brincar com o que está lá caso as correções principais não funcionarem.

Se você encontrar qualquer outro erro além dos corrigidos acima, crie uma "issue" informando o erro e eu tentarei investigar quando tiver tempo.