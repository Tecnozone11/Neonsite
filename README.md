# Neonsite
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechNeon - Soluções Digitais</title>
    <link rel="stylesheet" href="style.css" />
</head>
<body>
    <header>
        <h1 class="neon-text">TechNeon</h1>
        <p>Soluções digitais com estilo futurista</p>
        <nav>
            <a href="#calculators">Calculadoras</a>
            <a href="#puzzle">Quebra-Cabeça</a>
            <a href="#quiz">Quiz</a>
        </nav>
    </header>
    
    <div class="container">
        <section id="calculators">
            <h2><span class="neon-text">Ferramentas Úteis</span></h2>
            <div class="tool-grid">
                <div class="tool-card floating" style="animation-delay: 0.2s;">
                    <h3>Calculadora de Peso</h3>
                    <p>Converta seu peso entre diferentes planetas</p>
                    <div class="form-group">
                        <label for="earth-weight">Seu peso na Terra (kg):</label>
                        <input type="number" id="earth-weight" placeholder="Digite seu peso">
                    </div>
                    <div class="form-group">
                        <label for="planet">Planeta:</label>
                        <select id="planet">
                            <option value="mercury">Mercúrio</option>
                            <option value="venus">Vênus</option>
                            <option value="mars">Marte</option>
                            <option value="jupiter">Júpiter</option>
                            <option value="saturn">Saturno</option>
                            <option value="uranus">Urano</option>
                            <option value="neptune">Netuno</option>
                            <option value="pluto">Plutão</option>
                            <option value="moon">Lua</option>
                        </select>
                    </div>
                    <button id="calculate-weight">Calcular</button>
                    <div id="weight-result" class="result">
                        <p>Seu peso em <span id="planet-name"></span>: <span id="calculated-weight"></span> kg</p>
                    </div>
                </div>
                
                <div class="tool-card floating" style="animation-delay: 0.4s;">
                    <h3>Conversor de Moedas</h3>
                    <p>Converta entre as principais moedas do mundo</p>
                    <div class="form-group">
                        <label for="amount">Valor:</label>
                        <input type="number" id="amount" placeholder="Digite o valor">
                    </div>
                    <div class="form-group">
                        <label for="from-currency">De:</label>
                        <select id="from-currency">
                            <option value="USD">Dólar Americano (USD)</option>
                            <option value="BRL">Real Brasileiro (BRL)</option>
                            <option value="EUR">Euro (EUR)</option>
                            <option value="GBP">Libra Esterlina (GBP)</option>
                            <option value="JPY">Iene Japonês (JPY)</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="to-currency">Para:</label>
                        <select id="to-currency">
                            <option value="BRL">Real Brasileiro (BRL)</option>
                            <option value="USD">Dólar Americano (USD)</option>
                            <option value="EUR">Euro (EUR)</option>
                            <option value="GBP">Libra Esterlina (GBP)</option>
                            <option value="JPY">Iene Japonês (JPY)</option>
                        </select>
                    </div>
                    <button id="convert-currency">Converter</button>
                    <div id="currency-result" class="result">
                        <p><span id="original-amount"></span> <span id="from-currency-name"></span> = <span id="converted-amount"></span> <span id="to-currency-name"></span></p>
                    </div>
                </div>
            </div>
        </section>
        
        <section id="puzzle">
            <h2><span class="neon-text">Quebra-Cabeça Deslizante</span></h2>
            <p>Tente organizar os números em ordem crescente movendo as peças para o espaço vazio.</p>
            <div class="puzzle-container" id="puzzle-board">
                <!-- As peças serão geradas pelo JavaScript -->
            </div>
            <button id="shuffle-puzzle" style="margin-top: 1.5rem; max-width: 300px; margin-left: auto; margin-right: auto;">Embaralhar</button>
            <div id="puzzle-message" style="text-align: center; margin-top: 1rem; color: var(--neon-green); display: none;"></div>
        </section>
        
        <section id="quiz">
            <h2><span class="neon-text">Quiz Tecnológico</span></h2>
            <p>Teste seus conhecimentos sobre tecnologia com este quiz interativo!</p>
            
            <div class="quiz-container">
                <div id="quiz-questions">
                    <!-- As perguntas serão geradas pelo JavaScript -->
                </div>
                <button id="submit-quiz" style="display: none;">Verificar Respostas</button>
                <div id="quiz-score" class="quiz-result">
                    Você acertou <span id="correct-answers">0</span> de <span id="total-questions">0</span> perguntas!
                </div>
            </div>
        </section>
    </div>
    
    <footer>
        <p>&copy; 2023 TechNeon - Todos os direitos reservados</p>
        <p style="margin-top: 0.5rem;">Desenvolvido com ❤️ e efeitos neon</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
