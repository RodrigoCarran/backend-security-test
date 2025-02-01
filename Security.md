Para verificação de código foi utilizada versão opensource do projeto Snyk.io. 
Que pode ser utilizado localmente ou em esteiras de DevSecOps.


Vulnerabilidade detectada:
![image](https://github.com/user-attachments/assets/6c80fa5c-ee34-4ccd-ae2d-7a49e0abefa7)


O pacote bcrypt possui uma vulnerabilidade por conta de descontinuação de suporte:
![image](https://github.com/user-attachments/assets/63f75627-8d8e-4e94-a23b-479595cb9a1a)



A solução é a alteração do pacote bcrypt,  para o pacote bcryptjs (Pacote com suporte ativo de projeto).

![image](https://github.com/user-attachments/assets/d4807910-43bd-4a45-9ffb-3d463e921a0a)


Outras validações de segurança devem ser realizados em formato DAST. A partir da URL do públicada (Riscos e vulnerabilidades podem variar dependendo do servidor-backend de sustentação do projeto). 
