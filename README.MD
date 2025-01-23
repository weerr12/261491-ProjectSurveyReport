# ก่อนจะเริ่มใช้
1.ติดตั้ง LaTeX Distribution
    Windows: MikTeX
    MacOS: TeXLive
2.ติดตั้งภาษา Perl

คลิปสอน https://www.youtube.com/watch?v=4lyHIQl4VM8

# ติดตั้ง Packgage พวกนี้ด้วย
คำสั่งบน Windows
    miktex packages require latexmk fonts-tlwg fonts-arundina tex-gyre tex-gyre-math

จากนั้นไปที่
    File > Preferences > Settings แล้วพิมพ์ settings.json
    วางไฟล์นี้ลงไปตรงไหนก็ได้
    
    "latex-workshop.latex.tools": [
      {
        "name": "latexmk",
        "command": "latexmk",
        "args": [
          "-pdfxe",
          "-synctex=1",
          "-interaction=nonstopmode",
          "-file-line-error",
          "%DOC%"
        ]
      }
    ]