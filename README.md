# Projeto-Padr-o-Memento


 Classification -> Padrão Comportamental
 
 
 
 
Intent -> Permite capturar e externalizar  um estado  interno  interno  de objeto  possa ser  restaurado  para esse estado  mais tarde.



Applicability -> Sempre  quando houver  a necessidade de se criar pontos  de restauração de estado de objeto. Permitir que o programa se recupere  de erros.



Objetivo ->É fornecer  um mecanismo  para permitir  atender  esta demanda sem violar o principio de encapsulamento  da Orientação a Objetos.




Participantes

Memento -> Classe  que representa um snapshot,contendo o estado de um objeto  a ser restaurado em um Originador.Possui método para obter e definir  o estado que um  Memento  encapsula dentro.


Originador -> Classe na qual  o estado  atual é mantido. Define  método que permite criar  um Memento com o estado  atual do Originador armazenado no memento retornado.Originador também tem um método que define seu estado atual com  de um determinado  objeto Memento. Portanto , pode criar  um Snapshot (Memento) ou restaurar o estado do Snapshot fornecido (Mementos)


Caretaker-> Classe  auxiliar responsavel por armazenar  e restaurar o estado  do Originador por meio do objeto Memento.Um objeto Caretaker mantém os  membros , mas nunca  modifica os Mementos.
