Neste diretório serão armazenados os documentos solicitados ao longo do projeto. 

Para compilar os arquivos markdown em PDF você pode utilizar o seguinte comando: 

```bash
pandoc --bibliography referencias.bib -N --variable "geometry=margin=1.2in" --variable fontsize=12pt relatorio_final.md --pdf-engine=xelatex --toc -o relatorio_final.pdf
```
