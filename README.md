# PWM-TAREFA
Controle de Servo Motor com Raspberry Pi Pico
# Controle de Servo Motor com Raspberry Pi Pico

## Descrição
Este projeto utiliza um Raspberry Pi Pico para controlar um servo motor via PWM. O servo motor é movimentado entre as posições de 0°, 90° e 180°. Além disso, há uma rotina para movimentação suave entre os ângulos extremos.

## Requisitos
- Raspberry Pi Pico
- Servo motor compatível com PWM
- Software Pico SDK configurado

## Instalação e Uso
### Configuração do Ambiente
1. Instale o [Pico SDK](https://github.com/raspberrypi/pico-sdk) e configure seu ambiente de desenvolvimento.
2. Clone o repositório e entre na pasta do projeto:
   ```sh
   git clone <URL_DO_REPOSITORIO>
   cd <NOME_DO_PROJETO>
   ```
3. Compile o código usando CMake:
   ```sh
   mkdir build
   cd build
   cmake ..
   make
   ```
4. Carregue o arquivo `.uf2` gerado no Raspberry Pi Pico.

## Funcionamento
1. O programa inicia posicionando o servo motor em 180°.
2. Após 5 segundos, o servo vai para 90°.
3. Depois de mais 5 segundos, o servo se move para 0°.
4. Em seguida, o servo começa um movimento contínuo e suave entre 0° e 180°.

## Resultados e Observações
Durante a execução, observou-se que:
- A movimentação suave do servo melhora a estabilidade do sistema.
- O código permite ajustes simples para modificar os tempos e ângulos do servo.

## Conclusão
Este projeto demonstra o uso do Raspberry Pi Pico para controle de um servo motor utilizando PWM. A implementação pode ser expandida para aplicações mais complexas, como robótica e automação.

## Feito por
Eliseu Araujo Rios Neto
**MITLicense
