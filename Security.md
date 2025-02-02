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




Diversas vulnerabilidades de NoSQL injection foram detectadas:

exemplo:
![image](https://github.com/user-attachments/assets/39fdb72f-9903-4e95-bc3c-466278220cf4)






Todos os trechos com vulnerabilidades: 

Line 18 in observations.resolver.ts
src/observations/observations.resolver.ts

High
Line 18 in observations.resolver.ts
return this.observationsService.findOne(id);
src/observations/observations.service.ts

High
Line 42 in observations.service.ts
.findByIdAndUpdate(id, updateData, { new: true })
src/observations/observations.service.ts

High
Line 47 in observations.service.ts
return this.observationModel.findByIdAndDelete(id).exec();
src/observations/observations.service.ts

High
Line 79 in observations.service.ts
id
src/observatories/observatories.resolver.ts

High
Line 19 in observatories.resolver.ts
return this.observatoriesService.findOne(id);
src/observatories/observatories.service.ts

High
Line 19 in observatories.service.ts
const user = await this.usersService.findOne(userPayload.sub);
src/observatories/observatories.service.ts

High
Line 54 in observatories.service.ts
.findByIdAndUpdate(id, updateData, { new: true })
src/observatories/observatories.service.ts

High
Line 59 in observatories.service.ts
return this.observatoryModel.findByIdAndDelete(id).exec();
src/observatories/observatories.service.ts

High
Line 73 in observatories.service.ts
id,
src/telescopes/telescopes.resolver.ts

High
Line 19 in telescopes.resolver.ts
return this.telescopesService.findOne(id);
src/telescopes/telescopes.service.ts

High
Line 39 in telescopes.service.ts
.findByIdAndUpdate(id, updateData, { new: true })
src/telescopes/telescopes.service.ts

High
Line 44 in telescopes.service.ts
return this.telescopeModel.findByIdAndDelete(id).exec();
src/telescopes/telescopes.service.ts

High
Line 67 in telescopes.service.ts
id,
src/users/users.resolver.ts

High
Line 17 in users.resolver.ts
return this.usersService.findOne(id);
src/users/users.service.ts

High
Line 27 in users.service.ts
return this.userModel.findOne({ email }).exec();
src/users/users.service.ts

High
Line 32 in users.service.ts
.findByIdAndUpdate(id, updateData, { new: true })
src/users/users.service.ts

High
Line 37 in users.service.ts
return this.userModel.findByIdAndDelete(id).exec();







Outro exemplo de vulnerabilidade identificada:

Uma maneira insegura de comparar senhas com a entrada do usuário pode permitir que hackers apliquem força bruta nas senhas.

![image](https://github.com/user-attachments/assets/a52de8c8-10d0-41ab-b6ab-830ab8c6a345)

Exemplo de correção:

![image](https://github.com/user-attachments/assets/a4db9b5d-337b-4b91-bbb3-c0928f8163df)



 
