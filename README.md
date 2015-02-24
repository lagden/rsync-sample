rsync-sample
============

Neste exemplo, o `rsync` copiará todos os arquivos, diretórios e subdiretórios da pasta `source`, que corresponderem ao `pattern` do arquivo `dest/include.rsync`, para a pasta `dest`.

## Propósito

O propósito é apenas sincronizar alguns arquivos e pasta para o destino com mais agilidade, evitando que sobrescreva arquivos ou pastas não desejadas.

## Uso

    git clone https://github.com/lagden/rsync-sample.git sample
    cd sample/dest
    bin/sync
    
## Bastidores

O `rsync` da seguinte maneira:
    
    rsync SOURCE DEST -rav --include-from include.rsync --exclude-from exclude.rsync
    
1. Ele irá ignorar todos os arquivos e pasta. Ver `pattern` no `exclude.rsync`
2. Depois incluirá apenas os arquivos e pastas definidos no `include.rsync`

Bem simples!! Assim você terá apenas os arquivos e pastas.


## Contributors

[Thiago Lagden](https://github.com/lagden)
