# idp_image_try_2
Just for a test on a docker toolbox worker


!!! Aceasta imagine preia si scrie continut din/in fisierul \~/my_dir_1/data/test.txt. Acest path este referentiat in docker-compose-visualize.yml, in volumes din cadrul serviciului "web". Scrierea si citirea din path-ul acela (din acel .txt) se face in app.py, de fiecare data cand se acceseaza pagina 192.168.99.100:8888/ . Pe scurt, trebuie sa ai creat deja path-ul acela pe masina pe care rulezi! (~/my_dir_1/data/test.txt).

Pentru ca nu folosesc un path din /mnt/sda1/... (unde se afla volumele docker), inseamna ca acest path NU este persistent (dupa inchiderea masinii pe care ruleaza containerul, path-ul va disparea la urmatorul boot)! Aceeasi imagine, dar cu volum persistent (in /mnt/sda1/...), este prezenta in repository-ul idp_image_try_3.
