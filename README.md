# Docker-training
Assesment

# Coomands

cd "C:\Users\francisco.sosa\source\repos\dockertraining_francisco_sosa_v1" 

docker build -f dockertraining_francisco_sosa_v1\Dockerfile --force-rm -t dockertraining_francisco_sosa .

docker run --name Site1 -p 8085:80 dockertraining_francisco_sosa

docker run --name Site2 -p 8086:80 -e "AppSettings:storename"="4th Source" dockertraining_francisco_sosa
