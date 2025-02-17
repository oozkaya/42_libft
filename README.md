#libft@42

###Premier projet de l'ecole 42 : coder une librairie libft.a à l'identique pour les fonctions de la premiere partie et en suivant les recommendations dans la seconde partie. La partie bonus concerne quelques fonctions sur les listes chainées, et le reste regroupe quelques fonctions persos.
----


Partie 1 | Partie 2 | Partie Bonus | Persos
----------- | ----------- | ----------- | -----------
`ft_memset`| `ft_memalloc` | `ft_lstnew` | `ft_abs`
`ft_bzero` | `ft_memdel` | `ft_lstdelone` | `ft_isupper`
`ft_memcpy` | `ft_strnew`| `ft_lstdel` | `ft_islower`
`ft_memccpy` | `ft_strdel` | `ft_lstadd` | `ft_strlwr`
`ft_memmove` | `ft_strclr` | `ft_lstiter` | `ft_strupr`
`ft_memchr` | `ft_striter` | `ft_lstdelone` | `ft_capitalize`
`ft_memcmp` | `ft_striteri` |
`ft_strlen` | `ft_strmap` |
`ft_strdup` | `ft_strmapi` |
`ft_strcpy` | `ft_strequ` |
`ft_strncpy` | `ft_strnequ` |
`ft_strcat` | `ft_strsub` |
`ft_strncat` | `ft_strjoin` |
`ft_strlcat` | `ft_strtrim` |
`ft_strchr` | `ft_strsplit` |
`ft_strrchr` | `ft_itoa` |
`ft_strstrs` | `ft_putchar` |
`ft_strnstr` | `ft_putstr` |
`ft_strcmp` | `ft_putendl` |
`ft_strncmp` | `ft_putnbr` |
`ft_atoi` | `ft_putchar_fd` |
`ft_isalpha` | `ft_putstr_fd` |
`ft_isdigit` | `ft_putendl_fd` |
`ft_isalnum` | `ft_putnbr_fd` |
`ft_isascii` |
`ft_isprint` |
`ft_toupper` |
`ft_tolower` |


----
##Partie 1

###Les fonctions de la partie 1 sont celles tirées de la libC, explications consultables dans leurs mans ! 
----

##Partie 2


| Function name | Description                    |
| ------------- | ------------------------------ |
| `ft_memalloc` | Alloue avec malloc(3) et retourne une zone de memoire "fraiche". La memoire allouee est intialisee a 0. Si l'allocation echoue, la fonction renvoie NULL. |
| `ft_memdel`   | Prend en parametre l’adresse d’un pointeur dont la zone pointee doit etre liberee avec free(3), puis le pointeur est mis a NULL. |
| `ft_strnew` | Alloue avec malloc(3) et retourne une chaine de caractere “fraiche” terminee par un ’\0’. Chaque caractere de la chaine est initialise a ’\0’. Si l’allocation echoue, la fonction renvoie NULL. |
| `ft_strdel` | Prend en parametre l’adresse d’une chaine de caracteres qui doit etre liberee avec free(3) et son pointeur mis a NULL |
| `ft_strclr` | Assigne la valeur ’\0’ a tous les caracteres de la chaine passee en parametre. |
| `ft_striter` | Applique la fonction f a chaque caractere de la chaine de caracteres passee en parametre. Chaque caractere est passe par adresse a la fonction f afin de pouvoir être modifie si necessaire. |
| `ft_striteri` | Applique la fonction f a chaque caractere de la chaine de caracteres passee en parametre en precisant son index en premier argument. Chaque caractere est passe par adresse a la fonction f afin de pouvoir etre modifie si necessaire. |
| `ft_strmap` | Applique la fonction f a chaque caractere de la chaine de caracteres passee en parametre pour creer une nouvelle chaine “fraiche” avec malloc(3) resultant des applications successives de f. |
| `ft_strmapi` | Applique la fonction f a chaque caractere de la chaine de caracteres passee en parametre en precisant son index pour creer une nouvelle chaine “fraiche” avec malloc(3) resultant des applications successives de f. |
| `ft_strequ` | Compare lexicographiquement s1 et s2. Si les deux chaines sont egales, la fonction retourne 1, ou 0 sinon. |
| `ft_strnequ` | Compare lexicographiquement s1 et s2 jusqu’a n caracteres maximum ou bien qu’un ’\0’ ait ete rencontre. Si les deux chaines sont egales, la fonction retourne 1, ou 0 sinon. |
| `ft_strsub` | Alloue avec malloc(3) et retourne la copie "fraiche" d'un troncon de la chaine de caracteres passee en parametre. Le troncon commence a l'index start et a pour longueur len. Si start et len ne designent pas un troncon de chaine valide, le comportement est indetermine. Si l'allocation echoue, la fonction renvoie NULL. |
| `ft_strjoin` | Alloue avec malloc(3) et retourne une chaine de caracteres "fraiche" terminee pas un '\0' resultant de la concatenation de s1 et s2. Si l'allocation echoue, la fonction renvoie NULL. |
| `ft_strtrim` | Alloue avec malloc(3) et retourne une copie de la chaine passee en parametre sans les espaces blancs au debut et a la fin de cette chaine. On considere comme des espaces blancs les caracteres ' ', '\n' et '\t'. Si s ne contient pas d'espaces blancs au debut ou a la fin, la fonction renvoie une copie de s. Si l'allocation echoue, la fonction renvoie NULL. |
| `ft_strsplit` | Alloue avec malloc(3) et retourne un tableau de chaines de caracteres "fraiches" (toutes terminees par un '\0', le tableau egalement donc) resultant de la decoupe de s selon le caractere c. Si l'allocation echoue, la fonction retourne NULL. |
| `ft_itoa` | Alloue avec malloc(3) et retourne une chaine de caracteres "fraiche" terminee par un '\0' representatnt l'entier n passe en parametre. Les nombres negatifs sont geres. Si l'allocation echoue, la fonction renvoie NULL. |
| `ft_putchar` | Affiche le caractere c sur la sortie standard. |
| `ft_putstr` | Affiche la chaine s sur la sortir standard. |
| `ft_putendl` | Affiche la chaine s sur la sortie standard suivi d'un '\n'. |
| `ft_putnbr` | Affiche l'entier n sur la sortie standard. |
| `ft_putchar_fd` | Ecrit le caractere c sur le descripteur de fichier fd  |
| `ft_putstr_fd` | Ecrit la chaine s sur le descripteur de fichier fd. |
| `ft_putendl_fd` | Ecrit la chaine s sur le descripteur de fichier fd suivi d'un '\n'. |
| `ft_putnbr_fd` | Ecrit l'entier n sur le descripteur de fichier fd. |


----


##Partie bonus

| Function name | Description                    |
| ------------- | ------------------------------ |
| `ft_lstnew` | Alloue avec malloc(3) et retourne un maillon “frais”. Les champs content et content_size du nouveau maillon sont initialises par copie des parametres de la fonction. Si le parametre content est nul, le champs content est initialise a NULL et le champs content_size est initialise a 0 quelque soit la valeur du parametre content_size. Le champ next est initialise a NULL. Si l’allocation echoue, la fonction renvoie NULL. |
| `ft_lstdelone` | Prend en parametre l’adresse d’un pointeur sur un maillon et libere la memoire du contenu de ce maillon avec la fonction del passee en parametre puis libere la memoire du maillon en lui meme avec free(3). La memoire du champ next ne doit en aucun cas être liberee. Pour terminer, le pointeur sur le maillon maintenant libere doit etre mis a NULL (de maniere similaire à la fonction ft_memdel). |
| `ft_lstdel` | Prend en parametre l’adresse d’un pointeur sur un maillon et libere la memoire de ce maillon et celle de tous ses successeurs l’un apres l’autre avec del et free(3). Pour terminer, le pointeur sur le premier maillon maintenant libere doit etre mis à NULL (de maniere similaire à la fonction ft_memdel). |
| `ft_lstadd` | Ajoute l'element new en tete de la liste. |
| `ft_lstiter` | Parcourt la liste lst en appliquant a chaque maillon la fonction f. |
| `ft_lstmap` | Parcourt la liste lst en appliquant à chaque maillon la fonction f et cree une nouvelle liste “fraiche” avec malloc(3) resultant des applications successives. Si une allocation echoue, la fonction renvoie NULL. |


----


##Fonctions bonus perso

| Function name | Description                    |
| ------------- | ------------------------------ |
| `ft_abs`      | Permet d'obtenir la valeur absolue d'un nombre. |
| `ft_isupper`  | Retourne vrai si le caractere c passe est en majuscule. Ne fonctionne qu'avec les caracteres ASCII. |
| `ft_islower`  | Retourne vrai si le caractere c passe est en minuscule. Ne fonctionne qu'avec les caracteres ASCII. |
| `ft_strlwr`   | Passe toute la chaine de caractere en minuscule. |
| `ft_strupr`   | Passe toute la chaine de caractere en majuscule. |
| `ft_capitalize` | Passe chaque première lettre de chaque mot de la chaine de caractere en majuscule et le reste en minuscule. |
