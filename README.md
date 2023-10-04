# caos-mipt


## Вывести все файлы из указанной директории
```C
int main() {
  DIR* my_dir = opendir("/home/mostovykh/task2/A");
  struct dirent* direntry = readdir(my_dir);
  while (direntry != 0) {
    printf("%s\n", direntry->d_name);
    direntry = readdir(my_dir);
  }
}
```
