<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TERCEIRO</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap');
        body {
    margin: 0;
    font-family: 'Poppins', Arial, sans-serif;
    display: flex;
    background: #f5f6f7;
    color: #333;
}

.menu {
    background: linear-gradient(135deg, #4caf50, #81c784);
    height: 100vh;
    width: 200px; /* Largura reduzida */
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-top: 20px; /* Padding reduzido */
    box-shadow: 2px 0 4px rgba(0, 0, 0, 0.1);
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1000;
    border-right: 2px solid #ffffff; /* Borda reduzida */
    transition: width 0.3s ease;
}

.menu:hover {
    width: 220px;
}

.premium-header {
    color: #ffffff;
    font-size: 20px; /* Fonte reduzida */
    font-weight: 700;
    text-align: center;
    margin-top: 15px; /* Margem reduzida */
    text-transform: uppercase;
    letter-spacing: 1px; /* Espaçamento reduzido */
    border-bottom: 2px solid #ffffff; /* Borda reduzida */
    padding-bottom: 8px; /* Padding reduzido */
}

.menu-item {
    color: #ffffff;
    text-decoration: none;
    font-size: 16px; /* Fonte reduzida */
    margin: 15px 0; /* Margem reduzida */
    text-align: center;
    width: 100%;
    padding: 8px 15px; /* Padding reduzido */
    border-radius: 6px; /* Bordas arredondadas menores */
    transition: background-color 0.3s ease, transform 0.3s ease;
    position: relative;
    display: block;
}

.menu-item:hover {
    background-color: rgba(255, 255, 255, 0.2);
    transform: scale(1.03); /* Escala reduzida */
}

.menu-item::after {
    content: '';
    position: absolute;
    left: 0;
    bottom: 0;
    width: 0;
    height: 2px; /* Altura reduzida */
    background: #ffffff;
    transition: width 0.3s ease;
}

.menu-item:hover::after {
    width: 100%;
}

.section-container {
    margin-left: 200px;
    padding: 15px; /* Padding reduzido */
    width: calc(100% - 200px);
    background-color: #ffffff;
    border-radius: 6px; /* Bordas arredondadas menores */
    box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
}

.form-container {
    display: flex;
    flex-direction: column;
    gap: 10px; /* Espaçamento reduzido entre os campos */
}

.form-group {
    margin-bottom: 10px; /* Margem reduzida */
}

.form-group label {
    display: block;
    margin-bottom: 3px; /* Margem reduzida abaixo do rótulo */
    font-weight: 500;
    color: #4caf50;
}

.form-group input,
.form-group textarea,
.form-group select {
    width: 100%;
    padding: 8px; /* Padding reduzido */
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 14px; /* Tamanho da fonte reduzido */
}

.form-group textarea {
    resize: vertical;
    height: 50px; /* Altura reduzida para o textarea */
}

.form-group button {
    background-color: #4caf50;
    color: #fff;
    border: none;
    padding: 6px 12px; /* Padding reduzido */
    border-radius: 4px;
    cursor: pointer;
    font-size: 14px; /* Tamanho da fonte reduzido */
    margin-right: 8px; /* Margem reduzida */
}

.form-group button.clear-button {
    background-color: #f44336;
}

.form-group button:hover {
    opacity: 0.9;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); /* Sombra reduzida */
}

.form-group button.clear-button:hover {
    opacity: 0.9;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2); /* Sombra reduzida */
}

h2 {
    margin-bottom: 15px; /* Margem reduzida */
    color: #4caf50;
    font-size: 18px; /* Tamanho da fonte reduzido */
}

.instructions {
    margin-bottom: 15px; /* Margem reduzida */
    font-size: 14px; /* Tamanho da fonte reduzido */
    color: #333;
}

.instructions h3 {
    margin-top: 15px; /* Margem reduzida */
    font-size: 16px; /* Tamanho da fonte reduzido */
    color: #4caf50;
}

.alert {
    background-color: #ffdddd;
    border: 1px solid #f5c6cb;
    color: #721c24;
    padding: 8px; /* Padding reduzido */
    margin-bottom: 15px; /* Margem reduzida */
    border-radius: 4px;
    font-weight: bold;
    text-align: center;
    font-size: 14px; /* Tamanho da fonte reduzido */
    animation: blink 2s ease-in-out infinite;
}

@keyframes blink {
    0% { opacity: 1; }
    50% { opacity: 0.3; }
    100% { opacity: 1; }
}

table {
    width: 100%;
    border-collapse: collapse;
    margin-bottom: 10px; /* Margem reduzida */
    font-family: 'Poppins', Arial, sans-serif;
    font-size: 14px; /* Tamanho da fonte reduzido */
    color: #333;
}

table, th, td {
    border: 1px solid #e0e0e0;
}

th, td {
    padding: 8px; /* Padding reduzido */
    text-align: left;
}

th {
    background-color: #4caf50;
    color: #fff;
    font-weight: 500;
}

td {
    background-color: #ffffff;
}

.btn-gere-vistoria {
    display: inline-block;
    background-color: #4caf50;
    color: #fff;
    padding: 8px 16px;
    font-size: 14px;
    border-radius: 4px;
    text-decoration: none;
    text-align: center;
    margin-top: 20px;
    transition: background-color 0.3s ease, transform 0.3s ease;
}

.btn-gere-vistoria:hover {
    background-color: #45a049;
    transform: scale(1.02);
}

.container {
    max-width: 600px;
    margin: auto;
    padding: 20px;
    background: #fff;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

h1 {
    color: #333;
}

.field {
    margin-bottom: 15px;
}

.field label {
    display: block;
    font-weight: bold;
}

.field input {
    width: 100%;
    padding: 8px;
    margin-top: 5px;
    border: 1px solid #ddd;
    border-radius: 4px;
}

.observacao {
    color: red;
}

.modal {
    display: none;
    position: fixed;
    z-index: 1;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5); /* Fundo transparente */
}

/* Conteúdo da modal */
.modal-content {
    background-color: #fefefe;
    margin: auto;
    padding: 20px;
    border: 1px solid #888;
    width: 90%; /* Aumenta a largura da modal */
    max-width: 800px; /* Aumenta o tamanho máximo */
    border-radius: 10px;
    max-height: 90vh;
    overflow-y: auto;
    position: relative;
    top: 50%;
    transform: translateY(-50%);
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
}

/* Estilo do formulário horizontal */
.form-horizontal {
    display: flex;
    flex-wrap: wrap; /* Permite que os campos "quebrem" linha se necessário */
    gap: 20px; /* Espaçamento entre os campos */
}

.form-horizontal .form-group {
    flex: 1 1 45%; /* Faz com que os campos ocupem 45% da largura, lado a lado */
    display: flex;
    flex-direction: column;
}

.form-horizontal label {
    margin-bottom: 5px; /* Margem reduzida */
}

    .button-onclick {
    background-color: #17b9c5; /* Cor de fundo vermelha */
    color: white; /* Texto branco para contraste */
    padding: 10px 20px; /* Ajuste de padding para tornar o botão mais confortável */
    border: none; /* Remove a borda padrão */
    border-radius: 5px; /* Cantos arredondados */
    cursor: pointer; /* Cursor de mão para indicar que é clicável */
    transition: background-color 0.3s ease; /* Transição suave ao mudar a cor */
    font-size: 16px; /* Tamanho da fonte do botão */
    font-weight: bold; /* Deixa o texto do botão em negrito */
}

.button-onclick:hover {
    background-color: #c9d1da; /* Cor mais escura ao passar o mouse */
}
.alert {
    background-color: #fff3cd; /* Cor de fundo leve */
    border: 1px solid #ffeeba; /* Borda amarela clara */
    color: #856404; /* Texto em um tom mais escuro */
    padding: 15px;
    border-radius: 5px;
    margin: 10px 0; /* Margem superior e inferior */
    animation: none; /* Remove qualquer animação */
}
  .modal-content {
            background-color: #fefefe;
            margin: auto;
            padding: 20px;
            border: 1px solid #888;
            width: 90%; 
            max-width: 800px; 
            border-radius: 10px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
        }

        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }

        .close:hover,
        .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }


    </style>
    
    
</head>
<body>
    <div class="menu">
        <p class="premium-header">TERCEIRO</p>
        <a href="index.html" class="menu-item">Menu</a>
        <a href="cilia.html" class="menu-item">Cilia | edr </a>
        <a href="terceiro.html" class="menu-item">Terceiro</a>
    </div>
 
    <div class="section-container">
      
        <button class="button-onclick" onclick="toggleModal()">ABRA PRÉ ATENDIMENTO</button>
        
        <h2>Processo de Terceiros</h2>
        <div class="instructions">
            <h2>Processo de Tratamento de Sinistros</h2>
            <p>Todos os processos serão inicialmente tratados como acordo de valores. Caso o terceiro não aceite o acordo, a EDR irá indicar uma oficina Arval ao terceiro e enviar o orçamento no Cilia para sequência de aprovação pelo perito Arval.</p>
        
            <ol>
                <li><strong>Pré-atendimento:</strong> Aberto pelo SAC da forma tradicional.</li>
                <li><strong>Envio de Documentos:</strong> O terceiro envia os documentos.</li>
                <li><strong>Avaliação do Backoffice:</strong> 
                    O Backoffice avalia os documentos. Se estiverem “ok”, indica Cilia no Daytona, solicita lote, gera link na EDR, solicita análise de culpabilidade ao ponta de ilha, verifica se as fotos do carro Arval foram recebidas no Cilia ou por e-mail e orienta o terceiro, por e-mail, sobre o prazo inicial de tratativa da análise de culpabilidade.
                </li>
                <li><strong>Prazo para Análise:</strong> O prazo para análise de culpabilidade é de até 72 horas úteis (realizada pelo ponta de ilha). Após isso, podemos cobrar.</li>
                <li><strong>Análise da EDR:</strong> A EDR analisa a vistoria, monta o orçamento e estipula o valor.</li>
                <li><strong>Oferta de Acordo:</strong> A EDR oferta acordo ao terceiro (48 horas úteis para contato com o terceiro para proposta inicial de acordo).</li>
                <li><strong>Confirmação do Terceiro:</strong> O terceiro dá o "DE ACORDO".</li>
                <li><strong>Elaboração do Termo:</strong> A EDR elabora o termo e envia para o terceiro preencher e assinar.</li>
                <li><strong>Envio do Termo Assinado:</strong> Após receber o termo assinado, a EDR tem até 48 horas úteis para enviar à Laís.</li>
                <li><strong>Distribuição:</strong> Laís distribui ao ponta de ilha responsável.</li>
                <li><strong>Início das Tratativas:</strong> O ponta inicia as tratativas com o setor financeiro e, ao receber validação de pagamento, insere parecer no Cilia.</li>
            </ol>
        
            <p><strong>Observação:</strong> Todas as etapas do processo são inseridas no Cilia em “Pareceres”.</p>
        
        
     <div class="content">

      <h3>Processo de Lucros</h3>
  
      <p><strong>Quando o processo do terceiro está sendo tratado como Acordo de Valores pela EDR:</strong></p>
      <ul>
        <li>O Lucros Cessantes deve ser solicitado durante o período de negociação, antes de o terceiro assinar o acordo.</li>
        <li>A solicitação deve ser direcionada para a EDR, não para o Ponta de Ilha.</li>
      </ul>
  
      <p><strong>Quando a EDR trata o processo como Indicação de Oficina:</strong></p>
      <ul>
        <li>Se o reparo do veículo será realizado em uma oficina credenciada pela Arval, o Lucros Cessantes só pode ser solicitado após a conclusão do reparo.</li>
        <li>Neste caso, a solicitação deve ser direcionada ao Ponta de Ilha, responsável pela gestão do processo após o reparo.</li>
      </ul>
    </div>
  </div>
  
  <button class="button" id="openModal">Saiba como abrir um pré-atendimento no Daytona</button>

<!-- Tabela com Etapas, Responsáveis e Processos -->
<table>
    <thead>
        <tr>
            <th>Etapa</th>
            <th>Responsável</th>
            <th>Processo</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1</td>
            <td>Altio</td>
            <td>Abertura do Pré-atendimento<br>Solicitação de Documentos do Terceiro</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Altio</td>
            <td>Recepção dos documentos / Cobra documentos pendentes + Fotos do veículo Arval<br>
                Abertura do Sinistro<br>
                Preenche planilha terceiros para envio do lote<br>
                Indicação de oficina Cilia (todos os casos de terceiros)<br>
                Envia link da vistoria digital ao terceiro<br>
                Direciona o processo para Análise de culpabilidade (Pontas de ilha)</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Pontas de Ilha (Driv. Exp.)</td>
            <td>Realização da Análise de Culpabilidade<br>Incluir resultado e detalhes da Analise no Cilia</td>
        </tr>
        <tr>
            <td>4</td>
            <td>EDR</td>
            <td>Contato com o terceiro para proposta de acordo<br>
                Montagem do termo de acordo<br>
                Envio para assinatura do terceiro<br>
                Envio do termo para Arval programar o pagamento (SLA: 1 dia para envio do termo uma vez assinado)</td>
        </tr>
        <tr>
            <td>5</td>
            <td>Pontas de Ilha (Driv. Exp.)</td>
            <td>Recepção do termo assinado<br>Programação do pagamento no Daytona</td>
        </tr>
    </tbody>
</table>
<h3>Contatos EDR</h3>
    <table>
        <thead>
            <tr>
                <th>Nome</th>
                <th>Telefone</th>
                <th>E-mail</th>
                <th>Função</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Andrea Beneit</td>
                <td>11 94151-9864</td>
                <td>andrea.beneit@edr.com.br</td>
                <td>Analise Acordo Terceiro</td>
            </tr>
            <tr>
                <td>Luiza Tavares</td>
                <td>81 8107-3523</td>
                <td>luiza.tavares@edr.com.br</td>
                <td>Apoio Follow-up e Acordo Terceiros</td>
            </tr>
            <tr>
                <td>Wandson Santos</td>
                <td>19 97111-9562</td>
                <td>controle10@edr.com.br</td>
                <td>Agendamento Vistorias / Complementos</td>
            </tr>
            <tr>
                <td>Marcos Yuri</td>
                <td>81 7101-5654</td>
                <td>marcos.yuri@edr.com.br</td>
                <td>Follow-up</td>
            </tr>
            <tr>
                <td>Gabriel Dias</td>
                <td>51 9173-7528</td>
                <td>analistaonline13@edr.com.br</td>
                <td>Analise Técnica (SP/MG)</td>
            </tr>
            <tr>
                <td>Daniel</td>
                <td>19 99337-3580</td>
                <td>analistaonline2@edr.com.br</td>
                <td>Analise Técnica (Demais Estados)</td>
            </tr>
        </tbody>
    </table>
<div class="alert">
    Acompanhe o processo do Terceiro no Cília.

</div>
<strong><div class="alert"><span class="observacao">OBSERVAÇÃO:  </span></strong>caso o terceiro não aceite o acordo, a EDR irá indicar uma oficina Arval o terceiro, e enviar o orçamento no Cilia para sequência de aprovação pelo perito Arval.</div>

<div class="alert">
O processo do terceiro só irá seguir se o condutor Arval tiver encaminhado as fotos dos danos.
</div>
<h7>        <a href="https://app.inspections-management.com/login?token=bGlua2FydmFsOlBydHk0NTIzdFI=" class="btn-gere-vistoria" target="_blank">Gere a Vistoria Digital</a>
</h7>

<div id="modalPassoAPasso" class="modal">
    <div class="modal-content">
        <span class="close" id="closeModal">&times;</span>
        <h3>Passo a passo para abrir o evento para o primeiro atendimento ao terceiro:</h3>
        <ol>
            <li><strong>Vá para o CLAIMS.</strong></li>
            <li><strong>Clique em MODIFY.</strong></li>
            <li><strong>Vá para a guia de EVENTS & BALANCE.</strong></li>
            <li><strong>Clique em NOVO.</strong></li>
            <li><strong>Troque a natureza do evento de SINISTRO para RCF.</strong></li>
            <li><strong>Cole o código: F18348 (fornecedor Cilia).</strong></li>
            <li><strong>Vá para FOLLOW-UP.</strong></li>
            <li><strong>Cole os dados que você coletou com o condutor.</strong></li>
            <li><strong>Insira mais informações que achar necessário no follow-up.</strong></li>
            <li><strong>Dentro do Daytona, clique no botão EMAIL.</strong></li>
            <li><strong>Procure o email: ABERTURA PRÉ ATENDIMENTO TERCEIRO.</strong></li>
            <li><strong>Cole o email do condutor no campo "Para".</strong></li>
            <li><strong>Clique em enviar.</strong></li>
        </ol>
        <p>Pronto, chamado aberto ao terceiro.</p>
    </div>

</div>


            <!-- Tabela com código do fornecedor -->
            <table>
                <thead>
                    <tr>
                        <th>Fornecedor</th>
                        <th>F18348</th>
                    </tr>
                </thead>
                <tbody>
      
                </tbody>
            </table>
        </div>

        
        <div id="modalForm" class="modal">
            <div class="modal-content">
                <span class="close" onclick="toggleModal()">&times;</span>
                <div class="flex flex-col items-center justify-center h-screen dark">
                    <div class="w-full max-w-md bg-gray-800 rounded-lg shadow-md p-6">
                        <h2 class="text-2xl font-bold text-gray-200 mb-4">Dados do Terceiro</h2>
                        <form id="emailForm" onsubmit="submitForm(event)" class="flex flex-col">
                            <div class="form-group mb-4">
                                <input
                                    type="text"
                                    id="nome-terceiro"
                                    name="nome-terceiro"
                                    placeholder="Nome do terceiro"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                />
                            </div>
                            <div class="form-group mb-4">
                                <input
                                    type="email"
                                    id="email-terceiro"
                                    name="email-terceiro"
                                    placeholder="E-mail do terceiro"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                />
                            </div>
                            <div class="form-group mb-4">
                                <input
                                    type="text"
                                    id="telefone-terceiro"
                                    name="telefone-terceiro"
                                    placeholder="Telefone do terceiro"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                />
                            </div>
                            <div class="form-group mb-4">
                                <select
                                    id="tipo-terceiro"
                                    name="tipo-terceiro"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                >
                                <option value="CARRO">SELECIONE</option>
                                    <option value="CARRO">CARRO</option>
                                    <option value="MOTO">MOTO</option>
                                </select>
                            </div>
                            <div class="form-group mb-4">
                                <input
                                    type="text"
                                    id="placa"
                                    name="placa"
                                    placeholder="Placa do veículo"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                />

                            </div>
                            <div class="form-group mb-4">
                                <input
                                    type="text"
                                    id="marca"
                                    name="marca"
                                    placeholder="Marca do veículo"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                />

                               
                            </div>
                            <div class="form-group mb-4">
                                <input
                                    type="text"
                                    id="Modelo"
                                    name="Modelo"
                                    placeholder="Modelo"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                />

                               
                            </div>
                            <div class="form-group mb-4">
                                <input
                                    type="text"
                                    id="Cor"
                                    name="Cor"
                                    placeholder="Cor"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                />
                        </div>
                        <div class="form-group mb-4">
                            <input
                                type="text"
                                id="Ano"
                                name="Ano"
                                placeholder="Ano"
                                class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                            />
                    </div>
                            <div class="form-group mb-4">
                                <textarea
                                    id="danos"
                                    name="danos"
                                    placeholder="Descreva os danos"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                ></textarea>
                            </div>
                            <div class="form-group mb-4">
                                <textarea
                                    id="relato"
                                    name="relato"
                                    placeholder="Relato do ocorrido"
                                    class="bg-gray-700 text-gray-200 border-0 rounded-md p-2 focus:bg-gray-600 focus:outline-none focus:ring-1 focus:ring-blue-500 transition ease-in-out duration-150"
                                ></textarea>
                            </div>
                            <div class="form-group flex space-x-4 mb-4">
                                <button
                                    type="button"
                                    onclick="copiarDados()"
                                    class="bg-gradient-to-r from-indigo-500 to-blue-500 text-white font-bold py-2 px-4 rounded-md hover:bg-indigo-600 hover:to-blue-600 transition ease-in-out duration-150"
                                >
                                    Copiar
                                </button>
                                <button
                                    type="reset"
                                    class="clear-button bg-gray-600 text-gray-200 border-0 rounded-md p-2 hover:bg-gray-500 transition ease-in-out duration-150"
                                >
                                    Apagar
                                </button>
                            </div>
                        
                        </form>
                    </div>
                </div>
            </div>
        </div>
        
        <script>
            function copiarDados() {
                var formData = [
                    'Nome do Terceiro: ' + document.getElementById('nome-terceiro').value,
                    'E-mail: ' + document.getElementById('email-terceiro').value,
                    'Telefone: ' + document.getElementById('telefone-terceiro').value,
                    'Tipo de Terceiro: ' + document.getElementById('tipo-terceiro').value,
                    'Placa: ' + document.getElementById('placa').value,
                    'Marca: ' + document.getElementById('marca').value,
                    'Danos: ' + document.getElementById('danos').value,
                    'Relato do Ocorrido: ' + document.getElementById('relato').value
                ].join('\n');
                navigator.clipboard.writeText('*** ABERTURA PRÉ ATENDIMENTO TERCEIRO - SN ***\n' + formData);
                alert('Dados copiados, inclua no Daytona e não esqueça de colocar o número do SN !');
            }
            
            function toggleModal() {
                var modal = document.getElementById("modalForm");
                if (modal.style.display === "none" || modal.style.display === "") {
                    modal.style.display = "block";
                } else {
                    modal.style.display = "none";
                }
            }
            
            function submitForm(event) {
                event.preventDefault();
                alert("Formulário enviado!");
                document.getElementById("modalForm").style.display = "none";
            }
    
            // Modal Passo a Passo
            var modalPassoAPasso = document.getElementById("modalPassoAPasso");
            var btnOpenModal = document.getElementById("openModal");
            var btnCloseModal = document.getElementById("closeModal");
    
            btnOpenModal.onclick = function() {
                modalPassoAPasso.style.display = "block";
            }
    
            btnCloseModal.onclick = function() {
                modalPassoAPasso.style.display = "none";
            }
    
            // Modal do Formulário
            var modalForm = document.getElementById("modalForm");
            var btnCloseModal2 = document.getElementById("closeModal2");
    
            btnCloseModal2.onclick = function() {
                modalForm.style.display = "none";
            }
    
            window.onclick = function(event) {
                if (event.target === modalPassoAPasso) {
                    modalPassoAPasso.style.display = "none";
                } else if (event.target === modalForm) {
                    modalForm.style.display = "none";
                }
            }
        </script>
    </body>
    </html>
