# Mensagens Conventinais de Compromisso

Usar uma `git commit` convenção para nossas mensagens git nos ajuda a que todas as mensagens dos contribuidores tenham uma aparência homogênea.

Além disso, como vamos usar o mesmo padrão para todas as mensagens git, podemos usá-lo para fazer coisas extras, como, por exemplo, classificar os commits corretamente `CHANGELOG.md` ou determinar qual é a próxima versão a ser lançada com base no histórico de commits .

Para garantir que todas as mensagens git sigam o mesmo padrão, vamos usar o commitlint para lintar as mensagens git.

## Formatos de confirmação

<pre>
<b><a href="#types">&lt;tipo&gt;</a></b></font>(<b><a href="#scopes">&lt;escopo opcional&gt;</a></b>): <b><a href="#subject">&lt;assunto&gt;</a></b>
<sub>linha separadora vazia </sub>
<b><a href="#body">&lt;copo opcional&gt;</a></b>
<sub>linha separadora vazia</sub>
<b><a href="#footer">&lt;rodapé opcional&gt;</a></b>
</pre>

De modo simples é isso :

```
Tipo(escopo, se quiser colocar): assunto 
```
>PS.: Escreva sempre em inglês. 

### Escopo

O `escopo` fornece informações contextuais adicionais.

- É uma parte opcional do formato. 
- Os escopos permitidos dependem do projeto específico. 
- Não use identificadores de problemas como escopos. 

### Assunto

O `assunto` contém uma descrição sucinta da mudança.

- É uma parte obrigatória do formato. 
- Use o tempo presente imperativo: "mudar" e não "mudar" nem "mudar".
- Não coloque a primeira letra em maiúscula. 
- Sem ponto (.) No final. 

A mensagem git deve ter um _*tipo*_. Poderia ser:

- `build`: Mudanças que afetam o sistema de build ou como ferramenta de compilação, pipeline ci, dependências, versão do projeto,...
- `ci`: Mudanças em nossos arquivos e scripts de configuração de CI.
- `docs`: Alterações apenas na documentação.
- `feat`: um novo recurso.
- `fix`: uma correção de bug.
- `perf`: uma mudança de código que melhora o desempenho.
- `refactor`: uma alteração de código que não corrige um bug nem adiciona um recurso.
- `style`: alterações que não afetam o significado do código.
- `test`: Adicionando testes ausentes ou corrigindo testes existentes. 
- `ops`: Compromissos, que afetam componentes operacionais como infraestrutura, implantação, backup, recuperação, ...
- `chore`: Atualização de tarefas grunhidas etc; sem alteração do código de produção. 

## Exemplos:
Os exemplos a seguir são feitos com a sua forma em inglês e o assunto em português-BR em parênteses () 

* ```
build: update dependencies(atualiza dependências)
```

* ```
ci: setup travis credentials(configura credenciais travis) 
```

* ```
refactor: move scripts(move scripts) 
```

* ```
fix: use user agent provided by parameters(usa o agente do usuário fornecido por parâmetros) 
```

* ```
test: update snapshots(atualizações instantâneas) 
```

* ```
style: use space instead of tabs(usa espaço em vez de guias)
```

* ```
feat(shopping cart): add the amazing button(adiciona botão incrível)
```

* ```
feat(lang): add polish language
```

* ```
build: release version 1.0.0 -> para versões no github.
```

* ```
docs: correct spelling of CHANGELOG(ortografia correta de CHANGELOG) 
```

* ```
fix: correct minor typos in code (corrige pequenos erros de digitação no código) 

see the issue for details on typos fixed.(veja o ticket para detalhes sobre os erros de digitação corrigidos) 

Reviewed-by: Carlosvitr (Revisado por: Carlosvitr) 
Refs #133
```
