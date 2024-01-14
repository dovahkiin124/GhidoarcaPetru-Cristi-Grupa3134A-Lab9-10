# GhidoarcaPetru-Cristi,Grupa3134A,Lab9-10
 
# Utilizarea texturării în OpenGL

## Utilizarea pentru texturare imagini cu transparență și fără. Ce observați?

Atunci când se aplică texturi imaginilor care conțin informații despre transparență (canalul alfa), se permite apariția zonelor semi-transparente pe obiectele texturate. Această funcționalitate este utilă pentru obiecte sau texturi cu margini netede sau detalii fine care ar trebui să fie vizibile parțial prin transparență. Este esențial să configurați corespunzător proprietățile de amestecare (blending) pentru a gestiona eficient gradul de transparență.

În cazul texturării imaginilor care nu conțin informații despre transparență, acestea vor fi considerate opace, iar textura va acoperi în totalitate obiectul, fără niciun grad de transparență.

## Formate de imagine aplicate în procesul de texturare în OpenGL:

OpenGL oferă suport pentru diverse formate de imagini destinate texturilor, inclusiv:

RGB: Utilizat pentru texturi color fără canal alfa.
RGBA: Permite texturarea cu informații despre transparență prin intermediul canalului alfa.
Se acceptă și alte formate, cum ar fi formatul comprimat (DXT, ETC), formatul de adâncime, și altele. Utilizarea acestora depinde de cerințele specifice ale aplicației.

## Modificarea culorii obiectului texturat prin manipularea canalelor RGB:

Ajustarea canalelor RGB ale unui obiect texturat influențează culorile texturii. De exemplu, creșterea valorii canalului roșu (R) va intensifica tonurile roșii ale texturii, în timp ce scăderea acestei valori va accentua tonurile verzi.

## Diferențe între scena cu iluminare activată și dezactivată în contextul obiectelor texturate:

Iluminare activată:

Texturile vor reacționa la iluminare, reflectând lumină și umbre în funcție de poziția și intensitatea sursei de lumină.
Diferitele culori ale obiectului texturat vor fi afectate de iluminare, adăugând astfel un aspect mai realist.
Iluminare dezactivată:

Texturile vor fi afișate cu culorile lor originale, fără a fi influențate de sursele de lumină din scenă.
Imaginea texturată poate să pară mai uniformă și să se bazeze doar pe culorile din textură.
