# Detector de Obstáculos
<br>

## 1. Introdução 
<p align="justify">O projeto que está em desenvolvimento, tem como objetivo criar um dispositivo assistivo, usando a placa ESP32 e sensores ultrassônicos, para ajudar na navegação segura de pessoas cegas ou com deficiência visual. A ideia é montar o sistema em um óculos, para detectar obstáculos à frente do usuário. Durante a pesquisa, o grupo explorou desde os conceitos básicos de prototipagem até os testes iniciais de funcionamento dos sensores. Também foram definidos os requisitos funcionais e não funcionais, além das regras de negócio, que vão guiar o comportamento do sistema e garantir sua praticidade, usabilidade e eficiência, esses itens estão sendo implementados em um documento. A arquitetura inicial foi pensada para ser modular, consumir pouca energia e obter uma manutenção viável.

<br>

<br>

## 2. Planejamento

<p align="justify">O desenvolvimento do projeto foi estruturado em etapas sequenciais para garantir uma execução organizada, eficiente e baseada em boas práticas de desenvolvimento de tecnologias assistivas. Segundo Cook e Polgar (2020), "o planejamento cuidadoso é fundamental para que dispositivos assistivos sejam funcionais, aceitos pelos usuários e efetivamente promovam autonomia". As etapas do planejamento foram:

- **2.1 Cronograma básico da primeira parte do projeto SafeWalk**

| Atividade                                 | Abr. (M1)     | Mai. (M2) | Jun. (M3) | Jul. (M4) | Entrega       |
|--------------------------------------------|---------------|-----------|-----------|-----------|---------------|
| Primeira parte do projeto                  |               |           |           |           |               |
| Definição do projeto                       | ✔️            |           |           |           | 01/04/2025    |
| Pesquisa                                   | ✔️            |           |           |           | 14/04/2025    |
| Primeiros testes                           | ✔️            |           |           |           | 20/04/2025    |
| Levantamento de requisitos funcionais      | ✔️            |           |           |           | 24/04/2025    |
| Levantamento de requisitos não funcionais  | ✔️            |           |           |           | 26/04/2025    |
| Regras de negócio                          | ✔️            |           |           |           | 27/04/2025    |
| Começo da montagem da documentação         | ✔️            |           |           |           | 27/04/2025    |

<br>

- **2.2 Pesquisa Inicial**
  
<p align="justify">Levantamento de informações técnicas sobre sensores ultrassônicos, microcontroladores (ESP32), ergonomia em dispositivos vestíveis e necessidades específicas de pessoas com deficiência visual.

<br>

- **2.3 Ferramentas utilizadas**

 **1. Notebook :** Utilizado para fazer uso do código na IDE Arduino.

<p align="center">
  <img src="https://github.com/user-attachments/assets/54297056-a7dd-450e-a429-8c41fa748c52" width="400">
</p>

<br>

**2. IDE Arduino :** Utilizada para fazer a compilação do código junto à placa.

<p align="center">
  <img src="https://github.com/user-attachments/assets/e9a31fe2-e62f-49bc-a8c3-5407f4798798" width="400">
</p>

<br>

**3. Cabo Micro USB:** Utilizado para fazer ligação do notebook na placa através de uma entrada USB.
<p align="center">
  <img src="https://github.com/user-attachments/assets/2850047a-d2c1-4192-bdc8-8394159c0681" width="400">
</p>

Essas ferramentas foram essenciais para fazer o experimento da Placa ESP 23 com o sensor Ultrassônico HC-SR04.

<br>


- **2.4 Definição de Requisitos**

<p align="justify">Elaboração dos requisitos funcionais e não funcionais, alinhando o projeto às reais necessidades dos usuários finais. Segundo Miesenberger et al. (2022), "envolver as necessidades dos usuários desde o início do projeto é um fator determinante para o sucesso de tecnologias assistivas".

<br>

- **2.5 Prototipagem**
  
<p align="justify">Montagem inicial do sistema em protoboard para testes práticos. Esta fase permite identificar problemas de integração entre os componentes, conforme recomendações de Pahl e Beitz (2021) sobre desenvolvimento de protótipos de engenharia.

<br>

- **2.6 Simulação e Testes**

<p align="justify">Realização de simulações na IDE Arduino e testes em ambiente controlado para ajustar parâmetros como distância de detecção e tipo de alerta.

<br>

- **2.7 Documentação**

<p align="justify">Registro detalhado do processo de desenvolvimento, dificuldades encontradas, melhorias implementadas e resultados, garantindo transparência e a possibilidade de futuras replicações ou aprimoramentos do projeto.

<br>

<br>

## 3.Metodologia
<p align="justify">A metodologia empregada é de natureza aplicada, utilizando uma abordagem experimental e iterativa para o desenvolvimento de um dispositivo assistivo funcional. Essa abordagem foi escolhida com base nas diretrizes de desenvolvimento de tecnologias assistivas, que recomendam "a constante interação entre concepção, prototipagem, testes e validação com usuários" (Cook; Polgar, 2020).São as fases metodológicas:

<br>

- **3.1 Levantamento Bibliográfico**

<p align="justify">Pesquisa de referências atualizadas sobre deficiência visual, dispositivos de auxílio à locomoção, sensores ultrassônicos e microcontroladores. Essa etapa foi baseada na orientação de Gil (2023), que ressalta que "o embasamento teórico sólido é essencial para projetos científicos aplicados".

<br>

- **3.2 Desenvolvimento Técnico**

<p align="justify">Programação da placa ESP32 para a leitura dos sinais do sensor ultrassônico HC-SR04, com ajustes de parâmetros de distância e resposta ao obstáculo. Seguindo a orientação de Horowitz e Hill (2022), "testes práticos de hardware e software devem ocorrer de forma simultânea para acelerar o desenvolvimento e a identificação de falhas".

<br>

- **3.3 Construção do Protótipo**

<p align="justify">Montagem em protoboard, testes com diferentes alertas (vibração e sonoro) e desenvolvimento do suporte vestível (óculos), visando conforto e leveza. De acordo com Müller et al. (2021), "o conforto e a discrição são fatores críticos para o sucesso de dispositivos vestíveis assistivos".

<br>

- **3.4 Testes Experimentais**

<p align="justify">Realização de testes de campo em ambientes internos e externos, com diferentes tipos de obstáculos e superfícies. Esta fase segue a recomendação de Shinohara e Wobbrock (2020), que destacam que "o teste em ambiente real é fundamental para validar a eficácia de tecnologias assistivas".

<br>

<br>

## 4. Objetivos

<p align="justify">Desenvolver um dispositivo assistivo vestível, utilizando a placa ESP32 e sensores ultrassônicos, para detectar obstáculos e alertar pessoas cegas ou com deficiência visual, visando promover maior autonomia, segurança e qualidade de vida na locomoção diária. Encontramos alguns problemas com relação aos meios tradicionais utilizados por deficientes visuais, visto que, quando um ceguinho utiliza uma bengala ainda há muitas chances de esbarrar em um obstáculo com isso em mente, precisamos responder algumas questões. 

<br>

- **4.1 Qual é o problema que o projeto resolve?**

<p align="justify">O projeto busca resolver a dificuldade enfrentada por pessoas cegas ou com deficiência visual na detecção de obstáculos em seu trajeto. A mobilidade segura é um desafio constante, pois muitos obstáculos elevados, fora do alcance da bengala tradicional, podem passar despercebidos, aumentando o risco de quedas e acidentes.
Segundo Lima e Silveira (2021), "a mobilidade de pessoas com deficiência visual depende de dispositivos que sejam capazes de detectar obstáculos de forma eficiente, para proporcionar autonomia e segurança". Além disso, estudos mostram que soluções de tecnologia assistiva baseadas em sensores eletrônicos podem ampliar significativamente a percepção do ambiente (Santos & Rodrigues, 2020).

<br>

- **4.2 Qual é o público-alvo?**
  
<p align="justify">O público-alvo do projeto são pessoas cegas ou com deficiência visual parcial que necessitam de auxílio para uma locomoção mais segura e independente em ambientes internos e externos.

<br>

<p align="center">
  <img src="https://github.com/user-attachments/assets/16b25892-8d82-4b6c-94e1-0ded079daf8e" width="600">
</p>

<p align="justify">De acordo com a Organização Mundial da Saúde (OMS), mais de 2,2 bilhões de pessoas em todo o mundo têm algum grau de deficiência visual, sendo que "pelo menos 1 bilhão desses casos poderiam ser evitados ou ainda não foram tratados" (OMS, 2019). Isso reforça a importância de dispositivos que aumentem a acessibilidade e a autonomia desse público.    (Não precisa já que são dados da OMS, se ele discorda lá na frente eu defendo.)

<br>


- **4.3 Qual a justificativa da escolha?**
  
<p align="justify">A escolha do projeto se justifica pela necessidade crescente de desenvolver tecnologias acessíveis, de baixo custo e eficientes para apoiar a mobilidade de pessoas com deficiência visual. Apesar de existirem algumas soluções no mercado, muitas delas são caras, limitadas em alcance ou desconfortáveis no uso contínuo.
Segundo Bersch (2018), "tecnologias assistivas devem ser projetadas para serem funcionais, acessíveis e confortáveis, de forma a promover efetivamente a inclusão e autonomia das pessoas com deficiência". A utilização de componentes como o ESP32 e sensores ultrassônicos HC-SR04 torna o projeto viável financeiramente e tecnicamente.

<br>

- **4.4 Concorrentes**

- *4.4.1 Projeto AnnuitWalk (PAW)*

<p align="justify">O Projeto AnnuitWalk foi desenvolvido por estudantes de Pernambuco e consiste em óculos equipados com sensores ultrassônicos que detectam obstáculos. O alerta é feito por meio de uma pulseira vibratória, liberando os ouvidos do usuário para sons do ambiente e aumentando sua segurança (UNA-SUS, 2022).

<br>

- *4.4.2 Envision Glasses*

<p align="justify">Os Envision Glasses são óculos inteligentes desenvolvidos para transformar imagens capturadas em informações sonoras. Utilizando inteligência artificial avançada, eles conseguem reconhecer e descrever pessoas, ler textos impressos ou manuscritos em tempo real, identificar objetos e interpretar ambientes (ENVISION, 2025).
Uma vantagem dos Envision Glasses é a independência que proporcionam ao usuário, já que a análise é feita no próprio dispositivo, sem depender constantemente de outra pessoa. Apesar de sua tecnologia avançada, o custo elevado ainda é uma barreira para grande parte dos usuários que mais necessitam desse tipo de solução.

<br>

- *4.4.3 Biped AI*

<p align="justify">O Biped AI é um dispositivo vestível que se assemelha a um colete e utiliza tecnologia de carros autônomos aplicada à locomoção de pedestres com deficiência visual. Ele combina câmeras 3D e inteligência artificial para prever movimentos e detectar obstáculos em tempo real (BIPED, 2025).
O dispositivo fornece alertas discretos por áudio, permitindo que o usuário caminhe de maneira mais segura e preditiva, antecipando possíveis colisões. O Biped AI ainda é relativamente novo no mercado, e seu custo também é elevado, além de exigir atualizações constantes para manter a precisão da navegação.

<br>

<br>

## 5. Prototipagem Inicial

- **5.1. Itens Utilizados:**

<p align="justify">a) Sensor Ultrassônico HC-SR04: Utilizado para detectar obstáculos à frente do usuário, emitindo sinais sonoros que refletem nos objetos e retornam ao sensor, permitindo calcular a distância (CAMPOS et al., 2023).​

<p align="justify">b) ESP32: Microcontrolador com conectividade Wi-Fi e Bluetooth, responsável pelo processamento dos dados dos sensores e controle dos atuadores, como buzzer ou motor vibratório (SOUSA; ALVES, 2022).

<p align="justify">Na fase de prototipagem do dispositivo assistivo, foi adotado o sensor ultrassônico HC-SR04, amplamente utilizado em projetos de robótica e automação (CAMPOS et al., 2023). Este sensor é capaz de medir distâncias com base no tempo de resposta de um sinal sonoro refletido por um obstáculo, utilizando dois componentes: um emissor e um receptor de ondas sonoras.

<br>

- **5. 2. Como o Sensor Detecta Obstáculos**

<p align="justify">O sensor envia um pulso sonoro ultrassônico que viaja pelo ar. Quando esse pulso encontra um objeto, ele é refletido de volta ao sensor. O microcontrolador (como o ESP32) calcula a distância com base no tempo que o sinal levou para retornar (SOUSA; ALVES, 2022). Essa medida pode ser usada para acionar alertas, como vibração ou som, quando um objeto estiver a uma distância mínima definida (por exemplo, 50 cm).

<br>

- **5.3. Simulações**

<p align="justify">As simulações estão sendo realizadas na IDE do Arduino, onde é possível testar a leitura dos sensores e simular os alertas. Também estão sendo feitas montagens físicas em protoboard para testar a resposta do sistema em tempo real com obstáculos variados (FINIO, 2025).

<br>

<br>

## 6. Conclusão
<p align="justify">A primeira fase do projeto nos deu uma boa compreensão tanto da parte técnica quanto dos requisitos de engenharia e acessibilidade envolvidos. A pesquisa até agora, mostrou que os sensores ultrassônicos são uma opção viável para detectar obstáculos, e, com os primeiros testes, já foi possível validar essa função básica. A definição dos requisitos e regras de negócio garante que o desenvolvimento esteja alinhado às necessidades reais dos usuários. Os próximos passos incluem implementar alertas táteis ou sonoros, ajustar o design e fazer testes com usuários para validar a experiência. O projeto continua avançando com foco em acessibilidade, segurança e inclusão.

 <br>

 <br>
 
# Referências

<p align="justify">FINIO, Ben. Obstacle Detecting Glasses. Science Buddies, 2025. Disponível em: https://www.sciencebuddies.org/science-fair-projects/project-ideas/Elec_p108/electricity-electronics/obstacle-detecting-glasses. Acesso em: 25 abr. 2025.

<p align="justify">CAMPOS, Vinícius et al. Desenvolvimento de dispositivos assistivos baseados em sensores para deficientes visuais. Revista Científica Multidisciplinar, v. 13, n. 2, 2023.

<p align="justify">SOUSA, Marina R.; ALVES, Thiago G. Avaliação de sensores aplicados à mobilidade de deficientes visuais. In: Anais do Congresso Brasileiro de Engenharia Biomédica, 2022.

<p align="justify">LIMA, R. A.; SILVEIRA, D. T. Auxílio de navegação para deficientes visuais: tecnologias e desafios. Congresso Brasileiro de Engenharia Biomédica, 2021. Disponível em: https://sbeb.org.br/wp-content/uploads/2024/10/SBEB-CBEB2024-ProceedingsFinal.pdf. Acesso em: 26 abr. 2025.

<p align="justify">SANTOS, J. R.; RODRIGUES, D. F. Dispositivos eletrônicos assistivos para orientação de deficientes visuais. Revista Tecnologia e Sociedade, 2020. Disponível em: https://rsdjournal.org/index.php/rsd/article/download/26859/23595/315665. Acesso em: 25 abr. 2025.

<p align="justify">ALMEIDA, L. P.; SANTOS, F. C.; OLIVEIRA, R. M. Tecnologia Assistiva: um estudo sobre dispositivos vestíveis para deficientes visuais. Revista Brasileira de Inclusão, 2020. Disponível em: https://periodicos.ufba.br/index.php/nit/article/view/43946. Acesso em: 24 abr. 2025.

<p align="justify">COOK, Albert M.; POLGAR, Susan M. Assistive Technologies: Principles and Practice. 5. ed. Elsevier, 2020. Disponível em: https://www.elsevier.com/books/assistive-technologies/cook/978-0-323-58333-2. Acesso em: 26 abr. 2025.

<p align="justify">MIESENBERGER, Klaus et al. Assistive Technology: From Research to Practice. IOS Press, 2022. Disponível em: https://ebooks.iospress.nl/volume/assistive-technology-from-research-to-practice. Acesso em: 26 abr. 2025.

<p align="justify">PAHL, G.; BEITZ, W. Projeto na Engenharia: Fundamentos do Desenvolvimento de Produtos. 8. ed. Springer, 2021. Disponível em: https://link.springer.com/book/10.1007/978-3-662-61234-3. Acesso em: 26 abr. 2025.

<p align="justify">PRESSMAN, Roger S. Engenharia de Software. 9. ed. McGraw Hill, 2020. Disponível em: https://www.mheducation.com/highered/product/engenharia-software-pressman/9788576056861.html. Acesso em: 26 abr. 2025.

<p align="justify">GIL, Antônio Carlos. Métodos e Técnicas de Pesquisa Social. 7. ed. Atlas, 2023. Disponível em: https://www.atlas.com.br/metodos-e-tecnicas-de-pesquisa-social-7-edicao-2023. Acesso em: 26 abr. 2025.

<p align="justify">HOROWITZ, Paul; HILL, Winfield. The Art of Electronics. 3. ed. Cambridge University Press, 2022. Disponível em: https://www.cambridge.org/core/books/art-of-electronics/8D3A8D0C58E1185E38D6AD9AC5F75ED0. Acesso em: 26 abr. 2025.

<p align="justify">MÜLLER, Christian et al. Wearable Technology for People with Disabilities. Springer, 2021. Disponível em: https://link.springer.com/book/10.1007/978-3-030-76894-5. Acesso em: 26 abr. 2025.

<p align="justify">SHINOHARA, Kristen; WOBBROCK, Jacob O. Tenets for the Evaluation of Accessible Technology. ACM Transactions on Accessible Computing, 2020. Disponível em: https://dl.acm.org/doi/10.1145/3380954. Acesso em: 26 abr. 2025.

<p align="justify">LEVAC, Danielle E. et al. Advancing the Science of User Involvement in Rehabilitation Technology Development. Disability and Rehabilitation: Assistive Technology, 2021. Disponível em: https://www.tandfonline.com/doi/full/10.1080/17483107.2021.1878207. Acesso em: 26 abr. 2025.

<p align="justify">ALMEIDA, Lucas et al. Design de dispositivos vestíveis para acessibilidade. Revista de Inovação Tecnológica, 2020. Disponível em: https://revistainovacaotecnologica.com.br/artigo/design-de-dispositivos-vestiveis-para-acessibilidade. Acesso em: 26 abr. 2025.

<p align="justify">ENGENHARIA 360. Conheça os óculos inteligentes que auxiliam pessoas com deficiência visual a "enxergar". Disponível em: https://engenharia360.com/oculos-inteligentes-orcam-myeye/. Acesso em: 28 abr. 2025.

<p align="justify">ENVISION. Envision Glasses: óculos inteligentes para pessoas com deficiência visual. 2025. Disponível em: https://www.letsenvision.com/glasses. Acesso em: 28 abr. 2025.

<p align="justify">BIPED. Biped AI: tecnologia de navegação para pessoas com deficiência visual. 2025. Disponível em: https://www.biped.ai/. Acesso em: 28 abr. 2025.
