# ultrashield-cossignatario-p3

Cossignatario independente do batimento do UltraShield. Segura UMA parte (a 3) da chave FROST 2-de-3 e cossigna, a cada epoca de 5 min, a mesma cadeia que as demais partes assinam.
So cossigna: nunca propoe. Recusa qualquer proposta cujo codigo, cabeca da trilha ou sondas nao confiram.

- O codigo aqui e o empacotado de `cossignatario.mjs` (fonte no repositorio do UltraShield).
- Os segredos (`PARTE_SELADA`, `PARTE_SENHA`, `DATABASE_URL`) ficam nos GitHub Secrets. O papel de banco `cossig_p3` so le e cossigna batimentos.
- O agendamento do GitHub e "melhor esforco": a disponibilidade nao e garantida.
