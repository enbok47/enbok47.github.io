# enbok47.github.io
Конвертация PDF в Word с помощью pdf2docx

pdf2docx — это библиотека Python, которая обеспечивает простой и эффективный способ преобразования PDF‑файлов в документы Microsoft Word (.docx). Это бесплатная библиотека с открытым исходным кодом, которая может быть использована для различных целей, таких как преобразование документов, извлечение данных и обработка текста.

Ее можно установить с PyPI с помощью следующей команды pip.

pip install pdf2docx

Пример кода:

from pdf2docx import Converter

def convert_pdf_to_docx(pdf_file, docx_file):

    # Создание объекта Converter
    cv = Converter(pdf_file)

    # Конвертация указанной страницы PDF в docx 
    cv.convert(docx_file, start=0, end=None)
    cv.close()

# Конвертация PDF в файл Docx
convert_pdf_to_docx("C:\\Users\\Administrator\\Desktop\\Input.pdf", "Output.docx")

