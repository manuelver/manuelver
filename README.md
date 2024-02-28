<style>

  .custom-btn {
    width: 150px;
    height: 40px;
    color: #fff;
    border-radius: 5px;
    padding: 10px 25px;
    font-family: 'Lato', sans-serif;
    font-weight: 500;
    background: transparent;
    cursor: pointer;
    transition: all 0.3s ease;
    position: relative;
    display: inline-block;
    box-shadow:inset 2px 2px 2px 0px rgba(255,255,255,.5),
      7px 7px 20px 0px rgba(0,0,0,.1),
      4px 4px 5px 0px rgba(0,0,0,.1);
    outline: none;
  }

  button {
    margin-right: 20px;
  }

  /* 1 */
  .btn-1{
    position: relative;
    right: 20px;
    bottom: 20px;
    border:none;
    box-shadow: none;
    width: 150px;
    height: 40px;
    line-height: 42px;
    -webkit-perspective: 230px;
    perspective: 230px;
  }
  .btn-1 span {
    background: rgb(0,172,238);
    background: linear-gradient(0deg, rgba(0,172,238,1) 0%, rgba(2,126,251,1) 100%);
    display: block;
    position: absolute;
    width: 150px;
    height: 40px;
    box-shadow:inset 2px 2px 2px 0px rgba(255,255,255,.5),
      7px 7px 20px 0px rgba(0,0,0,.1),
      4px 4px 5px 0px rgba(0,0,0,.1);
    border-radius: 5px;
    margin:0;
    text-align: center;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
    -webkit-transition: all .3s;
    transition: all .3s;
  }
  .btn-1 span:nth-child(1) {
    box-shadow:
      -7px -7px 20px 0px #fff9,
      -4px -4px 5px 0px #fff9,
      7px 7px 20px 0px #0002,
      4px 4px 5px 0px #0001;
    -webkit-transform: rotateX(90deg);
    -moz-transform: rotateX(90deg);
    transform: rotateX(90deg);
    -webkit-transform-origin: 50% 50% -20px;
    -moz-transform-origin: 50% 50% -20px;
    transform-origin: 50% 50% -20px;
  }
  .btn-1 span:nth-child(2) {
    -webkit-transform: rotateX(0deg);
    -moz-transform: rotateX(0deg);
    transform: rotateX(0deg);
    -webkit-transform-origin: 50% 50% -20px;
    -moz-transform-origin: 50% 50% -20px;
    transform-origin: 50% 50% -20px;
  }
  .btn-1:hover span:nth-child(1) {
    box-shadow:inset 2px 2px 2px 0px rgba(255,255,255,.5),
      7px 7px 20px 0px rgba(0,0,0,.1),
      4px 4px 5px 0px rgba(0,0,0,.1);
    -webkit-transform: rotateX(0deg);
    -moz-transform: rotateX(0deg);
    transform: rotateX(0deg);
  }
  .btn-1:hover span:nth-child(2) {
    box-shadow:inset 2px 2px 2px 0px rgba(255,255,255,.5),
      7px 7px 20px 0px rgba(0,0,0,.1),
      4px 4px 5px 0px rgba(0,0,0,.1);
    color: transparent;
    -webkit-transform: rotateX(-90deg);
    -moz-transform: rotateX(-90deg);
    transform: rotateX(-90deg);
  }



  /* 2 */
  .btn-2 {
    background: linear-gradient(0deg, rgba(255,151,0,1) 0%, rgba(251,75,2,1) 100%);
    line-height: 42px;
    padding: 0;
    border: none;
  }
  .btn-2 span {
    position: relative;
    display: block;
    width: 100%;
    height: 100%;
  }
  .btn-2:before,
  .btn-2:after {
    position: absolute;
    content: "";
    right: 0;
    bottom: 0;
    background: rgba(251,75,2,1);
    box-shadow:
      -7px -7px 20px 0px rgba(255,255,255,.9),
      -4px -4px 5px 0px rgba(255,255,255,.9),
      7px 7px 20px 0px rgba(0,0,0,.2),
      4px 4px 5px 0px rgba(0,0,0,.3);
    transition: all 0.3s ease;
  }
  .btn-2:before{
      height: 0%;
      width: 2px;
  }
  .btn-2:after {
    width: 0%;
    height: 2px;
  }
  .btn-2:hover{
    color: rgba(251,75,2,1);
    background: transparent;
  }
  .btn-2:hover:before {
    height: 100%;
  }
  .btn-2:hover:after {
    width: 100%;
  }
  .btn-2 span:before,
  .btn-2 span:after {
    position: absolute;
    content: "";
    left: 0;
    top: 0;
    background: rgba(251,75,2,1);
    box-shadow:
      -7px -7px 20px 0px rgba(255,255,255,.9),
      -4px -4px 5px 0px rgba(255,255,255,.9),
      7px 7px 20px 0px rgba(0,0,0,.2),
      4px 4px 5px 0px rgba(0,0,0,.3);
    transition: all 0.3s ease;
  }
  .btn-2 span:before {
    width: 2px;
    height: 0%;
  }
  .btn-2 span:after {
    height: 2px;
    width: 0%;
  }
  .btn-2 span:hover:before {
    height: 100%;
  }
  .btn-2 span:hover:after {
    width: 100%;
  }


  /* 3 */
  .btn-3 {
    border: none;
    background: rgb(251,33,117);
    background: linear-gradient(0deg, rgba(251,33,117,1) 0%, rgba(234,76,137,1) 100%);
    color: #fff;
    overflow: hidden;
  }
  .btn-3:hover {
    text-decoration: none;
    color: #fff;
  }
  .btn-3:before {
    position: absolute;
    content: '';
    display: inline-block;
    top: -180px;
    left: 0;
    width: 30px;
    height: 100%;
    background-color: #fff;
    animation: shiny-btn1 3s ease-in-out infinite;
  }
  .btn-3:hover{
    opacity: .7;
  }
  .btn-3:active{
    box-shadow:  4px 4px 6px 0 rgba(255,255,255,.3),
                -4px -4px 6px 0 rgba(116, 125, 136, .2), 
      inset -4px -4px 6px 0 rgba(255,255,255,.2),
      inset 4px 4px 6px 0 rgba(0, 0, 0, .2);
  }
  
  @-webkit-keyframes shiny-btn1 {
    0% { -webkit-transform: scale(0) rotate(45deg); opacity: 0; }
    80% { -webkit-transform: scale(0) rotate(45deg); opacity: 0.5; }
    81% { -webkit-transform: scale(4) rotate(45deg); opacity: 1; }
    100% { -webkit-transform: scale(50) rotate(45deg); opacity: 0; }
  }


  /* 4 */
  .btn-4 {
    background: green;
    border: none;
    z-index: 1;
  }
  .btn-4:after {
    position: absolute;
    content: "";
    width: 100%;
    height: 0;
    top: 0;
    left: 0;
    z-index: -1;
    border-radius: 5px;
    background-color: #eaf818;
    background-image: linear-gradient(315deg, #eaf818 0%, #f6fc9c 74%);
    box-shadow:inset 2px 2px 2px 0px rgba(255,255,255,.5);
    7px 7px 20px 0px rgba(0,0,0,.1),
    4px 4px 5px 0px rgba(0,0,0,.1);
    transition: all 0.3s ease;
  }
  .btn-4:hover {
    color: #000;
  }
  .btn-4:hover:after {
    top: auto;
    bottom: 0;
    height: 100%;
  }
  .btn-4:active {
    top: 2px;
  }

  .link-tool {
    padding-right:12px;
  }

  .link-tool img {
    width: 40px;
    height: 40px;
  }

</style>

![snake](https://github.com/Platane/snk/raw/output/github-contribution-grid-snake.svg)

<br>

## Manuel Vergara - SysAdmin

<div class="frame">
  <a href="https://vergaracarmona.es" target="_blank" rel="noreferrer"> 
    <button class="custom-btn btn-1"><span>Click!</span><span>Web</span></button>
  </a> 
  <a href="https://gitea.vergaracarmona.es/manuelver" target="_blank" rel="noreferrer"> 
    <button class="custom-btn btn-2"><span>Gitea</span></button>
  </a> 
  <a href="https://www.linkedin.com/in/manu-vergara" target="_blank" rel="noreferrer"> 
    <button class="custom-btn btn-3">Linkedin<div class="dot"></div></button>
  </a> 
  <a href="https://vergaracarmona.es/certificaciones" target="_blank" rel="noreferrer"> 
    <button class="custom-btn btn-4">Certificaciones</button>
  </a>
</div>

<br>

### Languages and Tools:

<p align="left"> 
    <a href="https://www.linux.org/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="Linux"/> 
    </a> 
    <a href="https://www.docker.com/" target="_blank" rel="noreferrer"  class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/docker/docker-original-wordmark.svg" alt="Docker"/> 
    </a> 
    <a href="https://kubernetes.io/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/kubernetes/kubernetes-original.svg" alt="Kubernetes"/> 
    </a> 
    <a href="https://helm.sh/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/helm/helm-original.svg" alt="Helm"/> 
    </a> 
    <a href="https://git-scm.com/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="Git"/> 
    </a> 
    <a href="https://www.github.com/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/github/github-original.svg" alt="Github"/> 
    </a> 
    <a href="https://about.gitlab.com/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/gitlab/gitlab-original.svg" alt="Github"/> 
    </a> 
    <a href="https://www.ansible.com/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/ansible/ansible-plain.svg" alt="Ansible"/> 
    </a> 
    <!-- <a href="https://argoproj.github.io/cd/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/argocd/argocd-original.svg" alt="ArgoCD"/> 
    </a>  -->
    <!-- <a href="https://azure.microsoft.com/en-us/products/devops/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/azuredevops/azuredevops-plain.svg" alt="Azure DevOps"/> 
    </a>  -->
    <a href="https://airflow.apache.org/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/apacheairflow/apacheairflow-original.svg" alt="Apache Airflow"/> 
    </a> 
    <a href="https://apache.org/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/apache/apache-original.svg" alt="Apache"/> 
    </a> 
    <a href="https://www.nginx.com" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/nginx/nginx-original.svg" alt="Nginx"/> 
    </a> 
</p>
<p align="left"> 
    <a href="https://mariadb.org/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mariadb/mariadb-original.svg" alt="MariaDB"/> 
    </a> 
    <a href="https://prometheus.io/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/prometheus/prometheus-original.svg" alt="Prometheus"/> 
    </a> 
    <a href="https://grafana.com/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/grafana/grafana-original.svg" alt="Grafana"/> 
    </a> 
    <a href="https://terraform.io/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/terraform/terraform-original.svg" alt="Terraform"/> 
    </a> 
    <a href="https://aws.amazon.com/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/amazonwebservices/amazonwebservices-original-wordmark.svg" alt="AWS"/> 
    </a> 
    <!-- <a href="https://azure.microsoft.com/en-us" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/azure/azure-original.svg" alt="Azure"/> 
    </a>   -->
    <!--  <a href="https://cloud.google.com/?hl=en" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/googlecloud/googlecloud-original.svg" alt="GCloud"/> 
    </a>  -->
    <a href="https://www.digitalocean.com/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/digitalocean/digitalocean-original.svg" alt="Digital Ocean"/> 
    </a> 
    <a href="https://www.vim.org/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/vim/vim-original.svg" alt="Vim"/> 
    </a> 
    <a href="https://www.markdownguide.org/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/markdown/markdown-original.svg" alt="Markdown"/> 
    </a> 
    <a href="https://www.gnu.org/software/bash/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/bash/bash-original.svg" alt="Bash"/> 
    </a> 
    <a href="https://www.python.org" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python"/> 
    </a>
    <a href="https://go.dev/" target="_blank" rel="noreferrer" class="link-tool"> 
        <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/go/go-original.svg" alt="Golang"/> 
    </a>
</p>

<br>

### Blog of notes 

[Last notes (In Spanish)](https://vergaracarmona.es/apuntes):

<table>
  <tr><th>Date</th><th>Post</th><th>Link</th><th>Topics</th></tr>
<!-- APUNTES:START --><tr><td>17/02/2024</td><td>🤖 <b>Gestión de la Salida de Datos</b></td><td>https://vergaracarmona.es/gestion-de-la-salida-de-datos/</td><td>Teoría, comandos, Linux, shell</td></tr><tr><td>27/01/2024</td><td>🤖 <b>Estrategias de deployment</b></td><td>https://vergaracarmona.es/estrategias-de-deployment/</td><td>Teoría, CICD, cloud, Kubernetes</td></tr><tr><td>13/01/2024</td><td>🍺 <b>Gestión de secretos con Ansible Vault</b></td><td>https://vergaracarmona.es/gestion-de-secretos-con-ansible-vault/</td><td>Tutoriales, Ansible, seguridad</td></tr><tr><td>03/01/2024</td><td>🤙🏾 <b>Guía del comando tcpdump</b></td><td>https://vergaracarmona.es/guia-del-comando-tcpdump/</td><td>Guías, comandos, Linux, seguridad</td></tr><tr><td>23/12/2023</td><td>🚀 <b>Crear módulos de Terraform reutilizables</b></td><td>https://vergaracarmona.es/crear-modulos-de-terraform-reutilizables/</td><td>Guías, CICD, Terraform</td></tr><tr><td>09/12/2023</td><td>🔥 <b>Bats para testear scripts</b></td><td>https://vergaracarmona.es/bats-para-testear-scripts/</td><td>Teoría, bash, script, shell</td></tr><tr><td>25/11/2023</td><td>⚡️ <b>Estándares de codificación</b></td><td>https://vergaracarmona.es/estandares-de-codificacion/</td><td>Teoría, estándar, programación</td></tr><tr><td>11/11/2023</td><td>🔥 <b>Arquitectura serverless con KNative</b></td><td>https://vergaracarmona.es/arquitectura-serverless-con-knative/</td><td>Tutoriales, Kubernetes, programación</td></tr><tr><td>02/11/2023</td><td>🛠 <b>Guía para actualizaciones del clúster EKS</b></td><td>https://vergaracarmona.es/actualizaciones-del-cluster-eks/</td><td>Guías, AWS, cloud, Helm, Kubernetes, Terraform</td></tr><tr><td>21/10/2023</td><td>🔥 <b>Una breve historia de las shells</b></td><td>https://vergaracarmona.es/historia-de-las-shells/</td><td>Teoría, estándar, Linux, shell</td></tr><!-- APUNTES:END -->
</table>
<br>

```
  ____                  ____                     
 / __ \___  ___ ___    / __/__  __ _____________ 
/ /_/ / _ \/ -_) _ \  _\ \/ _ \/ // / __/ __/ -_)
\____/ .__/\__/_//_/ /___/\___/\_,_/_/  \__/\__/ 
    /_/                                          
 ___ _  _____ ______ ___    __/ /  ___ _______ 
/ -_) |/ / -_) __/ // / |/|/ / _ \/ -_) __/ -_)
\__/|___/\__/_/  \_, /|__,__/_//_/\__/_/  \__/ 
                /___/                          
```

<br>

---

## Stats

![Profile views](https://komarev.com/ghpvc/?username=manuelver&color=lightgrey)
![visitors](https://visitor-badge.glitch.me/badge?page_id=manuelver.manuelver)

[![manuelver's GitHub stats-Dark](https://github-readme-stats.vercel.app/api?username=manuelver&show_icons=true&theme=dark#gh-dark-mode-only)](https://github.com/manuelver/github-readme-stats#gh-dark-mode-only)
[![manuelver's GitHub stats-Light](https://github-readme-stats.vercel.app/api?username=manuelver&show_icons=true&theme=default#gh-light-mode-only)](https://github.com/manuelver/github-readme-stats#gh-light-mode-only)

[![GitHub Streak stats-Dark](https://github-readme-streak-stats.herokuapp.com/?user=manuelver&theme=dark#gh-dark-mode-only)](https://github.com/manuelver/github-readme-stats#gh-dark-mode-only)
[![GitHub Streak stats-Light](https://github-readme-streak-stats.herokuapp.com/?user=manuelver&theme=default#gh-light-mode-only)](https://github.com/manuelver/github-readme-stats#gh-light-mode-only)

[![Top Langs Dark](https://github-readme-stats.vercel.app/api/top-langs/?username=manuelver&layout=compact&theme=dark#gh-dark-mode-only)](https://github.com/manuelver/github-readme-stats#gh-dark-mode-only)
[![Top Langs Light](https://github-readme-stats.vercel.app/api/top-langs/?username=manuelver&layout=compact&theme=light#gh-light-mode-only)](https://github.com/manuelver/github-readme-stats#gh-light-mode-only)

---

<br><br>

<p align="center">
    <img src="https://media.giphy.com/media/NTur7XlVDUdqM/giphy.gif" width="70%"/>
</p>

<br>

<p align="center">
 ⬇️  Check out my repos  ⬇️ 
</p>
