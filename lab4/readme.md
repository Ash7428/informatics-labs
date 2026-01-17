# Лабораторная работа 4
содержимое Dockerfile:
<img width="551" height="354" alt="image" src="https://github.com/user-attachments/assets/ffd8012b-855c-4092-9a1e-b99afb80eb08" />

билдим контейнер c aafire:
<img width="1127" height="418" alt="image" src="https://github.com/user-attachments/assets/c1b7d58c-9404-4b99-8273-ea3c3e068148" />

Вводим `sudo docker run -it aafire` и смотрим результат:
<img width="1135" height="978" alt="image" src="https://github.com/user-attachments/assets/80319fe5-7c19-43dc-a7ab-466d9913e619" />

добавляем в Dockerfile утилиту ping:
<img width="1153" height="617" alt="image" src="https://github.com/user-attachments/assets/1984038d-60e0-4b8b-8d1b-84a890290d0d" />

вводим `sudo docker build -t aafire .` и создаем два новых контейнера:
<img width="1224" height="255" alt="image" src="https://github.com/user-attachments/assets/85cb1fed-c15d-4979-86d3-24564c4e3373" />

создаем сеть myNetwork и подключаем к ней контейнеры:
<img width="523" height="64" alt="image" src="https://github.com/user-attachments/assets/98937db5-0fee-4551-90ed-30fc7c3b7842" />

<img width="787" height="985" alt="image" src="https://github.com/user-attachments/assets/0da2f979-9990-4a92-a274-86cf8d9e5d73" />

заходим в **root** одного из контейнеров и пингуем отткда другой:
<img width="1128" height="514" alt="image" src="https://github.com/user-attachments/assets/90302fae-bd57-484b-82b4-e91ba7b87125" />

Пинг прошел успешно, выходим из под корня и удаляем контейнеры командой `docker rm $(docker ps -a -q)`
