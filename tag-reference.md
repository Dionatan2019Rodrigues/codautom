# Tag Reference

Este arquivo reúne as tags de variáveis atualmente utilizadas pelo sistema para preencher documentos Word e pelos campos do formulário.

## 1) Tags obrigatórias nos templates Word

Estas são as tags que o sistema usa de forma direta nos documentos Word e que devem estar presentes nos templates principais e individuais:

### Tags globais obrigatórias

- `data_atual`
- `nome_projeto`
- `titulo_projeto`
- `n_projeto`
- `classificacao`
- `instrumento_completo`
- `texto_empresas`
- `nome_coord`
- `siape_coord`
- `nome_fiscal`
- `siape_fiscal`
- `nome_coord_adm`
- `siape_adm`
- `membros`
- `objetivos`
- `metas`
- `justificativa`
- `resultados`
- `importancia_projeto`
- `justificativa_fund`
- `diretor_unidade`
- `siape_diretor`
- `sigla_fundacao`

### Tags por participante / membro obrigatórias

- `participante`
- `nome`
- `siape`
- `cargo`
- `ch_dentro`
- `ch_fora`
- `chefia_imediata`
- `nome_chefia`
- `siape_chefia`

## 2) Campos do formulário que alimentam as tags

Os campos visíveis no formulário e que preenchem esse contexto são:

### Dados gerais do projeto
- `tipo_processo`
- `fundacao_correta`
- `fund_sigla`
- `tit_proj`
- `n_proj`
- `resumo`
- `objetivos`
- `justificativa`
- `importancia`
- `justificativa_fund`
- `diretor_unidade`
- `siape_diretor`
- `data_termino_edit`
- `instrumento_juridico_edit`
- `resultados`
- `metas`

### Coordenadores e fiscais
- `c_g_n`
- `c_g_s`
- `f_nome`
- `f_siape`
- `nome_coord_adm`
- `siape_coord_adm`

### Empresas / instituições
- `num_empresas`
- `nome_emp` (para cada item da lista de empresas)

### Tabela de equipe
- `Nome`
- `SIAPE`
- `Vínculo`
- `Lotação`
- `Função`
- `CH_D`
- `CH_F`
- `Bolsa`
- `Início`
- `Término`
- `Chefia Imediata`
- `SIAPE Chefia`

## 3) Observação importante

A fonte real de verdade para as tags do Word está no dicionário `ctx_global` e no dicionário por membro `ctx_membro`, construído em [codautom.py](codautom.py#L572-L594) e [main.py](main.py#L107-L168).

Esses nomes são os que realmente devem ser usados nos templates `.docx` para renderização correta.

