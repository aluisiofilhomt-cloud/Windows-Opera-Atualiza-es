# Windows Opera 1.8 — Sistema completo (ISO para instalar do zero)

O GitHub não deixa um arquivo passar de 100 MB, então o ISO (2,6 GB) foi dividido em 27 partes
(`WindowsOpera-1.8.iso.000` até `.026`). Baixe **todas** as partes desta pasta e junte-as.

## Juntar as partes

**Windows** (Prompt de Comando, na pasta onde baixou as partes):
```
copy /b WindowsOpera-1.8.iso.??? WindowsOpera-1.8.iso
```

**Linux ou Mac** (Terminal):
```
cat WindowsOpera-1.8.iso.0?? > WindowsOpera-1.8.iso
```

Isso gera o arquivo final **`WindowsOpera-1.8.iso`**.

## Conferir se deu certo (opcional)
O SHA-256 do `WindowsOpera-1.8.iso` deve ser:
```
ef089ef20112a4c9bbeb41a9cf13d5edd3f9b25785a2cf265399ec4e0d121aca
```
No Windows: `certutil -hashfile WindowsOpera-1.8.iso SHA256`
No Linux/Mac: `sha256sum WindowsOpera-1.8.iso`

## Como instalar
1. No VirtualBox, crie uma máquina nova (Tipo: Linux, Versão: Ubuntu 64-bit), com 2 GB de RAM ou mais e um disco de 15 GB ou mais.
2. Nas configurações da máquina, em Armazenamento, aponte o leitor óptico para o `WindowsOpera-1.8.iso`.
3. Ligue a máquina e siga a instalação do Windows Opera.

Também funciona no VMware, no QEMU ou gravado num pendrive/DVD para instalar num PC de verdade.
