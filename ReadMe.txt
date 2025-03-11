Librarii necesare si environment:
1 Python 3.8 sau o alta versiune mai noua
2 Biblioteci necesare:

    opencv-python: 4.5.5.64
    numpy: 1.23.4
    easyocr: 1.6.2
    re (librarie built-in Python)
    os (librarie built-in Python )

Trebuie doar schimbat la fiecare path din C:\Users\alexn\OneDrive\Desktop\CAVA-2024-Tema1\antrenare in C:\Users\user_corespunzator\path_catre_un_folder_ales, antrenare trebuie chimbat cu folderul unde sunt cele 200 de imagini initiale, iar in restul path-urilor se inlocuieste cu path-ul de mai sus, dar pastrand folder-ul de la finalul path-ului. De asemenea path-ul imaginii cu tabla de joc cropuita si goala tebuie pus in scriptul 3.

Pasul 1: inputul din primul script trebuie sa fie calea catre cele 200 de imagini de test *trebuie schimbat cu calea corespunzatoare*, iar output-ul este calea unde se vor salva 200 de imagini de joc cropuite sa ramana doar tabla de joc (se creeaza un folder crop_1).

Pasul 2: inputul din al doilea script este outputul de la primul script (cele 200 de imagini cropuite doar cu tabla de joc, folder crop_1), iar outputul este calea unde vor fi salvate 200 de imagini cropuite astfel incat sa ramana doar poze cu grid-ul de 14x14 (se creeaza un folder crop_2).

Pasul 3: Scriptul 3 are ca input calea de la outputul scriptului 2( cele 200 de imagini cropuite sa se vada doar gridul 14x14, folder crop_2), outputul este calea unde vor fi salvate mastile (se creeaza  folderul masks), iar empty_board_path este o cale catre o imagine cu tabla de joc cropuita sa se vada doar gridul 14x14 (Poza prezenta in arhiva).

Pasul 4: Inputul de la scriptul 4 este calea catre cele 200 de masti * folderul masks*, iar output_tiles_dir este calea unde vor fi salvate patratele cu imagini cu numerele adaugate pe tabla de joc *se creaza folderul tiles*, cele care vor fi interpretate OCR, iar output_positions_dir este calea catre txt-urile cu pozitiile numerelor adaugate *folderul fisiere_txt*.

Pasul 5: input_dir este in scriptul 5 calea catre cele 200 de imagini cu numerele adaugate cropuite *folderul tiles*, iar positions_dir este calea catre txt-urile cu pozitiile care vor fi ulterior modificate *folderul fisiere_txt*.

Pasul 6: In path-ul de output al fisierelor dupa pasul 5, trebuie sa se afle 200 de txt cu pozitia si numarul adaugat la fiecare pas.