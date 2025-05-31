# Código de teste
A seguir, o código que utilizamos para fazer os primeiros testes:

    #define TRIG 33
    #define ECHO 32

    void setup() {
      Serial.begin(9600);
      Serial.println("Iniciando ESP32...");
      pinMode(TRIG, OUTPUT);
      pinMode(ECHO, INPUT);
    }

    void loop() {
      long duracao;
      int distancia;

      digitalWrite(TRIG, LOW);
      delayMicroseconds(2);
      digitalWrite(TRIG, HIGH);
      delayMicroseconds(10);
      digitalWrite(TRIG, LOW);

      duracao = pulseIn(ECHO, HIGH);

      if (duracao == 0) {
    Serial.println("Fora de alcance ou sem resposta do sensor.");
      } else {
    distancia = duracao * 0.04 / 2;

    if (distancia > 400) {
      Serial.println("Distância fora do alcance do sensor (> 400 cm).");
    } else {
      Serial.print("Distância: ");
      Serial.print(distancia);
      Serial.println(" cm");
    }
    }

    delay(500);
    }
