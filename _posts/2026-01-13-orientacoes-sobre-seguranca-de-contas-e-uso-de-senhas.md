---
layout: post
title: Orientações sobre Segurança de Contas e Uso de Senhas
---

No exercício de nossas funções públicas, a proteção das informações municipais é uma prioridade estratégica. Este documento apresenta orientações para a criação e manutenção de credenciais de acesso seguras.

## Introdução

A autorização é o processo de verificar se o usuário é, de fato, quem possui permissão para acessar determinada conta. Nossos nomes de usuário e senhas são as ferramentas fundamentais que atestam essa identidade. O processo de autenticação consiste em fornecer uma prova de acesso para receber a devida permissão.

## Tipos de Ataque

Os adversários utilizam diversos métodos para comprometer credenciais:

- Ataques de Força Bruta e Dicionário: Consistem no uso de listas extensas de palavras e combinações para adivinhar a senha por tentativa e erro. Se a senha for curta, o tempo para a descoberta é drasticamente reduzido.
- Credential Stuffing: Ocorre quando atacantes utilizam listas de senhas vazadas de outros sites para tentar acessar contas diferentes do mesmo usuário.
- Phishing e Engenharia Social: Técnicas de manipulação psicológica onde o atacante se passa por uma entidade confiável (como um site falso de login) para induzir o servidor a entregar seus dados.
- Keylogging: Instalação de software malicioso para registrar todas as teclas digitadas no computador.
- Shoulder Surfing: A observação direta de alguém digitando a senha, o famoso "olhar por cima do ombro".

## Defesas

A principal defesa é elevar o "custo" do ataque em termos de tempo.

- Complexidade: Utilizar uma combinação de letras maiúsculas, minúsculas, números e pontuação aumenta exponencialmente as combinações possíveis, tornando o ataque de força bruta inviável.
- Diretrizes do NIST: O _National Institute of Standards and Technology_ recomenda senhas de, pelo menos, oito caracteres, permitindo todos os caracteres ASCII e símbolos Unicode.
- Autenticação de Múltiplos Fatores (MFA/2FA): Adiciona camadas de segurança baseadas em algo que você sabe (senha), algo que você possui (dispositivo ou token) ou algo que você é (biometria). Recomenda-se o uso de aplicativos de autenticação em vez de SMS, que é vulnerável a clonagem de SIM.

## Exemplo de Criação de Senhas

Uma boa senha deve ser difícil de descobrir, mas memorizável. Algumas técnicas incluem:

- Palavras Inventadas: Criar termos que não existem no dicionário (ex: "fletuciladamente"), o que facilita a memorização por serem pronunciáveis, mas dificulta ataques automatizados.
- Mistura de Caracteres: Substituir letras por números ou símbolos (ex: trocar 'E' por '3'), embora esta técnica isolada não seja infalível contra ataques sofisticados.

## Memorização de Senhas

O processo de memorização é pessoal e exige autoconhecimento. Anotar senhas é uma prática controversa; se for necessário fazê-lo durante o processo de aprendizado, o papel deve ser destruído assim que a senha for decorada. O uso de frases ou associações de ideias, mesmo com palavras sem significado, pode auxiliar na retenção mental.

## Compartilhamento e Gerenciamento de Senhas

A reutilização de senhas deve ser evitada ao máximo para conter danos em caso de vazamento, seguindo o princípio da compartimentalização.

### Gerenciadores de Senhas

Softwares que armazenam senhas complexas em um banco de dados criptografado, protegido por uma única "senha mestre". Eles permitem que o servidor utilize senhas únicas e aleatórias para cada serviço sem a necessidade de memorizá-las individualmente.

**A utilização de gerenciadores de senhas é a prática recomendada pelo Departamento de Tecnologia e Inovação**. Assim é possível minimizar o número de senhas sem perda significativa de segurança.

Exemplo de utilização de aplicativo de gerenciamento de senha:

1. Senha para ligar e usar um computador com armazenamento criptografado;
2. Senha para destravar o gerenciador de senhas do computador;
3. Senha para ligar e usar telefone móvel com armazenamento criptografado;
4. Senha do banco para realizar operações financeiras sem precisar consultar nenhum dispositivo;

Essa pessoa precisa memorizar apenas 4 senhas. O inconveniente é que ela precisará ter acesso ao gerenciador de senhas para ter acesso as demais senhas.

Além disso, **é recomentado o backup da base de dados do gerenciador de senhas.**

Recomentações de aplicativos gerenciadores de senhas de código livre:

- [KeePass Password Safe](https://keepass.info/)
- [Bitwarden](https://bitwarden.com/)

## Digitando Senhas

No momento da digitação, alguns cuidados são essenciais:

- Certifique-se de que as teclas Caps Lock ou Num Lock não estão ativadas indevidamente.
- Aguarde o campo de senha carregar totalmente para evitar que os caracteres apareçam em texto claro na tela.
- Em locais públicos, proteja a visão do teclado e das mãos para evitar o shoulder surfing

## Limite da Confiabilidade

É fundamental compreender que nenhuma senha garante inviolabilidade absoluta. Senhas podem ser descobertas por falhas de protocolo, implementação ou até mesmo por coação física em casos extremos. A consciência do servidor sobre o valor dos dados que manipula é a camada de segurança mais importante da administração pública.

## Referencias

- [Guia da Autodefesa Digital](https://guia.autodefesa.org/)
- [CS50’s Introduction to Cybersecurity Lecture 1](https://cs50.harvard.edu/cybersecurity/notes/0/)
