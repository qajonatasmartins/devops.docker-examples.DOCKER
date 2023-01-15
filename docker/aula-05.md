# Container

- Add uma tag ao seu container `docker build -t app:v1 .`
- Verificando logs do container `docker logs -f image_id`: ??
- Verificando logs do container `docker logs -n number_logs_na_tela image_id`: ultimos 10 do final para o inicio.
- Verificando logs do container `docker logs -t image_id`: verifica data e hora do log
- Verificando logs do container `docker logs image_id`: Todos os logs
- rodar para comunicar `docker run -d -p 80:3000 --name banana app:v1`