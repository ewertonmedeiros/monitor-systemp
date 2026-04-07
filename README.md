# 🚂 Monitor Temperaturas Systemp - CCO | Malha Sul

Um painel web meteorológico desenvolvido especificamente para o Centro de Controle Operacional (CCO) monitorar as condições térmicas e climáticas ao longo da Malha Sul. O sistema foca na prevenção de riscos operacionais ferroviários/logísticos, gerando alertas visuais automáticos para condições extremas.

🔗 **[Acessar o Painel Ao Vivo](https://ewertonmedeiros.github.io/monitor-systemp/)**

---

## 🎯 Principais Funcionalidades

* **🚨 Monitor de Alertas Inteligente:** Tela inicial que filtra e exibe apenas as cidades com risco iminente, otimizando a tomada de decisão do operador.
* **🌡️ Riscos Térmicos:** Alertas automáticos para Calor Extremo (> 29ºC, risco de dilatação de trilhos) e Frio Extremo/Geada (< 5ºC).
* **💨 Alertas de Vendaval:** Monitoramento de rajadas de vento, sinalizando perigo de queda de árvores ou problemas na rede aérea quando os ventos ultrapassam 60 km/h.
* **🌩️ Alertas de Chuva Severa:** Identificação de tempestades através de códigos meteorológicos WMO.
* **📈 Gráficos de Evolução Térmica:** Integração com Chart.js para visualização da curva de temperatura nas próximas 24 horas, incluindo marcações de faixas de risco (backgrounds coloridos no gráfico) e períodos de chuva.
* **📅 Previsão Estendida:** Navegação rápida entre o dia atual (Hoje), o dia seguinte (D+1) e o posterior (D+2).
* **📥 Relatórios em PDF:** Exportação do painel atualizado com um clique, formatado perfeitamente para envio por e-mail ou impressão.

---

## 🛠️ Tecnologias Utilizadas

O painel foi construído de forma leve e responsiva (Mobile-First), sem a necessidade de frameworks pesados, garantindo carregamento rápido em qualquer máquina do CCO.

* **HTML5, CSS3 & JavaScript (ES6+)** - Estrutura, estilização e lógica nativa.
* **[Open-Meteo API](https://open-meteo.com/)** - Fornecimento gratuito e confiável de dados de previsão do tempo e rajadas de vento baseados em modelos globais.
* **[Chart.js](https://www.chartjs.org/)** - Renderização dos gráficos de evolução térmica.
* **[html2pdf.js](https://ekoopmans.github.io/html2pdf.js/)** - Geração de relatórios PDF *client-side*.

---

## ⚙️ Como Rodar Localmente (Desenvolvimento)

Caso queira fazer alterações no código ou testar localmente na sua máquina, siga os passos abaixo. 

*Nota: Não é possível abrir o arquivo `index.html` com duplo clique direto (via `file:///`) devido às políticas de segurança de CORS dos navegadores com a API.*

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/EwertonMedeiros/monitor-systemp.git](https://github.com/EwertonMedeiros/monitor-systemp.git)
