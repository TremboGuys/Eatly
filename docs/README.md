# Projeto Integrador - Modelo
# Eatly

Um modelo para o desenvolvimento do Projeto Integrador do Curso de Técnico em Desenvolvimento de Sistemas para a Internet Integrado ao Ensino Médio do IFC - Campus Araquari.

A Eatly busca expandir seus lucros intermediando vendas e entregas, além da hospedagem de restaurantes. O novo sistema permitirá pedidos online, rastreamento de entregas e avaliações. Restaurantes poderão gerenciar pedidos e cardápios, enquanto entregadores terão suporte via GPS. Administradores controlarão taxas, suporte e políticas da plataforma. A transparência será reforçada com relatórios detalhados para os restaurantes.

Equipe:
- [João](https://github.com/Joaovictor23t4)
- [Lucas](https://github.com/dnzlucas)
- [Luiz](https://github.com/LuizBlume)
- [Luna](https://github.com/LunaBolsoni)
- [Sara](https://github.com/SaraKozoski)

- [Documentação (esse documento)](https://github.com/TremboGuys/eatly_docs/blob/main/docs/README.md)
- Backend: [Repositório](https://github.com/TremboGuys/backend) e [Publicação](https://eatly-backend-cbai.onrender.com/api/)
- Frontend: [Repositório](https://github.com/TremboGuys/eatly_frontend) e [Publicação](https://eatly-frontend-trza.onrender.com)

# 1. Desenvolvimento

## 1.1 Modelo de sistema

### 1.1.1 Ordem de vendas

O dono de uma empresa chamada *Eatly* nos contatou com o intuito de aumentar os lucros de sua empresa. A Eatly faz parte do ramo de serviço de hospedagem de restaurantes, e há um rápido crescimento do interesse de mais restaurantes em ingressar no site. Sua forma lucrativa é por meio do aluguel da hospedagem de restaurantes no site, mas quer aumentar os seus lucros, por isso nos contactou.

# 2. Situação Problema

Sr. Diniz é dono da Eatly, uma empresa que existe a 1 ano e que conta com 2 desenvolvedores que fazem a manutenção do sistema.

No site do Sr. Diniz (Eatly), é necessário o cliente informar seu endereço, após isso ele pode escolher a categoria da comida que deseja consumir e uma seleção de restaurantes aparecem com base na categoria e endereço informados para que o cliente possa contatar o restaurante mais próximo e que mais se encaixa com sua fome. Após escolher, é informado o telefone e endereço do restaurante, para que o cliente contacte como deseja.

A forma como seu sistema lucra atualmente é com o pagamento dos restaurantes para que seus nomes apareçam nas pesquisas. Mas Diniz quer aumentar seus lucros, e conta com a gente para isso, ele pensa em além de ganhar com o aluguel dos restaurantes no sistema, também ganhar uma porcentagem das vendas realizadas no site, expandindo os serviços prestados pela empresa.

Um dos problemas que percebi no Eatly é a falta de transparência a empresa hospedada sobre quanto suas vendas aumentaram com a hospedagem no site de Sr. Diniz, e se vale apena ou não continuar pagando sua hospedagem no sistema. Uma boa maneira de ajustar é informando um relatório individual ao restaurante, sobre quantas vezes sua página foi acessada pelos clientes do Eatly, além é claro, de quantas **vendas** foram realizadas. Como vimos, o Sr. Diniz tem um pequeno software, e ele já vê os frutos da ajuda de um, mas agora, com seu software expandindo ainda mais e ficando mais robusto, ele poderá ver ainda mais benefícios, como receber outras fontes de lucro, por pagamentos de vendas realizadas, uma maior confiança dos restaurantes, com a garantia de possíveis relatórios e etc.

# 3. Descrição da Proposta

O foco de nosso software será ainda na hospedagem dos restaurantes e na sua visibilidade para pesquisas do usuário, mas agora principalmente para as vendas dos produtos desses restaurantes, e por fim na entrega de tais produtos ao usuário, agindo assim como um intermediador entre o restaurante e o cliente.

Falando agora de níveis de usuário do sistema, no planejamento é pensado em  tipos de usuário: cliente, restaurante, entregadores e administradores. Falaremos sobre as diferenças mais a frente.

As ações que um usuário poderá realizar em nosso software seriam:

- Pesquisar restaurantes por categoria alimentícia, como hambúrgueres, pizzas, pastéis, etc.
- Pesquisar um restaurante específico.
- Fazer um pedido por meio do nosso sistema.
- Acompanhar sua entrega.
- Realizar avaliações a restaurantes.

Agora sobre as diferenças de usuário:

- **Cliente**: poderá realizar pedidos e avaliações, além de processar pagamentos.
- **Restaurantes**: poderão gerenciar os pedidos que receberem, atualizar as opções de cardápio, bem como seus preços, responder avaliações de clientes e também atualizar o tempo de entrega mostrado no app conforme necessidade.
- **Entregadores**: recebem e realizam entregas, terão um GPS para a rota, bem como o valor a ser ganho na entrega, além de poder realizar avaliações a clientes e restaurantes.
- **Administradores**: gerenciam as taxas aos pedidos e mudam as políticas de privacidade caso necessário. Oferecem suporte a clientes, restaurantes e entregadores.

# 4. Modelo Entidade-Relacionamento

![image desc](./docs/modelagem_eatly.png)
[PDF da Modelagem](https://drive.google.com/drive/folders/1E8S3AcIBVeQJAK0EMntGa760i8VUi3qH?hl=pt-br)

# 4. Requisitos Funcionais

RF-001: O sistema deve manter um usuário cliente.

RF-002: O sistema deve manter restaurantes.

RF-003: O sistema deve manter proprietários de restaurantes.

RF-004: O sistema deve manter entregadores.

RF-005: O sistema deve manter veículos.

RF-006: O sistema deve manter produtos.

RF-007: O sistema deve manter pedidos.

RF-008: O sistema deve oferecer suporte a rastreamento em tempo real da entrega, exibindo a localização do entregador e atualizações de status.

RF-009: O sistema deve manter cupons.

RF-010: O sistema deve oferecer cupons de frete grátis em compras acima de R$150,00.

RF-011: O sistema deve disponibilizar uma interface onde o usuário possa visualizar, adquirir e resgatar cupons, considerando regras de uso, validade, valor mínimo e limite de uso por usuário.

RF-012: O sistema deve permitir que os usuários realizem pagamentos via cartão de crédito/débito, Pix ou dinheiro.

RF-013: O sistema deve manter os planos de restaurantes (básico e de entregadores).

RF-014: O sistema deve permitir que o usuário cliente e o entregador se autentiquem por e-mail e senha ou autenticação via Google.

RF-015: O sistema fornecerá ao restaurante a autenticação via CNPJ e senha.

RF-016: O sistema deve permitir a redefinição de senha via e-mail em caso de esquecimento da mesma.

RF-017: O sistema deve permitir ao usuário cliente o salvamento de múltiplos endereços.

RF-018: O sistema deve permitir ao usuário cliente o salvamento de múltiplos números de telefone.

RF-019: O sistema deve permitir a busca de produtos e restaurantes por nome, preço, categoria e localização.

RF-020: O sistema deve permitir a filtragem de produtos dentro do cardápio do restaurante por categoria, faixa de preço e disponibilidade.

RF-021: O sistema deve permitir que o usuário acompanhe os status do seu pedido *("pendente", "em preparação", "saiu para entrega", "entregue")*.

RF-022: O sistema deve permitir que o usuário avalie um restaurante ou entregador após cada pedido.

RF-023: O sistema deve permitir ao usuário que adicione/remova um produto a seção de favoritos.

RF-024: O sistema deve manter um log de todas as alterações críticas (pedidos, pagamentos e cadastros).

RF-025: O sistema deve permitir a geração de relatórios de vendas, entregas, cupons usados e o faturamento total gerado.

# 5. Regras de negócio

### 1. RN-001
 <font size=4.5>**Número Identificador**:</font> RN-001
 <font size=4>**Nome**:</font> Cadastro do Usuário Cliente
 <font size=4>**Data de Criação:**</font> 06/04/2025
 <font size=4>**Data da Última Atualização:**</font> 06/04/2025
 <font size=4>**Autor:**</font> João Victor Portela Rocha
 <font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências:**</font> RN-002 (Validação do Email), RN-003 (Permissões para cada faixa etária).
 - Os campos obrigatórios para o cadastro do usuário são: **nome, gênero, data de nascimento, email, senha e telefone**.
 - O email deve ser **único** no sistema, caso o usuário tente cadastrar um email já existente, deverá ser apresentado na tela o erro "Este email já foi cadastrado!".
 -  Para detalhes da validação do email, por favor consulte a RN-002 (Validação de emails).
 - A senha deverá conter pelo menos 8 dígitos, com no mínimo uma letra maiúscula, uma minúscula, um número e um dígito especial.
 - Para uma abordagem detalhada da resposta necessária do sistema referente a data de nascimento informada, por favor consulte a RN-003 (Permissões para cada faixa etária).
 - O número de telefone deve ser salvo no sistema sem formatação, exemplo: 912345678. No input da plataforma, pode haver a formatação para uma ajuda visual ao usuário, mas para o envio de dados, certifique-se de enviar apenas os números.

### 2. RN-002
<font size=4.5>**Número Identificador**:</font> RN-002
<font size=4>**Nome**:</font> Validação do Email
<font size=4>**Data de Criação:**</font> 11/04/2025
<font size=4>**Data da Última Atualização:**</font> 11/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências:**</font>
 - No formulário de cadastro de usuários (não importa o tipo), verifique antes de permitir a submissão, se o email do usuário está no padrão "*@email.com*", se não estiver, envie um erro com o problema. OBS: o "email" de *@email.com* está genérico, pois existem vários serviços de email, como o Gmail, outlook (antigo hotmail), incluindo até emails de empresas.
 - Após fazer a submissão, mostre uma tela avisando que nosso serviço enviou um email de confirmação para o email cadastrado pelo usuário.
 - O usuário só poderá logar e realizar suas ações após confirmar o email. Ele tem até 24 horas para confirmar seu email, após isso seu pré-cadastro realizado na plataforma será excluído e ele terá de fazer de novo.
 - **Casos excepcionais:**
	 - 1. O usuário errou o email de cadastro: neste caso, logicamente o usuário não conseguirá confirmar seu email. Podendo ocorrer estes casos nós permitimos que o usuário realize um novo cadastro, para que possa usufruir da plataforma. Quanto ao cadastro com o email errado, ele será excluído após 24h, então não há problemas.

### 3. RN-003
<font size=4.5>**Número Identificador**:</font> RN-003
<font size=4>**Nome**:</font> Permissões Para Cada Faixa Etária
<font size=4>**Data de Criação:**</font> 11/04/2025
<font size=4>**Data da Última Atualização:**</font> 12/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
<font size=4>**Dependências:**</font>
 - Para usuários **menores de 16 anos**: usuários menores de 16 anos são proibidos de criar uma conta na plataforma.
 - Para usuários **menores de 18 anos**: Usuários que tenham entre 16 e 17 anos podem criar uma conta na plataforma e usufruir de maneira limitada, sendo proibido apenas de comprar produtos permitidos apenas para maiores de 18 anos, como o álcool.

	<font size=5>**Como verificar a idade**</font>
	
	Para fins jurídicos, não podemos apenas pedir a idade e dar como infalível esse método, por isso teremos de criar mais meios para isso.
	
	1. **Pedir a idade na hora do cadastro**: já citado, o mais comum é este, mas não garante a veracidade da informação, porém ainda vamos pedir para ter um leve controle dos usuários que se cadastram na nossa plataforma.
	2. **Pedir o registro do RG na plataforma**: é a única forma de realmente ter certeza da maior idade do usuário.
	3. **Pedir a identidade antes de entregar o pedido**: caso o usuário não registre o RG, ele terá de apresentar o RG na hora da entrega. Caso o RG apresente menor-idade, o motoboy cancelará a entrega e o usuário haverá de pagar mesmo assim, seja na hora ou num próximo pedido.

### 4. RN-004
<font size=4.5>**Número Identificador**:</font> RN-004
<font size=4>**Nome**:</font> Cadastro de Restaurantes
<font size=4>**Data de Criação:**</font> 12/04/2025
<font size=4>**Data da Última Atualização:**</font> 12/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências:**</font>
-  Para iniciar o cadastro, é necessário o registro do proprietário do restaurante, que terá de informas os seguintes dados: nome, CPF, RG, o órgão emissor do RG, data de nascimento, email, senha, telefone e endereço.
- Para cadastrar um restaurante, é necessário os seguintes dados: CNPJ, telefone, a área alimentícia que o restaurante trabalha e o endereço do restaurante.
- Após o cadastro do *proprietário* e inseridas as informações do restaurante, o cadastro do mesmo irá para análise da nossa equipe, para verificar todas as informações, e quando uma decisão surgir (aprovação, necessidade de edição dos dados ou até mesmo reprovação em casos raros), um email será enviado ao proprietário.

### 5. RN-005
<font size=4.5>**Número Identificador:**</font> RN-005
<font size=4>**Nome:**</font> Cadastro de Entregadores
<font size=4>**Data de Criação:**</font> 12/04/2025
<font size=4>**Data da Última Atualização:**</font> 22/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências:**</font> RN-006 (Cadastro de Veículos)
- Os cadastros obrigatórios para um motoboy em nosso sistema é: CPF, CNH, data de nascimento, telefone, endereço, foto (selfie ou documento com foto), email e senha.

<font size=4.5>**Verificação da existência do motoboy**</font>
- Validação do CPF: podemos validar o CPF por meio de algoritmos, para ver se está formatado corretamente.
- CNH: devemos verificar se há irregularidades na CNH do usuário. Podemos fazer isso pedindo um PDF da Carteira Digital de Trânsito.
- Foto junto da CNH: com uma foto do rosto do motoboy junto da CNH podemos comparar a aparência dos rostos e os dados informados com a foto.

<font size=4.5>**Fluxograma de aprovação**</font>
1. O motoboy preenche todos os dados e faz o upload dos documentos.
2. O sistema valida automaticamente o CPF e formato da placa.
3. Os documentos são analisados (via API ou manualmente).
4. Se tudo estiver certo, o status do entregador vira `Aprovado`.
5. Caso contrário, o sistema marca como `Pendente` ou `Reprovado`, e envia uma notificação com o motivo.

### 6. RN-006
<font size=4.5>**Número Identificador:**</font> RN-006
<font size=4>**Nome:**</font> Cadastro de Veículos
<font size=4>**Data de Criação:**</font> 22/04/2025
<font size=4>**Data da Última Atualização:**</font> 22/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências:**</font>

<font size=4.5>**Dados do Veículo**:</font>
1. Tipo do veículo (moto, bicicleta, carro).
2. Placa do veículo.
3. Modelo, marca e o ano.
4. PDF ou foto do CRLV (documento de licenciamento do veículo).

<font size=4.5>**Verificar veracidade do veículo**</font>
1. Faça a validação do campo relacionado a placa do veículo, no formato AAA-0A00 (Mercosul) e no formato antigo também (ABC-1234).
2. Podemos utilizar a API oficial do Detran (Senatran), para ver irregularidades do veículos, multas, proprietário e etc. Porém essa API é paga, então não é tão eficiente para pequenas empresas.
3. Junto da validação, podemos pedir a foto do veículo junto da placa para verificar se as informações foram corretamente preenchidas. Dessa maneira, teremos total veracidade do veículo.

### 7. RN-007
<font size=4.5>**Número Identificador:**</font> RN-007
<font size=4>**Nome:**</font> Cadastro de Produtos
<font size=4>**Data de Criação:**</font> 25/04/2025
<font size=4>**Data da Última Atualização:**</font> 25/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências:**</font>
- É necessário estar logado na conta do restaurante.
- Os campos necessários para se cadastrar um produto são: nome, descrição, valor, calorias, categoria do alimento e se ele é um produto para maiores de idade ou não.

### 8. RN-008
<font size=4.5>**Número Identificador:**</font> RN-008
<font size=4>**Nome:**</font> Gerenciamento de Produtos
<font size=4>**Data de Criação:**</font> 25/04/2025
<font size=4>**Data da Última Atualização:**</font> 25/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências:**</font>
- É permitido atualizar detalhes do produto, todos os campos são passíveis de atualização.
- **Não é permitido** excluir um produto, pois outros dados podem se relacionar com ele e gerar erros no futuro.
- Para lidar com o problema de remover um produto do cardápio, o restaurante pode atualizar o status dele para **arquivado**, dessa maneira o produto sairá do cardápio do restaurante, não sendo mais permitido fazer pedidos com ele.
- Caso algum produto esteja impossibilitado de ser preparado, como a falta de algum ingrediente ou algo do tipo, o restaurante poderá atualizar o status do produto para **inativo**, desse modo, o produto será visualizado com um símbolo de indisponível, indo para o final do cardápio e não sendo permitido adicioná-lo a um pedido.
- O status *padrão* de um produto é o **ativo**, ou seja, o restaurante ainda o vende e não há nenhum problema que o impeça de ser preparado.

### 9. RN-009
<font size=4.5>**Número Identificador:**</font> RN-009
<font size=4>**Nome:**</font> Criação de um Pedido
<font size=4>**Data de Criação:**</font> 25/04/2025
<font size=4>**Data da Última Atualização:**</font> 25/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências**</font>: RN-007 (Cadastro de produtos), RN-008 (Gerenciamento de produtos) RN-010 (Uso do cupom), RN-011 (Horário de funcionamento do restaurante)
- Para iniciar um pedido, o usuário deve escolher um restaurante aberto.
- Todos os produtos escolhidos devem estar com o status *ativo*.
- O usuário deve indicar um endereço válido.
- Pedidos acima de R$150,00 terão sempre frete grátis. O benefício do frete grátis não conta como um cupom utilizado, podendo o usuário escolher mais um se preferir.
- O método de pagamento deve ser compatível com os aceitos pelo restaurante.
- Caso o usuário decidir usar um cupom, o  mesmo deve estar ativo, dentro do prazo e sua condição de uso deve estar correta (ex: se o cupom for para pedidos maiores de R$50,00, então o cupom só pode ser usado em pedidos maiores que R$50,00).
- O usuário só poderá utilizar um cupom por pedido.

### 10. RN-010
<font size=4.5>**Número Identificador:**</font> RN-010
<font size=4>**Nome:**</font> Uso do cupom
<font size=4>**Data de Criação:**</font> 25/04/2025
<font size=4>**Data da Última Atualização:**</font> 25/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências:**</font>
- Um cupom é composto pelos campos: nome, descrição, tipo, desconto, preço do cupom, valor minimo para usá-lo e data de validade.
- É opcional que um cupom seja pago, o próprio sistema pode oferecer a partir de uma certa condição.
- É opcional que um cupom tenha data de validade. A menos que sejam **pagos** , sendo assim, eles **não** podem ter data de validade.
- Um usuário só pode ter 3 cupons por vez.
- Um cupom só poderá dar um desconto de no máximo 30% do valor do produto, mas com algumas restrições.
<font size=4>**Teto máximo de cada cupom**</font>
		- Cupom de 30%: Só poderá ser usado em compras de até R$300,00
		- Cupom de 20%: Só poderá ser usado em compras de até R$500,00
		- Cupom de 15%: Só poderá ser usado em compras de até R$700,00.
		- Cupom de 10%: Só poderá ser usado em compras de até R$1000,00.
- Quanto menor o desconto, mais o usuário vai ter que pagar para utilizá-lo. Quanto maior o desconto, menos o usuário terá de gastar, porém mais baixo será seu teto.
<font size=4>**Piso mínimo de cada cupom**</font>
		- Cupom de 30%: Poderá ser usado em compras a partir de R$150,00.
		- Cupom de 20%: Poderá ser usado em compras a partir de R$200,00.
		- Cupom de 15%: Poderá ser usado em compras a partir de R$250,00.
		- Cupom de 10%: Poderá ser usado em compras a partir de R$300,00.

### 11. RN-011
<font size=4.5>**Número Identificador:**</font> RN-011
<font size=4>**Nome:**</font> Horário de Funcionamento do Restaurante
<font size=4>**Data de Criação:**</font> 27/04/2025
<font size=4>**Data da Última Atualização:**</font> 27/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
 <font size=4>**Dependências:**</font>
 - O aplicativo apenas efetuará o pedido se no momento exato em que ele for solicitado ainda esteja dentro do horário do restaurante. Exemplo: Se o restaurante fechar às 22h, e o cliente fizer o pedido às 21h59:59 segundos, o pedido será solicitado e o restaurante terá de atender.
 - Entende-se como pedido efetuado, o momento em que o cliente escolhe forma de pagamento e endereço e clica no botão para criar o pedido. Se o cliente adiciona os produtos no carrinho mas na hora de efetuar o pedido tiver passado do tempo (22h01 usando o nosso exemplo), o pedido será revogado.
 - Para pagamentos feitos no Pix, o sistema fará um pré-pedido, informando ao restaurante que um pedido está pré-processado, só esperando o pagamento. Com um prazo de no máximo 5 minutos, o usuário deve pagar nesse meio-tempo. Passado os 5 minutos sem nenhum pagamento, o pedido é cancelado, não podendo ser refeito caso o horário de funcionamento do restaurante já tenha passado.

### 12. RN-012
<font size=4.5>**Número Identificador:**</font> RN-012
<font size=4>**Nome:**</font> Pagamento por Cartão
<font size=4>**Data de Criação:**</font> 28/04/2025
<font size=4>**Data da Última Atualização:**</font> 28/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
<font size=4>**Dependências:**</font> RN-009 (Criação de um Pedido) RN-010 (Uso do Cupom)
- É necessário apenas informas os dados bancários.
- Tais dados não ficam salvos no sistema diretamente, pela LGPD (Lei Geral de Proteção de Dados) e o PCI-DSS (Payment Card Industry Data Security Standard). Em vez disso, ficamos com um token que contém criptografado as informações do usuário, sendo necessário apenas informar o CVV se o usuário optar por salvar esse token. Caso o usuário preferir poderá sempre informar os dados na hora da compra.
- O pagamento é feito automaticamente na hora do pedido, nunca na hora da entrega.

### 13. RN-013
<font size=4.5>**Número Identificador:**</font> RN-013
<font size=4>**Nome:**</font> Pagamento por Dinheiro
<font size=4>**Data de Criação:**</font> 28/04/2025
<font size=4>**Data da Última Atualização:**</font> 28/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
<font size=4>**Dependências:**</font> RN-009 (Criação de um Pedido)
- Para pagamentos no dinheiro, o restaurante ficará com todos os ganhos na hora. Porém, na hora do Eatly pagar as comissões, o nosso sistema descontará o total de ganhos da porcentagem em dinheiro que receberia caso fosse no cartão.
- Se o restaurante só aceitar dinheiro, ou por alguma coincidência só receber pedidos em dinheiro, o restaurante não receberá comissões do Eatly e ainda terá que pagar a porcentagem dos ganhos que está devendo.
- Caso o exemplo acima se concretize, nosso sistema gerará um boleto ou um pix para receber o pagamento do restaurante que está devendo, tendo um prazo de 10 dias úteis para o pagamento, mediante bloqueio caso não ocorra. Nosso sistema irá relembrar o restaurante do pagamento no dia que o boleto (ou o pix) for gerado, faltando 5 dias para vencer, 2 dias e no dia do vencimento.

### 13. RN-013
<font size=4.5>**Número Identificador:**</font> RN-013
<font size=4>**Nome:**</font> Pagamento por Pix
<font size=4>**Data de Criação:**</font> 28/04/2025
<font size=4>**Data da Última Atualização:**</font> 28/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
<font size=4>**Dependências:**</font>
- Para pagamentos via pix, o nosso sistema gera um QR-Code junto de um Pix Copia e Cola e mostra ao usuário.
- O prazo para o pagamento desse QR-Code é de 10 minutos. Caso o usuário passe disso, o pedido (tanto de comida, quanto de cupom) será cancelado.

### 14. RN-014
<font size=4.5>**Número Identificador:**</font> RN-014
<font size=4>**Nome:**</font> Porcentagem de comissão sobre os restaurantes
<font size=4>**Data de Criação:**</font> 28/04/2025
<font size=4>**Data da Última Atualização:**</font> 28/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
<font size=4>**Dependências:**</font> RN-015(Plano Básico Eatly) e RN-016 (Plano Entrega do Eatly)
- A porcentagem de comissão sobre os restaurantes irá depender do plano que eles assinarem com a Eatly.
- Para restaurantes assinantes do Plano Básico, a comissão será de 10% em cima do faturamento bruto recebido no Eatly. Somado a isso, receberemos uma comissão de 2,8% em cima dos pagamentos feitos no nosso app.
- Para restaurantes assinantes do Plano Entrega, a comissão será de 18% sobre o faturamento bruto gerado no nosso app. Some a isso os mesmos 2,8% sobre os pagamentos realizados no Eatly.

### 15. RN-015
<font size=4.5>**Número Identificador:**</font> RN-015
<font size=4>**Nome:**</font> Plano Básico Eatly
<font size=4>**Data de Criação:**</font> 29/04/2025
<font size=4>**Data da Última Atualização:**</font> 29/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
<font size=4>**Dependências:**</font>
- Com o plano básico o restaurante terá os seguintes benefícios:
	1. Será visível nas pesquisas de restaurantes.
	2. Gestor de pedidos para administrar os pedidos recebidos.
	3. A entrega será feita pelo próprio restaurante (pagará menos comissões).
- Para restaurantes que faturem mais de R$2.000,00 por mês a partir do 2º mês, uma mensalidade de R$130,00 deverá ser paga. Para restaurantes que faturem menos de R$2.000,00, ou que ainda não completaram 2 meses de assinatura, estarão isentos de pagar esta mensalidade.

### 16. RN-016
<font size=4.5>**Número Identificador:**</font> RN-016
<font size=4>**Nome:**</font> Plano Entrega Eatly
<font size=4>**Data de Criação:**</font> 29/04/2025
<font size=4>**Data da Última Atualização:**</font> 29/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
<font size=4>**Dependências:**</font>
- Com o plano entrega o restaurante terá os seguintes benefícios:
	1. Todos os benefícios do Plano Básico.
	2. Entrega realizada pelo Eatly.
	3. Rastreamento da entrega em tempo real.
	4. Suporte do Eatly até o final da entrega.
- Para restaurantes que faturem mais de R$2.000,00 por mês a partir do 2º mês, uma mensalidade de R$150,00 deverá ser paga. Para restaurantes que faturem menos de R$2.000,00, estarão isentos de pagar esta mensalidade.

### 17. RN-017
<font size=4.5>**Número Identificador:**</font> RN-017
<font size=4>**Nome:**</font> Comissões para Motoboys
<font size=4>**Data de Criação:**</font> 29/04/2025
<font size=4>**Data da Última Atualização:**</font> 29/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
<font size=4>**Dependências:**</font>
- Uma taxa fixa de R$5,00 por corrida será dado, para compensar corridas pequenas.
- O preço por quilômetro rodado será de R$3,00 (contando somente a saída do restaurante até o cliente).
- Haverá um adicional de R$8,00 em casos de trânsito ou chuva.

### 18. RN-018
<font size=4.5>**Número Identificador:**</font> RN-018
<font size=4>**Nome:**</font> Autenticação
<font size=4>**Data de Criação:**</font> 29/04/2025
<font size=4>**Data da Última Atualização:**</font> 29/04/2025
<font size=4>**Autor:**</font> João Victor Portela Rocha
<font size=4>**Número da Versão:**</font> 1.0
<font size=4>**Dependências:**</font>
- Nossa autenticação por email e senha será usando o SimpleJWT. Ele fara o trabalho de gerar os tokens e armazená-los para manter o login ativo.
- Para autenticações por *Social Accounts*, como o Google, Facebook e etc, nós usaremos o *dj-rest-auth* junto do *django-allauth*.
