<html>




<head>
    <title>Calculadora</title>

    <link rel="stylesheet" href="calculadora.css" type='text/css'>
    <link rel="stylesheet" href="https://code.jquery.com/ui/1.11.4/themes/smoothness/jquery-ui.css">

    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>
    <script src="https://code.jquery.com/ui/1.11.4/jquery-ui.js"></script>
    <script src="https://code.jquery.com/jquery-3.5.0.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js"></script>

</head>

<body>

    <div>
        <h1 class="titulo1">Calculadora</h1>
    </div>

    <div class="AreaDoCirculo">

        <p class="subtitulo1">Área do círculo</p>

        <div class="raio">
            <input type="number" id="raio" placeholder="Raio">
        </div>

        <div>
            <button type="button" class="btn1" onclick="Calcula1()">Calcular</button>
        </div>
        <form>
            <div class="resultado1">
                <input type="text" placeholder="Resultado" id="area">
            </div>

        </form>

        <script>
            function Calcula1() {
                var raio = document.getElementById("raio").value;
                console.log(raio);
                var area = raio * raio * Math.PI;
                console.log(area);
                document.getElementById("area").placeholder = area;
            }
        </script>

    </div>

    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <hr class="dashed">
    <br>
    <br>
    <br>

    <div class="AreaDoTriangulo">

        <div class="subtitulo2">
            <p> Área do Triângulo</p>
        </div>

        <div>
            <h1 class="formula"> Fórmula: A = (b * h) / 2, onde A = área, b = base e h = altura</h1>
        </div>

        <form>

            <div class="base">
                <input type="number" placeholder="Base" id="base">
            </div>

            <div class="altura">
                <input type="number" placeholder="Altura" id="altura">
            </div>

            <button type="button" class="btn2" onclick="Calcula2()">Calcular</button>

        </form>

        <div class="resultado2">
            <input type="text" placeholder="Resultado" id="area2">
        </div>

        <script>
            function Calcula2() {
                var base = document.getElementById("base").value;
                var altura = document.getElementById("altura").value;
                var area = (base * altura) / 2;
                document.getElementById("area2").placeholder = area;
            }
        </script>

    </div>

    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <hr class="dashed">
    <br>
    <br>
    <br>

    <div class="fahrenheit">

        <div class="subtitulo3">
            <p> Conversão de Fahrenheit (°F) em Graus Celsius (°C)</p>
        </div>

        <form>

            <div class="valorF">
                <input type="number" placeholder="valor em °F" id="valor2">
            </div>

            <div class="btn">
                <button type="button" class="btn3" onclick="Calcular3()">Calcular</button>
            </div>

            <div class="Resultado3">
                <input type="text" placeholder="Conversão" id="conversão">
            </div>

        </form>

        <script type="text/javascript">
            function Calcular3() {
                var valor2 = document.getElementById("valor2").value;
                var conversão = ((valor2 - 32) * 0, 5556);
                document.getElementById("conversão").placeholder = conversão;
            }

        </script>
    </div>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <hr class="dashed">
    <br>
    <br>
    <br>

    <div class="PorcentagemDeDesconto">

        <div class="subtitulo4">
            <p>Calcule 5% de desconto:</p>
        </div>

        <div>
            <label for="valor" class="escrita2"> Digite o valor do Produto: </label> <br>
            <input type="text" id="valor" name="valor" placeholder="valor" class="valor" required class="form-control">
        </div>

        <div>
            <input type="text" id="pagar" class="desconto" placeholder="pagar">
            <input class="btn4" id="botao1" type="button" value="Calcular" onclick="Calcular4()">
        </div>

        <script>
            function Calcular4() {
                var valor = document.getElementById("valor").value;
                var resultado = document.getElementById("pagar");
                var desconto = 0;

                desconto = valor * 0.05;
                valor = valor * 0.95;

                resultado.value = "Desconto: " + desconto + ". Pagar: " + valor;
            }
        </script>

    </div>

    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <hr class="dashed">
    <br>
    <br>
    <br>

    <div class="NumeroAoCubo">

        <div class="subtitulo5">
            <p> Número ao Cubo</p>
        </div>

        <div class="valor3">
            <input type="number" placeholder="Digite um número" id="valor3">
        </div>

        <div class="cubo">
            <input type="number" placeholder="Resultado" id="cubo">
        </div>

        <div class="btn">
            <button type="button" class="btn5" onclick="Calcular5()">Calcular</button>
        </div>

        <script>
            function Calcular5() {
                var valor3 = document.getElementById("valor3").value;
                var cubo = (valor3 ** 3);

                document.getElementById("cubo").placeholder = cubo;
            }
        </script>

    </div>

    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <br>
    <hr class="dashed">
    <br>
    <br>
    <br>

    <div class="Idade">

        <div class="subtitulo6">
            <p> Descrição de Idade </p>
        </div>

        <div class="custo">
            <input type="number" placeholder="Idade" id="idade">
        </div>

        <div class="resultado4">
            <input type="text" placeholder="Resultado" id="resultado4">
        </div>

        <div class="btn">
            <button type="button" class="btn6" onclick="Calcular6()">Calcular</button>
        </div>

        <script>
            function Calcular6(event) {

                event.preventDefault();
                var idade = document.getElementById("idade").value;

                if (idade < 18) {
                    resultado4.innerHTML = "<br/> Seu resultado foi: " + idade.toFixed(2) + "<br/> Menor de idade";
                }
                else if (idade >= 18) {
                    resultado4.innerHTML = "<br/> Seu resultado foi: " + idade.toFixed(2) + "<br/> Maior de idade";
                }
            }

            document.getElementById("idade").placeholder = idade;

        </script>

    </div>

</body>


</html>
