
# Comandos: 

# Busca / Informação de diretórios e arquivos.

- `Find:` Busca avançada por metadados. 
     - `-type f:` apenas arquivos.
     - `-size (tamanho)c:` tamanho exato em bytes.
     - `-user / -group:` filtra pelo dono do arquivo.
- `File:` Busca a verdadeira natureza do arquivo, revelando se é binário, texto, compactado, etc.

# Filtros e Tratamento de Texto

- `Strings:` Busca apenas o que é legível para humanos em um arquivo de texto.
- `tr:` Traduz ou substitui caracteres, um por um, usado pra quebrar cifras, como ROT13.

# Codificação ou engenharia reversa

- `base64 -d:` Desencripta um arquivo que esteja em base64
- `xxd:` Manipula hexdumps. a flag `-r` (reverse) reconstrói um arquivo binário. 

# Compressão de arquivos

- `gizp -` / `bzip2 -d:`  Descompactam arquivos, exigem que os mesmos terminem em .gz ou .bz2, respectivamente.
-  `tar -xf:` Extrai arquivos .tar.

# Privilégios

- `2>/dev/null:` Silencia mensagens de permissão negada.