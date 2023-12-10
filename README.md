usuario y contraseña de la aplicacion es user: jose y pass:12345
en la carpeta controlador/Conexionbd.java
modificar los campos:

private String BD ="Cobranza";
private String URL ="jdbc:postgresql://localhost:5432/"+BD;
private String User = "postgres";
private String Clave ="root";
