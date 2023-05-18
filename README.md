# Trainemto de teste com laravel

### iniciando o projeto

1. composer install
```
docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v "$(pwd):/var/www/html" \
    -w /var/www/html \
    laravelsail/php82-composer:latest \
    composer install --ignore-platform-reqs
```
2. criando atalho pro laravel sail
```
alias sail='[ -f sail ] && sh sail || sh vendor/bin/sail'
```

3. Copie o .env.example para .env

4. inicie os containers
```
sail up -d
```

5. rode os testes para verificar se está tudo ok
```
sail test
```
