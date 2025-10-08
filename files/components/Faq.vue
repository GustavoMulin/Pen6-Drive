<template>
  <section class="faq-one">
    <!-- <img src="/assets/images/shapes/faq-bg-1-1.png" class="faq-one__bg-shape-1" alt=""> -->

    <div class="container">
      <div class="block-title text-center">
        <h3><span>Perguntas</span> Frequentes</h3>
      </div><!-- /.block-title -->
      <div class="accrodion-grp wow fadeIn" data-wow-duration="1500ms" data-grp-name="faq-accrodion">
        <div class="row">

          <div class="col-lg-6">
            <div class="accordion-container-one">
              <div class="ac">
                <h2 class="ac-q accordion__title-text" tabIndex="0">Para quem é o P6.App?</h2>
                <div class="ac-a accordion__content">
                  <p class="accordion__content-desc">O P6.App é ideal para agências de publicidade que buscam mais agilidade, organização e controle em seus processos. Seja você freelancer, parte de uma pequena agência ou de uma equipe maior, a plataforma foi desenvolvida para facilitar o seu dia a dia, do briefing ao relatório final.
                  </p>
                </div>
              </div>

              <div class="ac accordion__content">
                <h2 class="ac-q accordion__title-text" tabIndex="0">A plataforma é fácil de usar? Vocês oferecem suporte?</h2>
                <div class="ac-a">
                  <p class="accordion__content-desc">Sim! O P6.App foi pensado para ser intuitivo e simples de usar, mesmo por quem não tem familiaridade com ferramentas digitais. E se você precisar de ajuda, oferecemos suporte rápido via chat, e-mail ou WhatsApp.
                  </p>
                </div>
              </div>

              <div class="ac">
                <h2 class="ac-q accordion__title-text" tabIndex="0">Os dados da minha agência e dos clientes estão seguros dentro da plataforma?</h2>
                <div class="ac-a accordion__content">
                  <p class="accordion__content-desc">Totalmente. Utilizamos criptografia, backups automáticos e seguimos boas práticas de proteção de dados para garantir que todas as informações da sua agência e dos seus clientes estejam protegidas e acessíveis apenas por quem você autorizar.
                  </p>
                </div>
              </div>
              <div class="ac">
                <h2 class="ac-q accordion__title-text" tabIndex="0">Quais são as formas de pagamento?</h2>
                <div class="ac-a accordion__content">
                  <p class="accordion__content-desc">Aceitamos pagamentos via cartão de crédito, Pix e boleto bancário. Você pode escolher a opção que for mais conveniente para a sua agência. Também oferecemos planos mensais e anuais com desconto progressivo.
                  </p>
                </div>
              </div>

            </div>
          </div>

          <div class="col-lg-6">
            <div class="accordion-container-two">
              <div class="ac">
                <h2 class="ac-q accordion__title-text" tabIndex="0">Ainda tenho dúvidas, como faço?</h2>
                <div class="ac-a accordion__content">
                  <p class="accordion__content-desc">A gente sabe que cada agência tem sua realidade e às vezes surgem dúvidas que só uma boa conversa resolve. Por isso, nosso time está à disposição pra te ajudar:
                  Você pode falar com a gente pelo WhatsApp (69) xxxxx-xxxx enviar um e-mail para contato@pen6app ou usar o chat direto dentro da plataforma.
                  </p>
                </div>
              </div>

              <div class="ac accordion__content">
                <h2 class="ac-q accordion__title-text" tabIndex="0">Preciso instalar algo para usar o P6.App?</h2>
                <div class="ac-a">
                  <p class="accordion__content-desc">Não! O P6.App é 100% online e funciona direto do seu navegador, em qualquer dispositivo. Basta acessar com seu login e senha — sem complicações, instalações ou atualizações manuais.
                  </p>
                </div>
              </div>

              <div class="ac">
                <h2 class="ac-q accordion__title-text" tabIndex="0">Consigo adicionar minha equipe para trabalhar junto comigo?</h2>
                <div class="ac-a accordion__content">
                  <p class="accordion__content-desc">Sim! Você pode adicionar membros da sua equipe, definir permissões e acompanhar o andamento das tarefas em tempo real. O P6.App foi pensado para facilitar o trabalho colaborativo e centralizar tudo em um só lugar.
                  </p>
                </div>
              </div>
              <div class="ac">
                <h2 class="ac-q accordion__title-text" tabIndex="0">O P6.App oferece algum período de teste gratuito?</h2>
                <div class="ac-a accordion__content">
                  <p class="accordion__content-desc">Sim, oferecemos um período de teste gratuito para você explorar todas as funcionalidades da plataforma antes de contratar um plano. Assim, você testa na prática e vê como o Pen6App pode transformar a rotina da sua agência.
                  </p>
                </div>
              </div>

            </div>
          </div>

        </div>

      </div>
    </div><!-- /.container -->
  </section>
</template>

<script>
    export default {
      name: "Faq",
      mounted() {
        new Accordion('.accordion-container-one');
        new Accordion('.accordion-container-two');
      }
    }
</script>

<style scoped>
  .ac {
    margin-top: 10px;
    padding: 10px;
    background: #F4F0F9;
    box-sizing: border-box;
  }

  .ac>.ac-q {
    font: bold 15px Arial, sans-serif;
    font-size: 20px;
    color: #444;
    padding: 10px 30px 10px 10px;
    margin: 0;
    text-decoration: none;
    display: block;
    cursor: pointer;
    position: relative;
    font-weight: 700;
  }

  .ac.is-active .ac-q {
    color: #3f1473 !important;
  }
  .ac>.ac-q::after {
    content: '+';
    text-align: center;
    width: 15px;
    right: 10px;
    top: 50%;
    -webkit-transform: translate(0, -50%);
    transform: translate(0, -50%);
    position: absolute
  }

  .ac>.ac-a {
    overflow: hidden;
    -webkit-transition-property: all;
    transition-property: all;
    -webkit-transition-timing-function: ease;
    transition-timing-function: ease
  }

  .ac>.ac-a p {
    font: 16px/1.5 Arial, sans-serif;
    color: #8b7f9a;
    margin: 0;
    padding: 10px;
    font-size: 18px;
    font-weight: 600;
  }

  .ac.js-enabled>.ac-a {
    visibility: hidden
  }

  .ac.is-active>.ac-a {
    visibility: visible
  }

  .ac.is-active>.ac-q::after {
    content: '\2013';
    color: #3f1473;
  }
</style>
