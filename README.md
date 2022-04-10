# :space_invader: Remoção do McAfee

Acesse o CMD da Máquina em Execução
```sh
psexec -s -e -h \\10.16.26.24 cmd
```
Navegue para o Diretório do McAfee
```sh
cd c:\program files\mcafee
```
Consulte os Arquivos da Pasta Agent
```sh
dir
```
[ Deve existir apenas a pasta Agent ]

Acesse a Pasta x86
```sh
cd agent\x86
```
Remova o Agent
```sh
FrmInst.exe /forceuninstall
```
[ Espere aparecer uma extensa página de comandos ]

```sh
enter
```

Volte para o Diretório c:\Program Files
```sh
cd c:\Program Files
```
Exclua a Pasta McAfee
```sh
rmdir /s .\mcafee
```
[ Será necessário confirmar a exclusão da pasta ]

Navegue para o Diretório c:\programdata
```sh
cd c:\programdata
```
Exclua a Pasta McAfee
```sh
rmdir /s .\mcafee
```
[ Será necessário confirmar a exclusão da pasta ]

## ✔️ Agent Removido com Sucesso

README construído com o ❤️ por [Carlos]. 

[Carlos]: <https://github.com/carlosribeirok>



