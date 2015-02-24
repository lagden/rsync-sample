rsync-sample
============

Neste exemplo, o `rsync` copiará todos os arquivos, diretórios e subdiretórios da pasta `source`, que corresponderem ao `pattern` do arquivo `dest/include.rsync`, para a pasta `dest`.

## Propósito

O propósito é copiar alguns arquivos e pasta para o destino com mais agilidade, evitando que sobrescreva arquivos ou pastas não desejadas.

## Uso

    git clone https://github.com/lagden/rsync-sample.git sample
    cd sample/dest
    bin/sync

## Contributors

[Thiago Lagden](https://github.com/lagden)
