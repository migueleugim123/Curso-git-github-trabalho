# Registro do conflito resolvido

## Objetivo

Foi criado um conflito controlado para demonstrar o processo de identificação e resolução de conflitos no Git.

## Situação criada

A mesma linha do README foi alterada em duas branches diferentes.

### Versão da main

```text
Este guia apresenta HTML para iniciantes.
```

### Versão da branch

```text
Este guia apresenta HTML de forma simples para iniciantes.
```

Ao tentar integrar as alterações, o Git identificou que as duas versões modificavam o mesmo trecho.

## Marcadores de conflito

O Git pode apresentar algo semelhante a:

```text
<<<<<<< HEAD
Este guia apresenta HTML para iniciantes.
=======
Este guia apresenta HTML de forma simples para iniciantes.
>>>>>>> feature/secao-01
```

## Resolução

Foi escolhida uma versão coerente, combinando as informações sem manter os marcadores:

```text
Este guia apresenta HTML de forma simples e sequencial para iniciantes.
```

Depois da edição, o arquivo foi salvo e o conflito foi marcado como resolvido.

## Comandos utilizados

```bash
git status
git add README.md
git commit -m "fix: resolve conflito no README"
```

## Resultado

O conflito foi resolvido manualmente e o conteúdo final ficou consistente. O processo foi registrado neste arquivo para servir como evidência da atividade.
