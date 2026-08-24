La idea de la imagen es que **un controlador de dominio no usa un único protocolo para todo**, sino varias “tuberías” distintas, cada una con su propio formato de mensajes: si un cliente quiere **consultar, crear, modificar o borrar objetos del directorio** como usuarios o grupos, usa **LDAP**; si quiere **autenticarse**, normalmente usa **Kerberos** y, en ciertos casos, **NTLM** como mecanismo alternativo o de compatibilidad; y si necesita **resolver nombres o localizar servicios del dominio**, usa **DNS**. Todos esos protocolos llegan al mismo entorno del controlador de dominio, pero no hacen lo mismo ni usan la misma estructura interna de paquetes. Además, DNS no es algo “inventado” por Active Directory, sino un servicio independiente que AD utiliza de forma fundamental para localizar controladores y servicios; Kerberos también existe como protocolo independiente, aunque en un dominio Windows el DC incorpora y presta ese servicio de autenticación como parte esencial del funcionamiento de AD.


<img width="1448" height="1086" alt="ChatGPT Image 24 ago 2026, 19_59_01" src="https://github.com/user-attachments/assets/35b8d41a-7438-4e4e-8777-400fad97fe4f" />

---

<img width="1448" height="1086" alt="ChatGPT Image 24 ago 2026, 20_11_26" src="https://github.com/user-attachments/assets/133f62b0-aa90-4826-942e-65f1c0fc52ff" />
