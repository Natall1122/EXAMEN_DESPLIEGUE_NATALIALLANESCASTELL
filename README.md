# Examen 2ª evaluación de Despliegue de Aplicaciones Web de 2º DAW

![This is an image](/enana.jpg)

## INSTRUCCIONES
### 1.- Completad la clase `Enana.php` para que realice su cometido, explicado en los comentarios de la misma.
### 2.- Completad los test unitarios en `enanaTest.php` conforme a las especificaciones que se detallan en los comentarios.
### 3.- Completad las Actions en el fichero `cicd.yml` para:
####    a. Complete el proceso de CI y ejecute de manera automática las pruebas unitarias
####    b. Complete el proceso de CD y suba las imágenes de Docker a tu DockerHub (latest e histórico)

## ENTREGA
### 1.- Archivo **zip** del repositorio en GitHub
### 2.- Como texto en linea:
####    a. **URL** del repositorio **PÚBLICO** en GitHub
####    b. **URL** de tu imagen de DockerHub



<!--   cd:
    runs-on: ubuntu-latest
        needs: ci

        steps:
          - uses: actions/checkout@v1
          - name: Docker Login
            run: docker login -u ${{ secrets.DOCKER_USER }} -p ${{ secrets.DOCKER_PASSWORD }}
          - name: Build
            run: |
              docker build -t ${{ secrets.DOCKER_USER }}/examen:${{ github.sha }} .
              docker build -t ${{ secrets.DOCKER_USER }}/examen:latest .
          - name: Push
            run: |
              docker push ${{ secrets.DOCKER_USER }}/examen:${{ github.sha }}
              docker push ${{ secrets.DOCKER_USER }}/examen:latest     -->