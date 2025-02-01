Para verificação de código foi utilizada versão opensource do projeto Snyk.io. 
Que pode ser utilizado localmente ou em esteiras de DevSecOps.


Risco Médio: 
Impacto em problemas de gestão de pacotes, ou manutenções futuras por conta de erros causados pelo pacote podem gerar paradas de esteira de devops, alocação necessária de recursos de desenvolvimento para identificação e correção de bugs ou problemas relacionados ao pacote.
Em caso de novas vulnerabilidades e exploits identificados para o pacote, risco de não atualização e grande dependencia do projeto em utilização do pacote podem gerar custos 'emergenciais' não considerados para o projeto.




Vulnerabilidade detectada:
![image](https://github.com/user-attachments/assets/6c80fa5c-ee34-4ccd-ae2d-7a49e0abefa7)


O pacote bcrypt possui uma vulnerabilidade por conta de descontinuação de suporte:
![image](https://github.com/user-attachments/assets/63f75627-8d8e-4e94-a23b-479595cb9a1a)



A solução é a alteração do pacote bcrypt,  para o pacote bcryptjs (Pacote com suporte ativo de projeto).

![image](https://github.com/user-attachments/assets/d4807910-43bd-4a45-9ffb-3d463e921a0a)


Outras validações de segurança devem ser realizados em formato DAST. A partir da URL do públicada (Riscos e vulnerabilidades podem variar dependendo do servidor-backend de sustentação do projeto). 
