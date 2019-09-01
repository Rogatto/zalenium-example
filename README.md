# Projeto de exemplo do Zalenium
**Demonstrando a execução do Zalenium de nossos testes criado com o Selenium.**

#Instalação do Zalenium

docker pull elgalu/selenium <br/>
docker pull dosel/zalenium
  

# Execução do Zalenium

**Executar container local para apontar nossos testes**

 docker run --rm -ti --name zalenium -p 4444:4444 \
    -v /var/run/docker.sock:/var/run/docker.sock \
    -v /tmp/videos:/home/seluser/videos \
    --privileged dosel/zalenium start <br/>
   
**Live:**
http://localhost:4444/grid/admin/live

**Dashboard:**
http://localhost:4444/dashboard/

# Apontar nossos testes para o seguinte endpoint para executar localmente: 
http://localhost:4444/wd/hub