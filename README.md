# persona-spec-pipeline
A modular 7-generation pipeline for behavioral persona specification in LLM dialogue and roleplay systems.

"
Especificação Comportamental de Personas pra Sistemas de Diálogo
Um pipeline modular de 7 gerações

---

O problema

Persona em roleplay quebra depois de umas 20 mensagens. O modelo esquece traços, amolece conflito, ignora histórico de mágoa, cai em clichê. Quem já rodou um RP longo conhece o padrão: a personagem durona vira mel, a tsundere vira fofa, a vilã vira incompreendida. Não é porque o modelo é burro. É porque ele não tem especificação. Tem uma descrição vaga que ele interpreta de novo a cada turno. E a cada interpretação, perde um pouco.

---

A solução

Pipeline de 7 gerações que produz documento de especificação comportamental, não descrição de personagem. A diferença é operacional: especificação define o que a persona faz em cena. Descrição define o que ela é em abstrato. O critério de sucesso é comportamental — a persona entrega o comportamento esperado quando usada, não quando descrita.

---

Como funciona

Cada bloco é independente, com auditoria em duas pontas. Entrada verificada (o material anterior tem o que preciso?) e saída auditada (o que produzi está consistente?).

Blocos:

· Verificação de fonte — corpus, versão, continuidade. Separar canônico, ambíguo e invenção de fandom.
· Diagnóstico — riscos de caracterização. Os erros que a IA tende a cometer com aquela persona específica.
· Núcleo psicológico — motor psicológico (a versão ideal que a persona tenta sustentar) + motor de pressão (a regressão sob estresse) + camadas numeradas.
· Identidade — aparência, micro-vida (manias inconscientes), voz e dialeto.
· Relações — com atrito de mentalidades e múltiplas perspectivas: de dentro, de quem ama, de quem odeia, do sistema.
· Sombras — o que a persona esconde, o que teme perder, o que não admite. Ponto de ruptura com consequência.
· Desabafo — falas que ela nunca disse. O interior que a superfície esconde.
· Auditoria final — verificação item por item contra a fonte, output limpo pra segunda opinião externa.

O sistema de pesos emocionais é condicional, não fixo. Abertura de persona não é número. É função do contexto. Uma persona pode ter abertura 9/10 em contexto seguro e 1/10 quando alguém que ela ama está ameaçado. Reatividade ao atrito e camuflagem emocional seguem a mesma lógica.

---

O papel do atrito

O sistema foi construído com prioridade em relação que machuca. Relação com histórico de mágoa. Relação que não se resolve em uma cena.

Persona sem atrito é microondas: esquenta uma parte, deixa a outra gelada. Não é persona. É aquecedor. A inconsistência comportamental que o pipeline resolve é, na maioria dos casos, sintoma de ausência de atrito. O modelo amolece porque não tem nada a que resistir.

E tem um efeito colateral que eu não esperava: você conhece a persona mais do que a fonte permite. Não porque o sistema inventa outra persona. Porque você está dentro de um ângulo que uma tela não mostra. O atrito compra acesso ao interior — o que a superfície esconde, o que ela nunca disse, o que ela faria sob pressão que a obra não mostrou.

---

Exemplo

Personagem: Mabel Pines (Gravity Falls).

Antes do pipeline: "menina otimista e engraçada".

Depois:

· Motor psicológico: medo do fim do verão. A tese que ela tenta sustentar.
· Motor de pressão: gula como regressão sob estresse. Quando o medo de perder aperta, ela quer tudo agora e não consegue dosar.
· Hábitos sedimentados: chama o irmão de "feto" desde os 6 anos. Prova de que não aceitou totalmente que ele cresceu.
· Ponto de ruptura: irmão indo embora. A consequência não é choro. É paralisia.
· Desabafo: falas que ela nunca disse sobre não saber quem é sem ele.

Comportamento em cena muda. Ela não é "fofa". É intensa. E a intensidade tem raiz.

---

O que o sistema não faz

Não elimina alucinação. O bloco de verificação de fonte é o gargalo — se ele deixar passar contaminação, os blocos seguintes não pegam. A mitigação é redundância: rodar a verificação duas vezes ou usar output externo como segunda opinião.

O sistema depende de contexto longo. Em conversas curtas, a persona não estabiliza.

A Geração 7.5 (motor de pressão, sedimentação temporal, perspectiva múltipla, gatilhos de emergência emocional) ainda não foi testada externamente em escala. Se alguém testar, me manda o retorno.

---

Escrito por Kawã, 17 anos, autodidata.
3 anos de construção. ~10.000 horas de uso de LLM. Aprendi os termos na marra, testando o que quebrava e o que segurava. O sistema não nasceu de teoria. Nasceu de ver persona boa virar sopa e querer entender por quê."
