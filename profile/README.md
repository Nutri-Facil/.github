# 🥗 Nutri-Fácil

## 📋 Descrição do Projeto

**Nutri-Fácil** é uma ferramenta funcional, intuitiva e bem documentada que auxilia os usuários na adoção de hábitos saudáveis de forma prática e segura. O sistema personaliza recomendações nutricionais com base nas necessidades individuais, promovendo bem-estar por meio da tecnologia e decisões alimentares conscientes.

## 🚀 Funcionalidades

```markdown
- Seleção personalizada de dietas: Mediterrânea, Low Carb, Cetogênica e Vegetariana
- Cálculo automático de:
  - TMB (Taxa de Metabolismo Basal)
  - IMC (Índice de Massa Corporal)
  - Consumo diário de água
- Geração de recomendações alimentares por categoria:
  - Proteínas, legumes, verduras e carboidratos
- Adaptação das recomendações ao objetivo do usuário:
  - Emagrecimento ou hipertrofia
- Gerenciamento de restrições alimentares:
  - Intolerâncias e alergias como lactose, glúten, frutos do mar, entre outras
- Interface amigável e responsiva
- Testes de funcionalidade com Jest
```

## 🛠️ Tecnologias Utilizadas

```markdown
- HTML5
- CSS3
- JavaScript
- Jest (para testes unitários)
```

## 💻 Instalação e Execução

```markdown
1. Clone o repositório:
   git clone https://github.com/seu-usuario/nutri-facil.git
   cd nutri-facil

2. Abra o arquivo index.html em qualquer navegador moderno.

3. Para rodar os testes com Jest:
   npm install
   npm test
```

## ✅ Uso do Projeto

```markdown
Ao acessar o Nutri-Fácil, o usuário pode:

1. Selecionar uma dieta de acordo com seu perfil e preferências.
2. Informar peso, altura, idade, sexo, objetivo (emagrecimento ou hipertrofia) e restrições alimentares.
3. Receber cálculos personalizados de TMB, IMC e necessidade diária de água.
4. Visualizar uma lista de alimentos recomendados conforme sua dieta, incluindo quantidades e calorias.
5. Adaptar as preferências alimentares por categoria (proteínas, legumes, verduras e carboidratos).
6. Obter recomendações seguras e personalizadas com base em seu perfil.
```

## 🙌 Créditos

```markdown
Este projeto foi desenvolvido por:

- @BJesuss
- @guivpn
- @Leonardogabriels
- @MarcoThulio1207
- @prod01
- @WesleyFilemon
```

## 2. Casos de Teste (exemplo)
      
      | ID   | Funcionalidade                   | Pré-Condição                        | Passos                                                   | Dados de Entrada                          | Resultado Esperado                                                                 | Resultado Obtido                            | Status (✅/❌) | Observações                         |
      | ---- | -------------------------------- | ----------------------------------- | -------------------------------------------------------- | ----------------------------------------- | ---------------------------------------------------------------------------------- | --------------------------------------------- | ------------- | ------------------------------------ |
      | FT-01 | Seleção de Dieta Mediterrânea                | Usuário autenticado e página de “Seleção de Dieta” aberta                | 1. Acessar a tela de seleção de dieta  2. Selecionar a opção **“Mediterrânea”**  3. Preencher o campo **Peso** com `70` kg  4. Preencher o campo **Altura** com `170` cm  5. Preencher o campo **Idade** com `30` anos  6. Selecionar **Sexo** como `Feminino`  7. Clicar no botão **“Solicitar Plano Alimentar”**                        |      - Dieta: `Mediterrânea`  - Peso: `70`  - Altura: `170`  - Idade: `30`  - Sexo: `Feminino`     |  O sistema exibe um plano alimentar contendo refeições ricas em azeite de oliva, peixes e grãos integrais.      |       _(preencher após a execução do teste)_        |                                    |
            
      ---

IMC: 24 Peso Normal
Água: 2450ml/dia
Objetivo: Emagrecer
Plano alimentar: Saúde cardiovascular e
manutenção de peso        |              ✅                      |