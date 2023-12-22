Examen Jordi ejercicio 1 Insignias. Completado entero. Backend funcional testeado en Swagger.

Implementacion de modelo Insignia  con atributos name y avatar.

Implementación de funciones     

    public void addInsignias(List<Insignia> i, String username);
    
    public ArrayList<Insignia> getInsignias(String username);

Creación de servicio para conseguir las insignias de un usuario a través de su username:

Localizado en UsuarioService.java

    @GET
    @ApiOperation(value = "get all Insignias", notes = "asdasd")
    @ApiResponses(value = {
            @ApiResponse(code = 201, message = "Successful", response = Insignia.class, responseContainer="List"),
    })
    @Path("/listar_insignias_usuario/insignias/{username}")

Inicializados usuarios y asignadas insignias a los siguientes usuarios:

username: jordi (4 insignias)

username: aran (2 insignias)

username: pedro (2 insignias)

username: bryan (2 insignias)
