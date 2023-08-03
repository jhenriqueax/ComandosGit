# ComandosGit


# Retornar um Commit Após o Push

Este é um guia para retornar a um commit anterior após o push usando o Git. Siga os passos abaixo:

1. Execute o comando `git log` para visualizar o histórico de commits no seu repositório local. Anote o hash do commit anterior ao qual você deseja retornar.

    ```
    git log
    ```

2. Utilize o comando `git reset --hard <hash_do_commit_anterior>` para voltar ao commit desejado. Certifique-se de substituir `<hash_do_commit_anterior>` pelo hash anotado no passo anterior. Tenha em mente que esse comando descarta todos os commits feitos após o commit desejado.

    ```
     git reset --hard <hash_do_commit_anterior>
    ```

3. Verifique o status do seu repositório usando o comando `git status`. Isso ajudará a confirmar se a operação foi bem-sucedida e se o seu repositório está no estado desejado.

     ```
     git status
     ```

4. Faça o push das alterações para o repositório remoto utilizando o comando `git push origin --force`. O uso da opção `--force` é necessário para substituir o histórico existente pelo novo histórico resultante do reset. Certifique-se de substituir `origin` pelo nome remoto adequado, caso necessário.

    ```
     git push origin --force
    ```

Lembre-se de que o uso do `--force` ao fazer push pode causar problemas para outras pessoas colaborando no mesmo repositório, pois essa operação reescreve o histórico do repositório. Portanto, tenha cuidado ao executar esse comando e comunique-se com sua equipe, se necessário.

------------------------------------------------------------------------------------------------------------------------

# NEW

```
git checkout <nome_da_branch> -- <arquivo> 
```

