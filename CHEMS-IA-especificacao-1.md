# CHEMS IA — Especificação
### Plataforma Educacional Inteligente de Química · Desenvolvido pela Kappa AI

Documento de referência antes da fase de desenvolvimento real (backend, base de dados, servidor).

---

## 1. Visão Geral do Produto

O Chems IA é uma plataforma educacional inteligente, desenvolvida pela Kappa AI, criada para ajudar estudantes a aprender Química de forma moderna, interativa e personalizada. O aplicativo utiliza Inteligência Artificial para responder dúvidas, resolver exercícios, analisar imagens, gerar fichas, resumos e revisões personalizadas, adaptando-se ao desempenho de cada estudante.

**Modelo de negócio:** aplicativo gratuito, monetizado por anúncios. Não há cobrança directa para registar ou usar as funcionalidades base — a receita vem da visualização de anúncios dentro do app.

**Missão:** Tornar o estudo da Química mais simples, acessível e inteligente para estudantes de todos os níveis.

**Slogan:** *"A inteligência da química nas tuas mãos."*

**Slogan do sistema de moedas:** *"Estude, evolua e ganhe KappaCoins."*

---

## 2. Funcionalidades Principais

- 🤖 IA para responder perguntas de Química
- 📸 Resolução de exercícios por foto
- 📄 Geração de fichas, resumos e PDFs
- 🧠 Detecção automática das dificuldades do estudante, com exercícios personalizados
- 🧪 Quizzes inteligentes
- 🏆 Ranking entre estudantes
- 🌍 Ranking por cidades
- 👥 Sistema de amigos
- 🪙 KappaCoins (moeda virtual)
- 👑 Sistema Premium
- 🔔 Frase química diária (notificação)
- ⚛️ Identidade visual: logo com átomo + cérebro IA

---

## 3. Limite Grátis Diário (IA)

| Recurso | Limite grátis/dia | Depois do limite |
|---|---|---|
| Perguntas de texto à IA | **Ilimitado, sempre grátis** | Não aplicável |
| Resolução de exercício por foto | 10/dia | 40 KappaCoins por foto extra, ou ilimitado durante o Premium |

Perguntas de texto nunca custam KappaCoins nem exigem Premium — é a funcionalidade base e gratuita do Chems IA, sem restrição. O limite aplica-se apenas à resolução de exercício por foto, que tem custo computacional mais alto (análise de imagem). O limite de fotos reinicia todos os dias à meia-noite (hora local do estudante). Durante o Premium, o limite de fotos é removido.

---

## 4. Modelo de Monetização — Anúncios

O Chems IA usa **dois tipos de anúncio, combinados**:

1. **Anúncios automáticos (banner + intersticial)**
   - Banner: faixa discreta e fixa, sempre visível, não interrompe o uso.
   - Intersticial: tela cheia, exibido em momentos naturais de transição — por exemplo, ao terminar um quiz ou trocar de secção.
   - Gera receita constante, independente da vontade do aluno.

2. **Anúncios recompensados (rewarded ads)**
   - O aluno escolhe assistir, através de um botão como "Ver anúncio e ganhar KappaCoins".
   - É a **principal fonte de KappaCoins** no sistema.
   - Gera receita mais alta por visualização e aumenta o tempo de uso do app.

**Lógica central:** quanto mais o aluno quiser desbloquear (Premium, PDFs, recursos de IA, itens de perfil), mais anúncios recompensados assiste — o que sustenta a receita do aplicativo.

**Fornecedor de anúncios: Google AdMob, apenas no app Android.**

- A maioria dos alunos é esperada a instalar o app (mais conveniente que usar pelo navegador), e o app nativo paga mais por visualização que anúncios em página Web — especialmente os anúncios recompensados, que praticamente não existem em versão Web.
- A versão Web (acessada directamente pelo navegador, sem instalar o app) **não exibe anúncios por agora** — evita duplicar a integração (AdMob + AdSense) sem ganho relevante de receita, já que a maior parte do uso é esperada vir do app instalado.
- Quando o Android estiver validado e a gerar receita estável, pode-se reavaliar adicionar Google AdSense à versão Web.

---

## 5. Sistema Oficial de KappaCoins

KappaCoins são a moeda virtual oficial do Chems IA. Os estudantes ganham KappaCoins ao utilizar o aplicativo e podem trocá-las por benefícios.

### 4.1 Como Ganhar KappaCoins

| Acção | Recompensa | Observação |
|---|---|---|
| Assistir anúncios | 3 anúncios = 100 KappaCoins | Principal fonte; deve ser a forma que mais recompensa |
| Completar quiz | 25 KappaCoins | Por quiz concluído |
| Desafio diário | 80 KappaCoins | Por desafio concluído |
| Estudo diário | 50 KappaCoins | Por entrar e estudar no dia |
| Convidar amigos | Bónus por amigo registado | Valor a definir |
| Temporadas/ranking | Recompensas especiais | Para os melhores estudantes do período |

### 4.2 Como Gastar KappaCoins

**Premium temporário**
| Item | Custo |
|---|---|
| 30 minutos de Premium | 200 KappaCoins |

**PDFs e materiais**
| Item | Custo |
|---|---|
| Resumo simples (1 tema) | 50 KappaCoins |
| Ficha de revisão completa | 100 KappaCoins |
| Simulado personalizado | 150 KappaCoins |

**Recursos especiais da IA**
| Item | Custo |
|---|---|
| Resolução de exercício por foto (extra, além do limite grátis) | 40 KappaCoins |
| Pacote de 5 exercícios premium | 120 KappaCoins |

**Itens de perfil (cosméticos, sem afectar o estudo)**
| Item | Custo |
|---|---|
| Badge comum | 60 KappaCoins |
| Moldura de avatar | 150 KappaCoins |
| Efeito visual especial (animação no perfil) | 300 KappaCoins |

### 4.3 Objectivo do Sistema

Permitir que estudantes sem dinheiro real consigam desbloquear funcionalidades premium através do esforço e dedicação dentro do aplicativo — principalmente assistindo anúncios, o que sustenta a receita do Chems IA.

---

## 5.1 Premium por Assinatura (pago, separado do Premium temporário por coins)

Diferente do Premium temporário (200 KappaCoins = 30 minutos), este é um plano contínuo, pago com dinheiro real.

**Benefícios:**
- Zero anúncios (nem banner, nem intersticial, nem recompensado).
- Fotos de exercício ilimitadas (remove o limite de 10/dia).
- Todos os recursos de IA, PDFs e materiais sem gastar KappaCoins.

**Planos:**

| Plano | Preço | Equivalente mensal |
|---|---|---|
| Mensal | 99 MZN/mês | 99 MZN/mês |
| Anual | 1000 MZN/ano | ≈83 MZN/mês (16% de desconto vs. mensal) |

> Nota: os valores de preço foram definidos com base em raciocínio de acessibilidade para o público estudantil moçambicano, mas não foram confirmados com pesquisa de mercado actualizada (a busca não esteve disponível no momento). Recomenda-se validar contra o poder de compra real antes do lançamento.

**Tensão de modelo a ter em mente:** cada assinante deixa de gerar receita de anúncios. O valor da assinatura precisa compensar essa perda — é importante observar dados reais de receita por utilizador (anúncios) depois do lançamento, para confirmar se o preço está bem calibrado.

---

## 6. Quizzes

- Gerados pela IA de forma **aleatória**, sem categorias fixas no menu — mas o aluno pode **escolher o assunto** ao pedir (ex.: "quiz sobre ligações químicas"), em vez de receber só surpresa.
- Cada quiz tem **10 perguntas**.
- Limite de **15 quizzes por dia** por aluno.
- Cada quiz concluído = 25 KappaCoins (já definido na Secção 5) + 50 pontos de Ranking (Secção 7).

---

## 7. Ranking

O Ranking usa uma **pontuação própria, separada dos KappaCoins** — assim, a posição reflecte esforço real de estudo, e não depende de quanto dinheiro ou anúncios o aluno consome.

**Dois rankings em paralelo:**

| Ranking | Comportamento |
|---|---|
| Geral (histórico) | Vitalício — acumula desde a criação da conta, nunca reinicia. Funciona como um "hall da fama" de longo prazo. |
| Mensal | Reinicia todo mês — dá oportunidade justa a quem entrou recentemente. |

**Pontuação:**

| Acção | Pontos de Ranking |
|---|---|
| Quiz concluído | 50 pontos |
| Desafio diário concluído | 150 pontos |
| Estudo diário (entrar e estudar no dia) | 75 pontos |

Existe também o **Ranking por Cidades**, que agrega a pontuação de todos os alunos de uma mesma cidade — incentiva competição saudável entre escolas/regiões.

**Prémios da temporada mensal (Top 10, em KappaCoins):**

| Posição | Prémio |
|---|---|
| 1º lugar | 500 KappaCoins |
| 2º lugar | 350 KappaCoins |
| 3º lugar | 250 KappaCoins |
| 4º lugar | 180 KappaCoins |
| 5º lugar | 150 KappaCoins |
| 6º lugar | 120 KappaCoins |
| 7º lugar | 100 KappaCoins |
| 8º lugar | 80 KappaCoins |
| 9º lugar | 60 KappaCoins |
| 10º lugar | 50 KappaCoins |

O Ranking Geral (histórico/vitalício) não distribui prémios — serve como reconhecimento de longo prazo, sem recompensa monetária.

---

## 8. Sistema de Amigos

- Adicionar amigo por **código de convite ou link** (fácil de partilhar via WhatsApp).
- Amigos podem **comparar pontos de Ranking e KappaCoins** entre si — competição leve, sem duelo directo.
- **Bónus de convite**: o convidador ganha **50 KappaCoins** quando o amigo convidado completa o seu primeiro quiz (não basta só registar-se — evita contas falsas criadas só para gerar bónus).

---

## 9. Identidade de Marca

- Nome: Chems IA
- Desenvolvido por: Kappa AI
- Logo: átomo + cérebro IA
- Slogan principal: "A inteligência da química nas tuas mãos."
- Slogan KappaCoins: "Estude, evolua e ganhe KappaCoins."

---

## 10. Plataforma de Desenvolvimento

Decisão tomada para evitar o problema enfrentado no SIGES (créditos temporários do Replit a esgotarem-se).

**Estratégia: um único código para Web + Android, hospedagem grátis permanente (não créditos com prazo).**

| Camada | Ferramenta | Função |
|---|---|---|
| Interface (app) | PWA + Capacitor | Mesmo código serve para a versão Web e para empacotar como app Android |
| Base de dados + Autenticação | Supabase | Armazena alunos, perguntas, KappaCoins, ranking; login/registo já pronto |
| Backend (lógica da IA, regras de coins) | Render (ou funções da própria Supabase) | Onde a lógica do servidor roda |

**Por que este caminho:**
- Custo de desenvolvimento: **0 USD**, até o app gerar receita.
- "Tier grátis" destas ferramentas é **permanente**, não créditos com prazo de validade — elimina o risco que travou o SIGES.
- Um único código atende Web e Android ao mesmo tempo, sem duplicar trabalho.

**Custo que só aparece na hora de publicar (não antes):**
- Conta de desenvolvedor Google Play: 25 USD, taxa única, pago apenas no momento de publicar na loja.

**Faseamento decidido:**
1. Android primeiro (mercado-alvo: Moçambique).
2. iOS e expansão de loja, mais tarde, se houver receita que justifique os 99 USD/ano da Apple.

---

## 11. Pontos Ainda Pendentes

1. **Currículo oficial do MINEDH (Moçambique), 8ª-12ª classe** — pesquisa pendente para alinhar perguntas, quizzes e fichas ao programa real de Química do ensino moçambicano.
2. **Validação dos preços do Premium por assinatura** (99 MZN/mês, 1000 MZN/ano) contra dados reais de mercado/poder de compra — definidos por raciocínio, sem confirmação por pesquisa actualizada.
