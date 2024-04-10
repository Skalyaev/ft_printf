# ft_printf
> *Le but de ce projet est assez simple. Vous allez recoder une partie de printf().*

## Checklist
- [x] `%c` Imprime un seul caractère.
- [x] `%s` Imprime une chaîne de caractères (selon la convention C courante).
- [x] `%p` L'argument du pointeur void * doit être imprimé en format hexadécimal.
- [x] `%d` Imprime un nombre décimal (base 10).
- [x] `%i` Imprime un entier en base 10.
- [x] `%u` Imprime un nombre décimal non signé (base 10).
- [x] `%x` Imprime un nombre en format hexadécimal (base 16) en minuscules.
- [x] `%X` Imprime un nombre en format hexadécimal (base 16) en majuscules.
- [x] `%%` Imprime un signe de pourcentage.

## Install
```bash
sudo apt update -y
sudo apt install -y ar
sudo apt install -y make
```
```bash
mkdir -p $HOME/.local/lib
mkdir -p $HOME/.local/src
mkdir -p $HOME/.local/include
```
```bash
link=Skalyaeve/ft_printf
name=libftprintf

git clone https://github.com/$link.git $name
cd $name && make && make clean

ln -s $PWD/$name.a $HOME/.local/lib/$name.a
ln -s $PWD/src $HOME/.local/src/$name
ln -s $PWD/include $HOME/.local/include/$name
```

## Usage
- `gcc` flags:
```bash
-L $HOME/.local/lib -lftprintf
```

## Uninstall
```bash
name=libftprintf

rm -r $name
rm $HOME/.local/lib/$name.a
rm $HOME/.local/src/$name
rm $HOME/.local/include/$name
```

