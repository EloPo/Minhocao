<template>
  <div class="regulamento">
    <v-layout fill-height justify-center align-center pa-5>
      <v-card width="80%" height="100%">
        <v-card-title>
          <v-layout justify-start align-center>
            <v-btn
              icon
              title="Voltar"
              @click="voltarPagina($event)"
            >
              <v-icon large>
                keyboard_backspace
              </v-icon>
            </v-btn>
          </v-layout>
        </v-card-title>
        <v-card-text class="content">
          <v-layout ml-5 mr-5 justify-center align-start column>
            <h1 class="regulamento-texto-titulo">
              Sobre o Jogo MinhocãoII com temáticas para o escape Game
            </h1>
            <br>
            <p>•	Um grupo será trancado em uma sala e terá um tempo determinado para encontrar a solução de sua saída.</p>
            <p>•	Nesta sala o grupo deve usar sua intuição, inteligência e habilidades, trabalhando em grupo para poder sair da sala.</p>
            <p>•	Para chegar à solução final o grupo deverá usar suas habilidades para decifrar uma serie de enigmas, códigos e puzzles.</p>
            <p>•	Os jogos são denominados “casos clínicos baseados em filmes e livros” e cada uma delas apresenta uma história e uma sala temática.</p>
            <p>•  Os jogos são projetados para serem uma experiência de entretenimento, desafio intelectual e também como uma ferramenta de desenvolvimento humano.</p>
            <h1 class="regulamento-texto-titulo">
              Sobre os Jogadores
            </h1>
            <br>
            <p>•	Jogadores de todas as idades são bem-vindos, porém menores de 18 anos devem estar acompanhados pelos pais ou responsável autorizado.</p>
            <p>•	Os jogadores deverão ser alunos presenciais da Unicesumar Campus Maringá.</p>
            <h1 class="regulamento-texto-titulo">
              Sobre as Sessões
            </h1>
            <br>
            <p>•	A ocupação da sala fica disponível até completar o seu máximo de jogadores. Você poderá jogar com desconhecidos e fazer novas amizades.</p>
            <br>
            <h1 class="regulamento-texto-titulo">
              Como Funciona
            </h1>
            <br>
            <p>•	Os jogadores deverão chegar com 15 minutos de antecedência ao horário agendado para receber as instruções sobre cada aventura e assinar o termo de compromisso.</p>
            <p>•	Os jogadores devem deixar seus pertences (bolsa, celular, câmera fotográfica e de vídeo) em um armário com chave, antes de entrar na sala. É proibido tirar fotografias, filmar no interior das salas e usar ajuda externa além daquela proporcionada pelo jogo.</p>
            <p>•	Assim que os jogadores entram na sala, inicia a contagem do tempo de 30, 15 ou 10 minutos, o qual pode ser visualizado em um tablet na sala.</p>
            <p>•	Os jogos são monitorados, pelos monitores do Minhocão II para acompanhar as ações dos jogadores, de forma a lhes ajudar com alguma necessidade ou em casos de emergência.</p>
            <p>•	Os monitores do Minhocão II e jogadores podem se comunicar caso for necessário.</p>
            <p>•	Após saírem da aventura, é tirada uma foto dos jogadores, a qual é publicada nas redes sociais.</p>
            <h1 class="regulamento-texto-titulo">
              Como Adquirir
            </h1>
            <br>
            <p>•	Os participantes devem adquirir ingressos através do site. Durante a inscrição no site, deve-se escolher a aventura que deseja jogar (respeitando o número mínimo e máximo de participantes).</p>
            <h1 class="regulamento-texto-titulo">
              Regras Gerais
            </h1>
            <br>
            <p>•	Não é permitido entrar com bebidas e alimentos nas salas das aventuras.</p>
            <p>•	Não quebrar nenhum objeto das salas.</p>
            <p>•	É proibido subir nos móveis das salas.</p>
            <p>•	É proibido mover móveis pesados.</p>
            <p>•	É proibido deixar marcas, dobras ou riscos nos objetos da sala.</p>
            <p>•	É proibido levar objetos da sala.</p>
            <p>•	Respeitar as indicações de “não tocar” e “não subir” coladas em alguns objetos da sala.</p>
            <br>
            <h1 class="regulamento-texto-titulo">
              Organização Geral
            </h1>
            <br>
            <p>Docente: Profª Cláudia Pinheiro</p>
            <br>
            <h1 class="regulamento-texto-titulo">
              Organização Temática
            </h1>
            <br>
            <p>Profª Waldecy Leonel</p>
            <p>Profª Roberta Leonel</p>
            <p>Profª Graziella Batista Silva</p>
            <p>Graduando: Anderson Assumpção</p>
            <br>
            <h1 class="regulamento-texto-titulo">
              Organização Técnica 
            </h1>
            <br>
            <p>Prof. Marcello Bonfim</p>
            <p>Prof. Arthur Zavadski</p>
            <p>Prof. Aparecido Vilela Junior</p>
            <p>Graduandos: Eloisa Potrich e Bruno Arruda</p>
            <br>
            <h1 class="regulamento-texto-titulo">
              Coordenação de Sala
            </h1>
            <br>
            <p>Profª Alexandra Perdigão – Nutrição</p>
            <p>Profª Carolina Semiguen – Fonoaudiologia</p>
            <p>Profª Graziella Batista Silva – Educação Física</p>
            <p>Profª Lilian Capellari – Odontologia, Enfermagem e Psicologia</p>
            <p>Profª Marcia Benedeti – Fisioterapia</p>
            <p>Profª Ana lucia de sa yamazaki - Fisioterapia</p>
            <p>Profª Patrícia Sandri – Nutrição</p>
            <p>Profª Sandra Pierini – Psicologia e Fisioterapia</p>
            <p>Profª Taísa Valques Lorencete - Biomedicina e Medicina</p>
          </v-layout>
        </v-card-text>
      </v-card>
    </v-layout>
  </div>
</template>

<script>
export default {
  name: 'Regulamento',
  methods: {
    voltarPagina() {
      this.$router.go(-1);
    },
  },
};
</script>

<style>
.regulamento {
  height: 100vh;
}

.regulamento-texto-titulo {
  font-size: 24px;
  font-style: italic;
}

.tabela-titulo{
  font-size: 18px;
  font-weight: 900;
}

p {
  font-size: 18px;
}

td {
  padding-right: 20px;
}

.content {
  height: 80%;
  overflow: auto;
}
</style>
