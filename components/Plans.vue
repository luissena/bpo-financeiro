<template>
  <section class="flex flex-col items-center">
    <h1 class="text-lg font-bold mt-24 pb-2 text-center">
      ESCOLHA O PLANO QUE MAIS SE ADEQUA A SUA EMPRESA
    </h1>
    <div class="border-t-2 border-[#7D3246] w-[200px]"></div>

    <div class="grid grid-cols-3 items-center justify-center gap-5 w-4/5 py-10">
      <ul
        class="z-50 py-5 px-5 bg-[#E4E4E4] rounded-ss-2xl rounded-ee-2xl"
        v-for="plan in plans"
      >
        <li class="text-[#7D3246] font-bold text-center mb-2">
          PLANO {{ plan.name }}
        </li>
        <li class="flex gap-2 items-center" v-for="feature in plan.features">
          <IconV class="w-3 h-3" />
          {{ feature }}
        </li>
        <li
          class="flex gap-2 items-center text-[#21515D80]"
          v-for="exclude in plan.excludes"
        >
          <IconX class="w-3 h-3" />
          {{ exclude }}
        </li>
      </ul>
    </div>
    <img class="w-1/4" id="globo" src="/globo.png" />
  </section>
</template>

<script setup lang="ts">
const plans = [
  {
    name: "BASIC",
    features: [
      "Implantação do serviço;",
      "Treinamento Administrativo;",
      "Gestão de Contas a Receber e a Pagar;",
      "Gestão Documental;",
      "Controle Financeiro;",
      "Agendamento Bancário;",
      "Conciliação Bancária e de Caixa;",
      "Auditoria das operadoras de cartões;",
      " Relatório de Fluxo de Caixa;",
      "Painel de métricas e resultados;",
      "Assessoria de Especialistas;",
    ],
    excludes: [
      "Emissão e envio de Notas Fiscais;",
      "Emissão e envio de Boletos Bancários;",
      "Painel de Indicadores em Dashboards;",
      "Vídeo explicativo do Resultado Financeiro Mensal;",
      "Consultoria Estratégica Mensal;",
      "Planejamento Orçamentário;",
      "Power Bl de Gestão Financeira",
    ],
  },
  {
    name: "PREMIUM",
    features: [
      "Implantação do serviço;",
      "Treinamento Administrativo;",
      "Gestão de Contas a Receber e a Pagar;",
      "Gestão Documental;",
      "Controle Financeiro;",
      "Agendamento Bancário;",
      "Conciliação Bancária e de Caixa;",
      "Auditoria das operadoras de cartões;",
      " Relatório de Fluxo de Caixa;",
      "Painel de métricas e resultados;",
      "Assessoria de Especialistas;",
      "Emissão e envio de Notas Fiscais;",
      "Emissão e envio de Boletos Bancários;",
      "Painel de Indicadores em Dashboards;",
      "Vídeo explicativo do Resultado Financeiro Mensal;",
    ],
    excludes: [
      "Consultoria Estratégica Mensal;",
      "Planejamento Orçamentário;",
      "Power Bl de Gestão Financeira",
    ],
  },
  {
    name: "BLACK",
    features: [
      "Implantação do serviço;",
      "Treinamento Administrativo;",
      "Gestão de Contas a Receber e a Pagar;",
      "Gestão Documental;",
      "Controle Financeiro;",
      "Agendamento Bancário;",
      "Conciliação Bancária e de Caixa;",
      "Auditoria das operadoras de cartões;",
      " Relatório de Fluxo de Caixa;",
      "Painel de métricas e resultados;",
      "Assessoria de Especialistas;",
      "Emissão e envio de Notas Fiscais;",
      "Emissão e envio de Boletos Bancários;",
      "Painel de Indicadores em Dashboards;",
      "Vídeo explicativo do Resultado Financeiro Mensal;",
      "Consultoria Estratégica Mensal;",
      "Planejamento Orçamentário;",
      "Power Bl de Gestão Financeira",
    ],
    excludes: [],
  },
]
</script>

<style scoped>
#globo {
  position: absolute;
  top: 6000px;
  right: 0;

  object-fit: cover;
}
</style>
