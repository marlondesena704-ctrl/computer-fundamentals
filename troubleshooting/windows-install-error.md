# Erro ao instalar Windows

## Vídeo 36 — Windows não pode ser instalado nesta unidade

Erro causado por incompatibilidade entre:

- modo de boot (UEFI ou Legacy)
- tipo de partição (GPT ou MBR)

Solução usando diskpart:

diskpart
list disk
select disk 0
clean
convert mbr
exit
