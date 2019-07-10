## Comandos Linux - Canivete

1. Parametro -p cria diretório recursivamente, sem a necessidade de desce a cada nível
```
mkdir -p /app/directory/path
```

2. Muda o dono e o grupo da pasta atual recursivamente
```
sudo chown -R $USER:$(id -gn $USER) .
```