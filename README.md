# Backend del Proyecto – FastAPI

## Instalación
pip install -r requirements.txt

## Ejecución
python -m uvicorn main:app --reload

## Endpoints disponibles
- GET /students
- GET /students/{id}

## Testing 
python -m pytest

## Docker
docker build -t daw-backend .
docker run -p 8000:8000 daw-backend

## CI/CD – GitHub Actions
Workflows ubicados en backend/.github/workflows/
- backend-test.yml
- backend-docker.yml

Requiere secrets:
- DOCKERHUB_USERNAME
- DOCKERHUB_TOKEN

## Información gráfica
+En este apartado se muestra la información obtenida al usar el comando `git log`  

```
PS C:\Users\francisco.guerrero\Desktop\proyecto-examen\backend> git log --oneline --graph
* a6a9343 (HEAD -> rama1_FranciscoGuerrero, origin/main, GitLab/main, rama2_FranciscoGuerrero, main) primer commit
```  
>Aquí indica id del commit y posición de las ramas
## Listado de remotos conectados  
***En este apartado se pueden comprobar los repositorios remotos conectados tanto en Github como Gitlab***

```
PS C:\Users\francisco.guerrero\Desktop\proyecto-examen\backend> git remote -v
GitLab  https://gitlab.com/franciscojose.guerrero/backend.git (fetch)
GitLab  https://gitlab.com/franciscojose.guerrero/backend.git (push) 
origin  https://github.com/FranKisekis/backend.git (fetch)
origin  https://github.com/FranKisekis/backend.git (push)
```  
