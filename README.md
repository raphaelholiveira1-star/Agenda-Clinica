# Clínica Vitta | Agenda online (projeto de demonstração)

Sistema de agendamento de consultas de uma clínica fictícia, com a tela do paciente e a agenda da recepção. Foi criado para demonstrar como uma clínica pequena pode receber agendamentos sem depender de ligações. Não é uma clínica real e nenhum dado é enviado a lugar nenhum.

## O que o projeto faz

- Escolha da especialidade e do profissional, com o valor da consulta particular
- Datas dos próximos 14 dias, sem domingos, e horários livres por profissional (manhã e tarde, com intervalo de almoço e sábado só de manhã)
- Horários já ocupados aparecem bloqueados, inclusive os que você acabou de agendar
- Formulário com validação, escolha entre particular e convênio e aceite de uso dos dados
- Confirmação com código do agendamento e arquivo para adicionar ao calendário do celular
- Aba **Agenda da clínica**, com todos os agendamentos por dia e opção de cancelar
- Layout pensado para o celular, com tema claro e escuro conforme o aparelho

## Como abrir

1. Baixe ou clone esta pasta.
2. Abra o arquivo `index.html` no navegador.

Não precisa instalar nada. Mantenha o `index.html` e o `style.css` na mesma pasta.

## Como adaptar para um cliente

- **Profissionais, especialidades e valores:** ficam na lista `SP`, no `<script>` do `index.html`.
- **Horários de atendimento:** definidos na lista `T`, no mesmo `<script>`.
- **Nome, endereço e cores:** o nome e o endereço estão no `index.html`, e as cores no começo do `style.css`.

## Tecnologias

HTML, CSS e JavaScript puros, sem bibliotecas. Os agendamentos ficam salvos no navegador (`localStorage`).

## Como seria em um projeto real

Nesta versão os horários ocupados de exemplo são simulados e os agendamentos existem só no navegador de quem os fez. Em um projeto de verdade, tudo ficaria em um banco de dados, a recepção teria login próprio, e os lembretes seriam enviados de fato por WhatsApp e e-mail. Como envolve dados de saúde, também seria preciso seguir a LGPD, com política de privacidade e armazenamento seguro.
