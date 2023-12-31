# Trabalho realizado na Semana #3

## Identificação

- Esta vulnerabilidade é conhecida por FORCEDENTRY e afeta as versões do macOS anteriores a 11.6, as do iOS precedentes à 14.8 e as do watchOS que precedem a 7.6.
- Com este exploit o atacante pode corromper a memória e ficheiros do dispositivo, no entanto, não consegue assumir o controlo do dispositivo. 
- Este ataque não necessita de privilégios para funcionar.

## Catalogação

- Foi descoberto pela organização Citizen Lab em março de 2021, suspeitando-se que o exploit fosse utilizado desde fevereiro do mesmo ano.
- Esta vulnerabilidade resulta em memória corrompida e integridade de ficheiros corrompida. No entanto, não permite ao atacante ganhar acesso ao dispositivo em questão.
- Não é necessário qualquer tipo de autenticação nem de interação da vítima (zero-click attack).
- De acordo com o "National Institute of Standards and Technology", este exploit obteve uma pontuação de severidade de 7.8 (alto).

## Exploit

- Resulta do overflow de um inteiro no processo de renderizar uma imagem da Apple (CoreGraphics).
- Bastava a um atacante mandar um ficheiro .pdf ou .gif para comprometer o dispositivo.
- Apesar de ter extensão .gif, era na verdade um ficheiro de 748-byte Adobe PSD que causava um IMTranscoderAgent crash no dispositivo.
- Alguns dos .gif encontrados no sistema eram ficheiros PDF encriptados com o protocolo JBIG2.

## Ataques

- Foi determinado que o NSO Group utilizou esta vulnerabilidade através do spyware Pegasus.
- Embora não se saiba exatamente o número de ataques, é estimado que este exploit tenha sido utilizado em vários dispositivos, por exemplo, telemóveis de ativistas.
- Muitos clientes desta firma são governos e organizações, sendo credível que alguns aparelhos afetados tenham sido atacados a mando destes. 

