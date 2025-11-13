# stereo_camera_calibration

Este é um projeto que busca utilizar um par de câmeras, onde seus parâmetros intrínsecos ainda desconhecidos, para obter uma imagem sem distorções, simulando um terceiro ponto de observação.

## Você acha que conhece sua câmera?

Todas as câmeras possuem estes parâmetros de distorção de imagem:

- <b> fx </b>
- <b> fy </b>
- <b> skew </b>
- <b> cx </b>
- <b> cy </b>
- <b> w,d </b>

O resultado da literal >imagem< é uma combinação destes parâmetros dos quais a lente produz! Para corrigir estes erros de imagem, vamos primeiro determinar estes parâmetros de suas câmeras, para depois começar a brincar de verdade <i> hahahaha </i>

### Para responder a essa pergunta, vamos utilizar o BoofCV e um padrão de calibração de câmeras:

- Obtenha uma placa de Xadrez ou um padrão óptico para calibração de câmeras!
- Instale o Java SDK 11 ou superior a partir de https://www.oracle.com/java/technologies/downloads/#jdk25-windows
- Faça o download do módulo boofcv desejado ("boofcv-core-1.2.4-javadoc.jar" foi utilizado neste projeto) a partir de https://central.sonatype.com/artifact/org.boofcv/boofcv-core/versions
- Extraia o conteúdo da pasta e execute applications.bat a partir da pasta BoofApplications
- Selecione a opção "Assisted Calibration"
- Siga os passos e armazene os 6 resultados presentes na aba "Calib"

### E agora?

Bom, agora vamos ver como está a sua imagem corrigida! Para isso:
- Baixe o arquivo "ver3.py" e insira os parâmetros que você obteve lá do BoofCV com sua câmera
- <i> Et voilá! </i>, as duas imagens exibidas em tempo real refletem sua câmera com e sem distorções!
- ****inserir imagem comparativo*****
