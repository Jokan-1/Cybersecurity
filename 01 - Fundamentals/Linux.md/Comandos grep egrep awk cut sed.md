# What I learned?

**Answer:** Comandos de otimização de tempo para utilizar no terminal do linux.

# **Comandos:**
- `grep [word/dir] <dir/file>` : Serve para buscar a palavra ou diretório selecionado em um diretório qualquer.
- `grep -v [word] <dir/file>`: Excluirá a palavra selecionada do resultado.
-  `egrep "[word/dir1]|[word/dir2]" <dir/file>`: Ao usar o operador `pipe: |` , pode-se buscar por mais termos ou diretório.
- `awk -F : '{print $1}' <dir/file>`: Este em específico retornará apenas a primeira coluna do diretório selecionado, se , o mesmo, for dividido entre : , a flag `-F` é de Field, campo.
- `awk -F : '{print $1}' <dir/file> > <dir/file2>`: Criará um novo arquivo com o conteúdo selecionado.
- `cut -d : -f1 <dir/file>`: Possui a mesma função que o `awk` , porém mais limitado.
- `sed 's/antigo/novo/' <dir/file>`: Editor simples na qual o comando selecionado substituirá a palavra "antigo" por "novo" neste exemplo em específico no diretório/arquivo selecionado. 
- `sed 's/antigo/novo/' <dir/file> > <dir/file2>`: Criará um novo arquivo com o conteúdo selecionado.

# Observações:
- Em certas ocasiões, usar " " ao utilizar o grep ou o egrep evitará com que o sistema não identifique o pedido, exemplo: `egrep root|desec /etc/passwd`: o sistema não conseguirá compreender o que se pede por conta do pipe |. Forma correta: `egrep "root|desec" /etc/passwd`.
- Para que o `egrep` funcione com exatidão, ponha o diretório a ser vasculhado logo após o primeiro comando: `egrep "palavra1" <dir/file> | grep "palavra2"`.