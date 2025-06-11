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
| FT-01 | Seleção de Dieta Mediterrânea                | Usuário autenticado e página de “Seleção de Dieta” aberta                | 1. Acessar a tela de seleção de dieta 2. Selecionar a opção “Mediterrânea” 3. Preencher o campo Peso com 70kg 4. Preencher o campo Altura com 170 cm 5. Preencher o campo Idade com 30 anos 6. Selecionar Sexo como Feminino 7. Selecionar o objetivo "Emagrecimento" 8. Selecionar uma restrição alimentar "Nenhuma" 9. Clicar no botão “Continuar Para Preferências Alimentares” 10. Selecionar preferências alimentar 11. Clicar no botão "Ver Meu Plano Alimentar" |      - Dieta: `Mediterrânea`  - Peso: `70`  - Altura: `170`  - Idade: `30`  - Sexo: `Feminino`     |  O sistema exibe um plano alimentar contendo refeições ricas em azeite de oliva, peixes e grãos integrais.      |       Taxa metabólica basal: 1451kcal/diaIMC: 24 Peso NormalÁgua: 2450ml/dia Objetivo: Emagrecer Plano alimentar: Saúde cardiovascular e manutenção de peso_        |                ✅                    |
| FT-02 | Seleção de Dieta Low Carb                | Usuário autenticado e página de “Seleção de Dieta” aberta                | 1. Acessar a tela de seleção de dieta 2. Selecionar a opção “Low Carb” 3. Preencher o campo Peso com 85kg 4. Preencher o campo Altura com 172 cm 5. Preencher o campo Idade com 27 anos 6. Selecionar Sexo como Masculino 7. Selecionar o objetivo "Emagrecimento" 8. Selecionar uma restrição alimentar "Nenhuma" 9. Clicar no botão “Continuar Para Preferências Alimentares” 10. Selecionar preferências alimentar 11. Clicar no botão "Ver Meu Plano Alimentar"  |      - Dieta: `Low Carb` - Peso: `85` - Altura: `172` - Idade: `27` - Sexo: `Masculino`     |  O sistema exibe um plano alimentar contendo refeições ricas nas preferências que foram solicitadas (Redução de carboidratos, aumento de proteínas e gorduras boas)      |       Taxa metabólica basal: 1795kcal/dia IMC: 28 Sobrepeso Água: 2975ml/dia Objetivo: Emagrecer Plano alimentar: Emagrecimento e controle glicêmico        |                ✅                    |
| FT-03 | Seleção de Dieta Cetogênica               | Usuário autenticado e página de “Seleção de Dieta” aberta               | 1. Acessar a tela de seleção de dieta 2. Selecionar a opção “Cetogênica” 3. Preencher o campo Peso com 62kg 4. Preencher o campo Altura com 160 cm 5. Preencher o campo Idade com 25 anos 6. Selecionar Sexo como Feminino 7. Selecionar o objetivo "Emagrecimento" 8. Selecionar uma restrição alimentar "Nenhuma" 9. Clicar no botão “Continuar Para Preferências Alimentares” 10. Selecionar preferências alimentar 11. Clicar no botão "Ver Meu Plano Alimentar"   |      - Dieta: `Cetogênica` - Peso: `62` - Altura: `160` - Idade: `25` - Sexo: `Feminino`     |  O sistema exibe um plano alimentar contendo refeições ricas nas preferências que foram solicitadas (Ingestão muito baixa de carboidratos e alta em gorduras)      |       Taxa metabólica basal: 1334kcal/dia IMC: 24 Sobrepeso Água: 2170ml/dia Objetivo: Emagrecer Plano alimentar: Perda de gordura rápida e aumento de foco        |                ✅                    |           
| FT-04 | Seleção de Dieta Vegetariana               | Usuário autenticado e página de “Seleção de Dieta” aberta               | 1. Acessar a tela de seleção de dieta 2. Selecionar a opção “Vegetariana” 3. Preencher o campo Peso com 83kg 4. Preencher o campo Altura com 157 cm 5. Preencher o campo Idade com 43 anos 6. Selecionar Sexo como Feminino 7. Selecionar o objetivo "Emagrecimento" 8. Selecionar uma restrição alimentar "Nenhuma" 9. Clicar no botão “Continuar Para Preferências Alimentares” 10. Selecionar preferências alimentar 11. Clicar no botão "Ver Meu Plano Alimentar"    |      - Dieta: `Vegetariana` - Peso: `83` - Altura: `157` - Idade: `43` - Sexo: `Feminino`     |  O sistema exibe um plano alimentar contendo refeições ricas nas preferências que foram solicitadas (Sem carnes; inclui ovos, laticínios, grãos, vegetais e leguminosas)      |       Taxa metabólica basal: 1435kcal/dia IMC: 33 Sobrepeso Água: 2905ml/dia Objetivo: Emagrecer Plano alimentar: Alimentação plant-based com proteínas completas        |                ✅                    |      Inclui ovos e laticínios que podem ser retirados pelo usuário         |
| FT-05 | Cálculo de TMB, IMC e Consumo de Água              | Usuário autenticado, Dieta Selecionada, Dados Pessoais Preenchidos e Preferências Alimentares Selecionadas               | 1. Acessar a tela de seleção de dieta 2. Selecionar a opção “Mediterrânea” 3. Preencher o campo Peso com 92kg 4. Preencher o campo Altura com 180 cm 5. Preencher o campo Idade com 46 anos 6. Selecionar Sexo como Masculino 7. Selecionar o objetivo "Emagrecimento" 8. Selecionar uma restrição alimentar "Nenhuma" 9. Clicar no botão “Continuar Para Preferências Alimentares” 10. Selecionar preferências alimentar 11. Clicar no botão "Ver Meu Plano Alimentar"     |      - Dieta: `Mediterrânea` - Peso: `92` - Altura: `180` - Idade: `46` - Sexo: `Masculino`     |  O sistema exibe o resultado do TMB, IMC e o Consumo de água ideal.      |       Taxa metabólica basal: 1820kcal/dia IMC: 28 Sobrepeso Água: 3220ml/dia Objetivo: Emagrecer Plano alimentar: Saúde cardiovascular e manutenção de peso        |                ✅                    |      
---

IMC: 24 Peso Normal
Água: 2450ml/dia
Objetivo: Emagrecer
Plano alimentar: Saúde cardiovascular e
manutenção de peso        |              ✅                      |


## 🐞 Registro de Bugs
```markdown
| ID do Bug | Caso de Teste Relacionado | Descrição do Problema                                                                                               | Severidade | Status    | Responsável     |
| --------- | ------------------------- | ------------------------------------------------------------------------------------------------------------------- | ---------- | --------- | --------------- |
| BUG-01    | FT-08                     | Alimentos contendo lactose podiam ser escolhidos mesmo ao selecionar "Lactose" como restrição alimentar             | Alta       | Resolvido | Pedro Rodrigues |
| BUG-02    | FT-08                     | Ovos podiam ser escolhidos como preferência alimentar mesmo ao selecionar “Ovos e Lactose” como restrição alimentar | Alta       | Resolvido | Pedro Rodrigues |
| BUG-03    | FT-07                     | Era possível selecionar “Selecione seu objetivo” como opção ao invés de “Hipertrofia” ou “Emagrecimento”            | Alta       | Resolvido | Marco Thulio    |
| BUG-04    | FT-07                     | Era possível selecionar “Selecione” como sexo ao invés de “Masculino” ou “Feminino”                                 | Alta       | Resolvido | Marco Thulio    |
| BUG-05    | FT-03                     | IMC mostra “peso normal” mesmo com valores de peso e altura incompatíveis                                           | Alta       | Resolvido | Marco Thulio    |
| BUG-06    | FT-02                     | TMB calculada incorretamente para valores extremos                                                                  | Alta       | Resolvido | Marco Thulio    |
| BUG-07    | FT-07                     | Campo de entrada de altura aceita valores negativos                                                                 | Média      | Resolvido | Pedro Rodrigues |
| BUG-08    | FT-08                     | Preferência de alimentos não é salva corretamente entre sessões                                                     | Baixa      | Resolvido | Pedro Rodrigues |
| BUG-09    | FT-03                     | Ao selecionar dieta Cetogênica, ainda são sugeridos alimentos ricos em carboidratos                                 | Alta       | Resolvido | Marco Thulio    |
| BUG-10    | FT-04                     | Consumo de água não é recalculado após alteração de peso                                                            | Média      | Resolvido | Marco Thulio    |
```
