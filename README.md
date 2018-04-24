O que é um Branch
Para compreender realmente a forma como o Git cria branches, precisamos dar um passo atrás e examinar como o Git armazena seus dados. Como você pode se lembrar do capítulo 1, o Git não armazena dados como uma série de mudanças ou deltas, mas sim como uma série de snapshots.

Quando você faz um commit no Git, o Git guarda um objeto commit que contém um ponteiro para o snapshot do conteúdo que você colocou na área de seleção, o autor e os metadados da mensagem, zero ou mais ponteiros para o commit ou commits que são pais deste commit: nenhum pai para o commit inicial, um pai para um commit normal e múltiplos pais para commits que resultem de um merge de dois ou mais branches.
