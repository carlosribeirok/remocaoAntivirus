# :space_invader: Remoção do McAfee

Acesse o CMD da Máquina em Execução
```sh
psexec -s -e -h \\10.16.26.24 cmd
```
Navegue para o Diretório do McAfee e Consulte os Arquivos da Pasta Agent
```sh
cd c:\program files\mcafee && dir
```
[ Deve existir apenas a pasta Agent ]

Acesse a Pasta x86 e Remova o Agent
```sh
cd agent\x86 && FrmInst.exe /forceuninstall
```
[ Espere aparecer uma extensa página de comandos ]

Volte para o Diretório c:\Program Files e Exclua a Pasta McAfee
```sh
cd c:\Program Files && rmdir /s .\mcafee
```
[ Será necessário confirmar a exclusão da pasta ]

Navegue para o Diretório c:\programdata e Exclua a Pasta McAfee
```sh
cd c:\programdata && rmdir /s .\mcafee
```
[ Será necessário confirmar a exclusão da pasta ]

## ✔️ Agent Removido com Sucesso

README construído com o ❤️ por [Carlos]. 

[Carlos]: <https://github.com/carlosribeirok>



