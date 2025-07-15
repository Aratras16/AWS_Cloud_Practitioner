# IAM Introduction: Users,Groups,Policies
 **IAM** = Identity and Access Management, is a **Global** service
- Es una cuenta raiz creada por default, esta no debe ser usada o compartida, para ello crearemos los llamados usuarios y grupos.

- **Usuarios** son personas dentro de tu organizacion y pueden ser agrupadas.
- **Grupos** son conjuntos que contienen solo usuarios y no otros grupos.

Un usuario puede no pertenecer a ningun grupo o puede estar en varios grupos a la vez.
![alt text](image-7.png)

Los grupos son creados para darles acceso a los usuarios a ciertas funciones de AWS para ello debemos darles permisos **policies**
- Los permisos **Policies** son documentos JSON que pueden ser asignados a usuarios o grupos, estos documentos describen que acciones pueden realizar dentro del entorno de AWS.
- En AWS se debe aplicar el principio de menor privilegio, es decir, no le des a un usuario mas permisos de los que necesita.
![alt text](image-8.png)

    Al momento de entrar a la consola de IAM podemos notar que las regiones estan desactivadas esto se debe a que IAM es un servicio global.
    ![alt text](image-9.png)

## IAM POLICIES INHERITANCE

Al momento de crear un grupo a las personas pertenecientes a dicho grupo se les otorgan los permisos correspondientes al grupo en el que pertencen a esto se le conoce como herencia de permisos **Policies Inheritance**. Como nota hay que recordar que una persona puede pertenecer a varios grupos por lo cual tendra acceso a los servicios  que su grupo permita.
![alt text](image-10.png)