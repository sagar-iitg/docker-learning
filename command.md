
    
   ` clear
    2  sudo apt update
    3  sudo apt install docker.io
    4  docker --version
    5  docker run hello-world
    6  reboot
    7  sudo reboot
    8  clear
    9  docker images
   10  touch master.txt
   11  ls
   12  clear
   13  ls
   14  clear
   15  docker swarm init
   16  docker node ls
   17  history
   18  docker swarm join-token worker


   docker service create --name django-app-service --replicas 3 --publish 8001:8001 sagarkumar99/react-django-todo-app:latest


    1  clear
    2  sudo apt update
    3  sudo apt install docker.io
    4  docker --version
    5  docker run hello-world
    6  reboot
    7  sudo reboot
    8  clear
    9  docker images
   10  touch master.txt
   11  ls
   12  clear
   13  ls
   14  clear
   15  docker swarm init
   16  docker node ls
   17  history
   18  clear
   19  docker node ls
   20  docker swarm leave
   21  docker swarm -f leave
   22  docker -f swarm leave
   23  clear
   24  docker ls
   25  docker node ls
   26  docker swarm leave
   27  sudo docker swarm leave
   28  sudo docker swarm leave --force
   29  clear
   30  docker swarm
   31  clear
   32  docker node ls
   33  docker swarm init
   34  docker node ls
   35  docker swarm join-token worker
   36  docker ps -a
   37  clear
   38  docker service create --name django-app-service --replicas 3 --publish 8001:8001 sagarkumar99/react-django-todo-app:latest
   39  docker ps
   40  docker service ls
   41  docker ps
   42  docker service ls
   43  free -h
   44  clear
   45  mkdir deployments
   46  clear
   47  cd deployments/
   48  vi django-cluster.yaml
   49  cat django-cluster.yaml
   50  docker ps
   51  docker services ls
   52  docker service ls
   53  docker service rm  django-app-service
   54  clear
   55  ls
   56  clear
   57  ls
   58  docker stack deploy -c django-cluster.yaml django-stack
   59  docker ps
   60  docker service ls
   61  docker ps
   62  docker ps -a
   63  cat django-cluster.yaml
   64  vi django-cluster.yaml
   65  clear
   66  docker ps
   67  docker ps -a
   68  docker sevice ls
   69  docker service ls
   70  docker service rm o6mephegr119 6xc
   71  clear
   72  docker stack deploy -c django-cluster.yaml django-stack
   73  docker ps
   74  docker service ls
   75  docker node ls
   76  hostname
   77  docker service scale  django-stack_mysql-db=3
   78  clear
   79  vi django-cluster.yaml
   80  docker service ls
   81  docker service rm zz ns
   82  clear
   83  docker stack deploy -c django-cluster.yaml django-stack
   84  vi django-cluster.yaml
   85  docker stack deploy -c django-cluster.yaml django-stack
   86  docker ps
   87  docker service scale  django-stack_mysql-db=3
   88  docker service ls
   89  docker service scale  django-stack_django-app=3
   90  docker ps
   91  clear
   92  docker service logs
   93  history
   94  clear
   95  ls
   96  cd
   97  ls
   98  cd react-app/
   99  ls
  100  cd react_django_demo_app/
  101  ls
  102  cd frontend/
  103  ls
  104  cd build/
  105  ls
  106  vi index.html
  107  clear
  108  ls
  109  cd
  110  cd react-app/
  111  ls
  112  cd react_django_demo_app/
  113  ls
  114  docker images
  115  docker build -t todo .
  116  docker login
  117  docker images
  118  docker tag todo sagarkumar99/react-django-todo-app
  119  docker push sagarkumar99/react-django-todo-app:latest
  120  clear
  121  docker service l
  122  clear
  123  docker service ls
  124  docker service update --image sagarkumar99/react-django-todo-app:latest django-stack_django-app
  125  ls
  126  cd frontend/
  127  ls
  128  cd build/
  129  ls
  130  vi index.html
  131  clear
  132  ls
  133  cd ..
  134  ls
  135  cd ..
  136  ls
  137  docker image -t app .
  138  docker build -t app .
  139  docker images
  140  docker tag app sagarkumar99/react-django-todo-app
  141  docker images
  142  docker push sagarkumar99/react-django-todo-app-todo:latest
  143  docker push sagarkumar99/react-django-todo-app-todo
  144  docker tag app sagarkumar99/react-django-todo-app
  145  docker push sagarkumar99/react-django-todo-app-todo:latest
  146  clear
  147  docker images
  148  docker rmi app
  149  docker images
  150  docker ps
  151  docker ls
  152  clear
  153  docker ls
  154  docker images
  155  docker image prune
  156  clear
  157  docker images
  158  docker rmi c16
  159  docker rmi -f c16
  160  clear
  161  docker images
  162  docker rmi sagarkumar99/react-django-todo-app
  163  clear
  164  docker images
  165  docker tag todo sagarkumar99/react-django-todo-app:latest
  166  clear
  167  docker images
  168  docker push sagarkumar99/react-django-todo-app:latest
  169  clear
  170  docker service
  171  docker service ls
  172  docker service update --image  sagarkumar99/react-django-todo-app:latest  django-stack_django-app
  173  ls
  174  docker images
  175  docker run -itd todo -p 8002:8002 todo
  176  docker run -itd  -p 8002:8002 todo
  177  docker ps
  178  docker images
  179  ls
  180  docker ps
  181  clear
  182  docker ps
  183  clear
  184  docker ps
  185  docker rm -f fe337e7e51a9
  186  docker images
  187  docker run -itd  -p 8002:8001 todo
  188  ls
  189  cat Dockerfile
  190  clear
  191  cat Dockerfile
  192  ls
  193  cd frontend/
  194  ls
  195  cd build/
  196  ls
  197  cat index.html
  198  clear
  199  cd ..
  200  ls
  201  cd ..
  202  clear
  203  ls
  204  docker build -t todo1 .
  205  docker ps
  206  docker images
  207  docker rmi -f todo
  208  clear
  209  docker iamges
  210  docker images
  211  docker ps
  212  docker rm -f c452ae7aa255
  213  clear
  214  docker ps
  215  clear
  216  docker ps
  217  clear
  218  docker ps
  219  clear
  220  docker images
  221  clear
  222  docker images
  223  docker run -itd -p 8002:8001 todo1
  224  docker ps
  225  clear
  226  docker ps
  227  clear
  228  docker ps
  229  docker images
  230  docker ps
  231  clear
  232  docker images
  233  docker ps
  234  docker rm -f fff7915da5be
  235  clear
  236  docker images
  237  docker tag todo1 sagarkumar99/react-django-todo-app:latest
  238  docker images
  239  docker push sagarkumar99/react-django-todo-app:latest
  240  docker images
  241  docker service ls
  242  docker service update --name sagarkumar99/react-django-todo-app:latest  django-stack_django-app
  243  docker service update --image sagarkumar99/react-django-todo-app:latest  django-stack_django-app
  244  clear
  245  cd
  246  docker images
  247  history
  
  ```
