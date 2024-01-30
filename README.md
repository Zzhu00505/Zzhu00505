Сообщение для себя
19.11.2023

405 kB

6:34 PM

363 kB

6:34 PM

412 kB

6:34 PM

376 kB

+15
01.12.2023

358 kB

7:22 PM

333 kB

7:22 PM
СЕГОДНЯ
from pptx import Presentation

# Создание новой презентации
prs = Presentation()

# Добавление заголовочного слайда
slide_1 = prs.slides.add_slide(prs.slide_layouts[0])
title = slide_1.shapes.title
subtitle = slide_1.placeholders[1]
title.text = "Абай жолы 2 том"
subtitle.text = "Презентация по истории и творчеству"

# Добавление слайда с текстом
slide_2 = prs.slides.add_slide(prs.slide_layouts[1])
title = slide_2.shapes.title
content = slide_2.placeholders[1]
title.text = "Биография Абая"
content.text = "Здесь вы можете добавить текст с биографией Абая"

# Добавление слайда с изображением
slide_3 = prs.slides.add_slide(prs.slide_layouts[5])
title = slide_3.shapes.title
title.text = "Природа в произведениях Абая"
img_path = "путь_к_изображению.jpg"
left = top = 0
slide_3.shapes.add_picture(img_path, left, top)

# Сохранение презентации в файл
prs.save("абай_жолы_2_том.pptx")
