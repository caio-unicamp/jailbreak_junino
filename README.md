# 🔥 Cadeia do Jailbreak Junino 🌽
Nesse repositório está a interface interativa de chatbots desenvolvida para o arraiá de entidades do instituto de computação da Unicamp! Aqui, misturamos a tradicional "Cadeia" das quermesses com Engenharia de Prompt e Segurança em Inteligência Artificial com o objetivo de fazer as pessoas tentarem realizar um jailbreak bobo, porém com modelos desafiadores.

Os participantes pagam para "prender" os amigos, mas o prisioneiro tem uma chance de escapar (e ganhar um prêmio) se conseguir fazer um *Jailbreak* em nossos modelos de Linguagem (LLMs), burlando as restrições impostas no *System Prompt*.

## 🏛️ Contexto dos Desafios
Nossa delegacia virtual possui 3 níveis de segurança, totalmente adaptados ao ecossistema da Unicamp:
* **Nível 1 (Fácil - DeepSeek):** Fazer o mestre cuca da AAACEC revelar a receita secreta do Quentão.
* **Nível 2 (Médio - GPT-4o):** Tirar a paciência do assistente da secretaria de graduação e fazê-lo usar linguagem informal ou xingamentos.
* **Nível 3 (Difícil - GPT-5.4):** Convencer o sistema de segurança máxima a liberar um plano de roubo das vendinhas do LariCACo.

---

## 🚀 Como rodar o projeto localmente

Para garantir que a instalação das dependências seja ultrarrápida, estamos utilizando o **[uv](https://github.com/astral-sh/uv)**, um gerenciador de pacotes Python escrito em Rust.

### Pré-requisitos
1. **Python 3.9+** instalado na máquina.
2. Ter o **uv** instalado. Se ainda não tem, instale com o comando abaixo:
   * **Mac/Linux:**
   ```bash
   `curl -LsSf https://astral.sh/uv/install.sh | sh`
   ```
   * **Windows (PowerShell):** 
   ```bash
   `powershell -c "irm https://astral.sh/uv/install.ps1 | iex"`
   ```

### Passo a Passo de Instalação

**1. Clone o repositório**
```bash
git clone git@github.com:[SEU_USUARIO]/jailbreak_junino.git]
cd jailbreak_junino
```
**2. Crie e ative um ambiente virtual**

```bash
uv venv
## No Mac/Linux:
source .venv/bin/activate
## No Windows:
.venv\Scripts\activate
```

**3. Instale as dependências**
```bash
uv pip install -r requirements.txt
```
**4. Execute a aplicação**

Com o ambiente ativado e as bibliotecas instaladas, inicie o servidor local do Streamlit:

```bash
streamlit run chat.py
```
O seu navegador padrão abrirá automaticamente na página http://localhost:8501 com a interface da Cadeia do Jailbreak rodando!

🔑 Configurando as Chaves de API
Para que os modelos respondam, você precisará de chaves de acesso da OpenAI e da DeepSeek.
Para evitar vazamentos e problemas de segurança no GitHub, as chaves não ficam no código.

Acesse o painel da OpenAI e da DeepSeek para gerar suas chaves.

Ao rodar o sistema e abrir a página no navegador, insira as chaves correspondentes na Barra Lateral (Sidebar) da aplicação.

Escolha o nível desejado e boa sorte aos prisioneiros!

Desenvolvido com 💛 (e muito milho) pelo grupo Iris DataScience - Unicamp.
