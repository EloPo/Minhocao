<template>
  <div class="detalhes">
    <v-layout fill-height column>
      <v-flex fill-height xs6>
        <v-card width="100%" height="30vh" class="elevation-0">
          <v-layout fill-height>
            <v-img :src="detalhes.imagem"></v-img>
          </v-layout>
        </v-card>
      </v-flex>
      <v-layout fill-height pl-4 pb-4 pr-4 pt-3 column>
        <v-layout row>
          <v-flex xs12>
            <span class="sala-titulo">{{ detalhes.titulo }}</span>
          </v-flex>
        </v-layout>
        <v-layout fill-height>
          <v-flex xs12>
            <v-layout pa-3 justify-start align-center>
              <p class="sala-descricao">{{ detalhes.descricao }}</p>
            </v-layout>
          </v-flex>
        </v-layout>
        <v-layout row justify-center align-center fill-height>
          <v-flex xs12>
            <v-layout justify-center align-center>
              <button class="botao" @click="irParaFormulario(detalhes.id)">
                <span class="botao-texto">Inscrição</span>
              </button>
            </v-layout>
          </v-flex>
        </v-layout>
      </v-layout>
    </v-layout>
  </div>
</template>

<script>
import Vampiro from '@/assets/vampiro.jpg';
import Crossfit from '@/assets/crossfit.jpg';
import Terry from '@/assets/terry.png';
import Ossos from '@/assets/ossos.jpg';
import Abigail from '@/assets/abigail.jpg';
import Bipolar from '@/assets/bipolar.png';
import Pegada from '@/assets/pegada.jpg';
import Ventriculo from '@/assets/ventriculo.jpg';
import Possessao from '@/assets/possessao.png';
import Pescoco from '@/assets/pescoco.jpg';
import Aglomerado from '@/assets/aglomerado.jpg';
import Botos from '@/assets/botos.jpg';

export default {
  name: 'Detalhes',
  data() {
    return {
      detalhes: {},
      links: [
        'https://forms.gle/6zNvgTwV9ehacgsa8',
        'https://forms.gle/acb44X3oasP7WsP79',
        'https://forms.gle/JcufJYq9CpFPzcss5',
        'https://forms.gle/rsLXikTsFVfdj2y58',
        'https://forms.gle/fmnpRqR4KFkWCrBf9',
        'https://forms.gle/UxN9Uwfa13F79FRCA',
        'https://forms.gle/yahb78Mp1kn4cmCD8',
        'https://forms.gle/tQ6bjV4uxKG3MCAY6',
        'https://forms.gle/krA799L9AfKUCd5F7',
        'https://forms.gle/xbN17SoF4vUK3qZ66',
        'https://forms.gle/nZ5TwtQf3ZTubCRB7',
        'https://forms.gle/F7pKD3CJAshBTX3v5',
      ],
      salas: [
				{
					id: 1,
					imagem: Vampiro,
					titulo: 'Cidade dos ossos - O Vale das sombras | 1º Ano Educa Matutino',
					card: 'Cidade dos ossos - O Vale das sombras',
					descricao: 'Simon leva uma vida monótona com sua amiga Clary, que desaparece no dia do seu 18º Aniversário, o que o faz entrar em depressão. Sozinho Simon, se encontra frente a um mistério que terá de desvendar para encontrar sua amiga e para isso terá de juntar todas as pistas possíveis. Mas durante esta busca algo aparece em seu caminho, seres sombrios que ameaçam sua vida, para ser mais claro “Vampiros”. Simon começa a ser terrivelmente perseguido e atacado, porém depois de horas consegui despista-los e escapa com vida, mas, ele não é mais o mesmo, pois sem que percebesse foi mordido durante um duelo. Ele se tornou mais forte, mais resistente, porém descontrolado. Controlar sua sede de sangue era impossível para um iniciante, mas Simon não quer machucar ninguém, então ele decide ficar em uma dieta de sangue animal. Mas o sangue animal não fornece os mesmos nutrientes de uma alimentação regrada a sangue humano aos vampiros, causando uma alimentação desregrada para Simon, afetando assim seu desenvolvimento de tecidos corporais, força, controle mental e produção de energia o que comprometerá sua saúde. Mediante a todas essas mudanças e acontecimentos, conseguirá Simon ainda encontra sua amida de infância?',
					limite: 6,
					tempo: 30,
				},
				{
					id: 2,
					imagem: Crossfit,
					titulo: 'Quebrando as Regras com Crosfit 1º Ano “B” Noturno Educa',
					card: 'Quebrando as Regras com Crossfit',
					descricao: 'Seu nome é Jack. Tenho um passado um tanto conturbado. Há um mês me envolvi em uma briga feia no qual foi registrada por câmeras e celulares. Agora quero revanche. Para isso procurei um mestre que com técnicas de crosfit e uma suplementação adequada me ensinou a moldar as minhas habilidades. É hora da revanche! Sua equipe consegue escapar em 30 minutos? Então descubra. Quais foram os suplementos que usei? E as principais atividades do crosfit que aprendi ao longo desses 30 dias. As pistas estão espalhadas por toda sala!',
					limite: 6,
					tempo: 30,
				},
				{
					id: 3,
					imagem: Terry,
					titulo: 'O Universo Físico de Terry Crews 1º Ano “A” Noturno Educa',
					card: 'O Universo Físico de Terry Crews',
					descricao: 'Terry Crews( Terrence Alan Crews) com 50 anos nascido em 30 de julho de 1968 em Flint, Michigan depois de ganhar o seu diploma do ensino médio na Flint Southwestern Academy, ele recebeu uma bolsa de estudos no prestigiado Center for the Arts em Michigan seguido por uma bolsa na Art Excellence scholarship, e logo após ganhou uma bolsa de estudos integral, para futebol americano Western Michigan University. Atuou em filmes como A Mais Louca Sexta-feira em Apuros, Malibu&#39;s Most Wanted, Starsky &amp; Hutch, Um Voo Muito Louco, As Branquelas, Click, Os Mercenários e Todo Mundo em Pânico 5. Ganhou destaque por interpretar Julius Rock no seriado estadunidense Todo Mundo Odeia o Chris. Entre outros trabalhos. Artista, ex Jogador de futebol americano, dançarino, comediante, dublador, escritor entre outras funções. Onde arrumar tanta energia e vigor? Será que apenas malhando? Vamos juntos desvendar esse mistério.',
					limite: 6,
					tempo: 30,
				},
				{
					id: 4,
					imagem: Ossos,
					titulo: 'O vagão de ossos 1º Fisioterapia Matutino',
					card: 'O vagão de ossos',
					descricao: 'No século XX e forma mais comum de transporte entre cidades, eram através da rodovia de ferro, pensando nisso, uma empresa criou um vagão para o transporte de cadáveres. O vagão de madeira servia como funeral, em sua totalidade, como um lugar para velas e toda a família do morto, propulsionando assim a oportunidade de velar o corpo durante a viagem. Hoje em dia, este vagão fica aberto para visitação.',
					limite: 6,
					tempo: 30,
				},
				{
					id: 5,
					imagem: Abigail,
					titulo: 'Área 51 – Projeto Abigail Western 1º Ano Fonoaudiologia e Fisioterapia Noturno',
					card: 'Área 51 – Projeto Abigail Western',
					descricao: 'Em 1943, um cientista chamado Albert Western trabalhava para o exército americano em uma base militar secreta denominada ÁREA 51. Albert era obcecado em desenvolver o soldado perfeito. Sem sucesso ao solicitar voluntários para o experimento, decidiu que a pessoa certa para esse trabalho seria sua própria filha, a qual apresentava paralisia cerebral, mediante a isso deu inicio ao projeto Abigail. Porém os experimentos propostos por Albert não deram certo, resultado em um grande fracasso, sua filha tornou-se uma aberração. Com isso Abert comete suicídio, deixando uma carta aos seus colegas, implorando para que a salvasse. O que estará escrito nessa carta? Qual a formula para poder salva-la? Venha e aventure-se nesta descoberta.',
					limite: 6,
					tempo: 30,
				},
				{
					id: 6,
					imagem: Bipolar,
					titulo: 'Jim Carrey - 8/80, "Não sou bipolar, eu sou?" | 1º Psicologia Matutino',
					card: 'Jim Carrey - 8/80, "Não sou bipolar, eu sou?"',
					descricao: 'O Ator Jim Carrey interpretou diversos filmes de comédia que tiraram de nós boas gargalhadas. Os diversos personagens representados caracterizam aspectos de uma pessoa com Transtorno Bipolar. Não somente nas telas, o ator também demonstra o distúrbio em sua vida particular. No Escape Game, você será desafiado descobrir os enigmas na sala da Bipolaridade representada por alguns filmes.',
					limite: 6,
					tempo: 30,
				},
				{
					id: 7,
					imagem: Pegada,
					titulo: 'A Equação 1º Psicologia Noturno',
					card: 'A Equação',
					descricao: 'Paulo Martins foi diagnosticado com esquizofrênico aos 25 anos, e atualmente com os seus 35 anos foi reabilitado em viver em sociedade. Recentemente, recebeu uma missão de extrema urgência, que caso não seja comprida, que pode resultar na destruição do Brasil. Como se isso não fosse problemático o suficiente, constantemente é perturbado por familiares cegos ao perigo eminente e espiões comunistas de médicos e psicólogos que alegam que Paulo enlouqueceu de vez. Siga o gênio Paulo em sua cruzada a fim de encontrar a resposta da pesquisa que o mesmo escondeu em seu quarto antes de ser capturado.',
					limite: 6,
					tempo: 30,
				},
				{
					id: 8,
					imagem: Ventriculo,
					titulo: 'It Ventriculos 1º Ano Nutrição Matutino',
					card: 'It Ventriculos',
					descricao: 'It foi consultar um endocrinologista para perder peso. O endocrinologista o encaminhou ao Gastro para uma possível avaliação de cirurgia bariátrica. Ele conheceu todas as condições para a cirurgia, assim como os riscos da mesma. Quando avaliou os malefícios, It resolveu consultar a Nutricionista.',
					limite: 6,
					tempo: 30,
				},
				{
					id: 9,
					imagem: Possessao,
					titulo: 'A Possessão Medicina',
					card: 'A Possessão',
					descricao: 'Gritos pela casa, comportamentos estranhos, pais desesperados. Sejam Bem Vindos a Casa de Emily Rose. No Inverno de 1976, era tudo que se comentava na pequena e religiosa cidade no interior do RS. Sem hospitais próximos, a atitude dos pais foi chamar por socorro divino. Você será capaz de ajuda-la?',
					limite: 6,
					tempo: 30,
				},
				{
					id: 10,
					imagem: Pescoco,
					titulo: 'O corpo fala Biomedicina Matutino/Noturno',
					card: 'O corpo fala',
					descricao: 'O ano de 1995 foi marcado por uma onda de assassinatos cruéis em Portlonal. O modo operante ao serial killer será sempre o mesmo: mulheres tinham toda a sua pele removida e após um doloroso procedimento cirúrgico, sempre o mesmo osso era retirado de seus corpos. A identidade do assassino em série nunca foi descoberta, mas depois de 24 anos, uma nova onda de assassinatos com a mesma característica volta a assombrar a população. Agora a situação é diferente, o perito biomédico, com a utilização dos perfis genéticos, radiografia forense e impressão digital, promete solucionar este caso. Porém, em certo dia, o biomédico acorda em um local desconhecido ao lado de um corpo e esse fato promete mudar o mundo desse caso. Quem é a vítima? Onde o perito está? Quem será o assassino?',
					limite: 6,
					tempo: 30,
				},
				{
					id: 11,
					imagem: Aglomerado,
					titulo: 'Aglomerados 1º Enfermagem Noturno',
					card: 'Aglomerados',
					descricao: 'Uma festa organizada por estudantes de pedagogia, agronomia, medicina veterinária e zootecnia de uma universidade do Rio Grande do Sul acabou em tragédia, após um incêndio na boate que deixou 242 mortos 680 feridos. O desastre foi provocado pela imprudência e pelas más condições do local. As vítimas foram admitidas nos hospitais por lesões de queimaduras grave. Venha desvendar os mistério por trás das Queimaduras.',
					limite: 6,
					tempo: 30,
				},
				{
					id: 12,
					imagem: Botos,
					titulo: 'Botox Mortais 1º Odontologia Matutino',
					card: 'Botox Mortais',
					descricao: 'Um acadêmico de odontologia ao estudar sobre procedimentos estéticos fica deslumbrado pela área, sua fascinação o leva a uma prática destes procedimentos de forma obsessiva. Ele utiliza de seu poder de convencimento para atrair pessoas e leva-las até sua casa, local onde ele tem a oportunidade de tornar as mesmas vulneráveis. Esse vício o faz agressivo, contudo impõe regras para as aflitas pessoas captadas em sua discrepante armadilha. Para elas serem libertadas terão que passar por algumas etapas de seu sanguinário jogo!',
					limite: 6,
					tempo: 30,
				},
			],
    };
  },
  created() {
    const numeroDaSala = this.$route.params.id;
    this.escolherSala(numeroDaSala);
  },
  methods: {
    escolherSala(numeroDaSala) {
      this.detalhes = this.salas[numeroDaSala-1];
    },
    irParaFormulario(sala) {
      const linkCurto = this.links[sala-1];
      window.open(linkCurto);
    },
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Roboto&display=swap');

.detalhes{
  height: 100vh;
  font-family: 'Roboto', sans-serif;
  font-style: normal;
  font-weight: 500;
  color: #000000;
}

.sala-titulo {
  font-size: 3vh;
}

.sala-descricao {
  font-size: 2vh;
}

.botao {
  width: 50vh;
  height: 10vh;
  background-color: black;
  border-radius: 5px;
  border: 1px solid black;
}

.botao-texto {
  font-size: 2.5vh;
  color: white;
}
</style>
