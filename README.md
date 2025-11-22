# 🐍 PosturAI-Python: O seu Assistente de Postura com Inteligência Artificial

## 💡 Sobre o Projeto
O **PosturAI-Python** é um projeto desenvolvido no âmbito da **FIAP Global Solution 2025** com o objetivo de combater os problemas de saúde relacionados à má postura durante longas jornadas de trabalho ou estudo.

Utilizando a visão computacional e modelos de *Machine Learning* para estimativa de pose, o PosturAI monitora em tempo real a postura do usuário através da webcam, fornecendo feedback imediato para correções. A má postura é um problema crescente na era do trabalho híbrido e remoto, e este projeto visa promover o bem-estar e a **ergonomia digital**.

---

## 👥 Autores

- **Ulisses Ribeiro - RM562230** — Desenvolvimento *core* e arquitetura técnica da solução em Visão Computacional.
- **Arthur Berlofa Bosi - RM564438** — Responsável pela integração IoT (ESP32) e pela gestão de configuração via arquivos JSON.
- **Arthur Ferreira - RM564958** - Responsavel pela organização das pastas, e planejamento do software.

---

## ✨ Recursos Principais
* **Detecção de Postura em Tempo Real:** Monitoramento contínuo usando a webcam.
* **Estimativa de Pose:** Utiliza bibliotecas avançadas (como MediaPipe ou OpenPose) para mapear pontos-chave do corpo (ombros, pescoço, orelha).
* **Feedback Visual e Sonoro:** Alertas discretos quando a postura ideal não é mantida por um período de tempo.
* **Alerta Tátil (Integração IoT):** Capacidade de enviar sinais para um microcontrolador (como **ESP32 ou Arduino**) para ativar dispositivos de feedback físico, como a **emissão de vibração** em acessórios vestíveis ou superfícies de contato, para um alerta discreto e imediato.
* **Perfis de Uso Customizáveis:** Utiliza o arquivo de configuração **`preferences.json`** para definir o nível de monitoramento desejado, como:
    * **Fraco (Low):** Baixa sensibilidade e maior tempo de tolerância para alertas.
    * **Moderado (Medium):** Configuração padrão e equilibrada.
    * **Forte (High):** Alta sensibilidade e resposta imediata a pequenos desvios posturais.
* **Análise Ergonômica:** Avaliação de métricas chave de postura, como o alinhamento da cabeça.
* **Relatório Postural:** Ao finalizar a sessão, gera um **gráfico detalhado que exibe seus desvios posturais** ao longo do tempo, ajudando a identificar padrões de fadiga e áreas que requerem mais atenção.

---

## 📊 Análise Pós-Sessão: Relatórios de Desvios
Após encerrar o monitoramento, o PosturAI processa os dados coletados para gerar um relatório visual. Este relatório utiliza gráficos para mostrar:

1.  **Métrica de Postura ao Longo do Tempo:** Um gráfico de linha que ilustra como sua postura variou durante a sessão.
2.  **Distribuição dos Desvios:** Um gráfico de barras ou pizza que quantifica o tempo gasto em cada categoria de má postura detectada (e.g., "Cabeça Inclinada", "Ombros Curvados", "Postura Correta").

Essa funcionalidade é crucial para fornecer um *feedback* tangível, permitindo que o usuário visualize e compreenda melhor seus hábitos posturais.

---

## 🛠️ Tecnologias Utilizadas
O projeto é construído principalmente em Python, aproveitando o poder das seguintes bibliotecas:

* **Python 3.x**
* **OpenCV:** Para captura, exibição e processamento de vídeo da webcam.
* **MediaPipe:** Para a estimativa de pose e detecção de *landmarks*.
* **NumPy:** Para manipulação eficiente de dados numéricos.
* **Matplotlib:** Para a geração dos gráficos de análise pós-sessão.

---

## 🚀 Instalação e Configuração

Siga os passos abaixo para ter o PosturAI-Python rodando em sua máquina:

### 1. Clonar o Repositório
```bash
git clone https://github.com/FIAP-Global-Solution-2k25/PosturAI-Python.git

cd PosturAI-Python
````

### 2\. Criar e Ativar o Ambiente Virtual

É altamente recomendado o uso de um ambiente virtual para isolar as dependências.

**Criar o ambiente virtual (venv):**

```bash
python -m venv venv
```

**Ativar o ambiente virtual no macOS/Linux:**

```bash
source venv/bin/activate
```

**Ativar o ambiente virtual no Windows (Prompt de Comando ou PowerShell):**

```bash
venv\Scripts\activate
```

### 3\. Instalar as Dependências

Instale todas as bibliotecas necessárias listadas no arquivo `requirements.txt`:

```bash
pip install -r requirements.txt
```

### 4\. Executar o Aplicativo

Após a instalação, execute o script principal para iniciar o monitoramento de postura via webcam:

```bash
python main.py
# (Nota: o nome do arquivo principal pode ser ajustado conforme a estrutura final)
```

-----

## 🤝 Contribuição

Contribuições são o que tornam a comunidade de código aberto um lugar incrível para aprender, inspirar e criar. Qualquer contribuição que você fizer será **muito apreciada**.

1.  Faça um **Fork** do Projeto.
2.  Crie uma **Branch** para sua Feature (`git checkout -b feature/NovaFuncionalidade`).
3.  Commit suas Mudanças (`git commit -m 'Adiciona NovaFuncionalidade'`).
4.  Faça um **Push** para a Branch (`git push origin feature/NovaFuncionalidade`).
5.  Abra um **Pull Request**.

-----

## 📜 Licença

Este projeto está sob a licença **MIT**. Consulte o arquivo `LICENSE` no repositório para mais detalhes.

-----

<div align="center">
  Desenvolvido para a Global Solution 2025 da FIAP.
  
  Você pode encontrar mais informações sobre a Global Solution da FIAP no site oficial: <a href="https://www.fiap.com.br/graduacao/global-solution/?utm_term=&utm_campaign=GRAD+-+DSA&utm_source=adwords&utm_medium=ppc&hsa_acc=3358810376&hsa_cam=21102294227&hsa_grp=158449020381&hsa_ad=737370541126&hsa_src=g&hsa_tgt=dsa-2403784242683&hsa_kw=&hsa_mt=&hsa_net=adwords&hsa_ver=3&gad_source=1&gad_campaignid=21102294227&gbraid=0AAAAADqmiBBL0vsXCBVGF-uBG2qZC6mbY&gclid=CjwKCAiAlfvIBhA6EiwAcErpyZ9ifXZTOhMagASAJJAlFp0BM2fjwkvAjUnWgSHiFA5UMkvOpMlhyhoCflUQAvD_BwE">Global Solution FIAP</a>
</div>


