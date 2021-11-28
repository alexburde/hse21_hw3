# hse21_hw3
# Проверка качества чтений из fastQC: сравнительная статистика из multiQC
![image](https://user-images.githubusercontent.com/93148620/143721798-f0c93152-5c8a-458e-9e67-368a14d39010.png)
![image](https://user-images.githubusercontent.com/93148620/143721804-711cb668-cb23-4029-a4e4-d61c852e2025.png)
![image](https://user-images.githubusercontent.com/93148620/143721811-03e6b3a9-b42f-4625-a562-9e77c83db712.png)
![image](https://user-images.githubusercontent.com/93148620/143721819-46a0ee70-f5e4-42a0-bf60-6333b071ea33.png)
![image](https://user-images.githubusercontent.com/93148620/143721831-80c04969-e14d-4982-9532-a6761943d6b7.png)
![image](https://user-images.githubusercontent.com/93148620/143721836-53d48426-b321-4a65-b826-7fd8b30735d6.png)
![image](https://user-images.githubusercontent.com/93148620/143721846-601f6175-484d-493e-8d67-d2581e7bb1b9.png)
# Суммарная статистика
![image](https://user-images.githubusercontent.com/93148620/143721863-84deea0e-cd18-483a-b461-1ad14456d002.png)
# Количество уникально картированных чтений по каждому образцу:
![image](https://user-images.githubusercontent.com/93148620/143721936-299c91fa-f151-4800-933c-07e357b01b2e.png)
![image](https://user-images.githubusercontent.com/93148620/143721941-11c4b113-9e20-473a-b7f7-e138b8e7674e.png)
# Смотрим статистику HTSeq и узнаем, количество чтений соответствует участкам генома, где не аннотировано ни одного экзона и количество чтений, которые могут принадлежать разным генам
![image](https://user-images.githubusercontent.com/93148620/143721964-75541aeb-af71-48ce-a1c1-841118557c44.png)
![image](https://user-images.githubusercontent.com/93148620/143721968-a549d3f7-258f-4feb-b47e-540ae660a97d.png)
С помощью данных, приведенных выше, можно посчитать количество чтений, соответствующих хотя бы одному гену
![image](https://user-images.githubusercontent.com/93148620/143721984-232382bc-4c1d-4c01-966a-63c3cf74218e.png)
![image](https://user-images.githubusercontent.com/93148620/143721989-dc4c91c3-73e4-4ce4-8b37-c81c2f223b3b.png)
# Наглядная статистика по каждому из 6 образцов
# Объединяем файлы с прочтениями в один - all_counts (столбцы - образцы, при чем c1, c2, c3 - контрольные образцы; r1, r2, r3 - перепрограммированные образцы)
![image](https://user-images.githubusercontent.com/93148620/143722013-8addb18e-d593-48dd-9232-628e31849eb3.png)
# Часть 2. Анализ с помощью DESeq2
# MA-plot, показывающий Log2FC для генов
Можно заметить, что большее количество дифференциально экспрессированных генов увеличило свою
![image](https://user-images.githubusercontent.com/93148620/143723912-17bffe3a-97e3-4cd4-9551-17567061fc95.png)
# Heatmap, показывающий созависимость экспрессии генов из контрольных и репрограммированных образцов
Можно заметить, что экспрессия генов одинакова в одной группе образцов и отличается между группами
![image](https://user-images.githubusercontent.com/93148620/143723933-1963e117-0597-42c6-951e-855c1699b2f7.png)
# Heatmap для первых 20 наиболее дифференциально экспрессированных генов
![image](https://user-images.githubusercontent.com/93148620/143723951-62f020b6-80b2-42a8-a6ff-79baa558ce08.png)
# Графики со значениями "Normalized counts" в контрольных и перепрограммированных образцах
(поиск генов производился сортировкой по L2FC - ноутбук в папке src)
![image](https://user-images.githubusercontent.com/93148620/143723975-918a4953-5c58-4603-af02-137c08b384e3.png)

![image](https://user-images.githubusercontent.com/93148620/143723981-b91d09ed-427b-4152-a70f-e77474089d02.png)

![image](https://user-images.githubusercontent.com/93148620/143723986-7214b12e-d54b-479c-9fe4-151d5abb792b.png)

![image](https://user-images.githubusercontent.com/93148620/143723995-98ce6222-ddb9-44ff-b71f-8522f2666f47.png)

![image](https://user-images.githubusercontent.com/93148620/143724007-dd3dc269-ba3f-467b-9ede-a3dc0d670819.png)

![image](https://user-images.githubusercontent.com/93148620/143724009-bf2d5b1c-6db8-488f-99d8-0a5f4ee2b9a8.png)

![image](https://user-images.githubusercontent.com/93148620/143724021-9a583376-49fe-44ef-a577-938fa8fe32c1.png)

![image](https://user-images.githubusercontent.com/93148620/143724024-19ccf9b0-59f0-4245-9fd9-b6a19aa25869.png)


