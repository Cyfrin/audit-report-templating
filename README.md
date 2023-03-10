# How to generate a PDF audit report

<br/>
<p align="center">
<a href="https://cyfrin.io" target="_blank">
<img src="./report-image.png" width="400" alt="Chainlink Brownie logo">
</a>
</p>
<br/>


1. Add all your findings to a markdown file like `report-example.md`
   1. Add the metadata you see at the top of that file
2. Install [pandoc](https://pandoc.org/installing.html)
3. Download `eisvogel.latex` and add to your templates directory (should be `~/.pandoc/templates/`)
4. Add your logo to the directory as a pdf named `logo.pdf`
5. Run this command:
```
pandoc report-example.md -o report.pdf --from markdown --template=eisvogel --listings
```
