# Prueba técnica frontend
Prueba técnica a realizar a perfil Frontend Developer Jr.

### Objetivo
Realizar la maquetación (HTML y CSS) y realizar la funcionalidad en Javascript/TypeScript del siguiente prototipo: /recursos/mockup_form.svg

Se recomienda usar algun frameworks como Angular o React.

### Funcionamiento
Tener en cuenta los siguientes requerimientos para realizar la funcionalidad.

* La imagen inicial se encuentra en /recursos/iconoUser.svg
* Validar los campos obligatorios del formulario, los cuales están marcados con asterisco
* Validar la estructura de correo electrónico
* El campo Profesión es un <select>, los valores se obtendrán del siguiente endpoint:
	https://www.plmconnection.com/devplmservices/RestPLMClientsEngine/RestPLMClientsEngine.svc/getProfessions

* El campo Especialidad es un <select> y solo se mostrará cuando el la profesión seleccionada sea Médico [ ProfessionId= 7], los valores se obtendrán del siguiente endpoint:
	https://www.plmconnection.com/devplmservices/RestPLMClientsEngine/RestPLMClientsEngine.svc/getSpecialities?professionId=7

* El campo Cédula Profesional solo se mostrará cuando la profesión seleccionada sea Médico [ProfessionId= 7]

* El campo País es un <select>, los valores se obtendrán del siguiente endpoint:
	https://www.plmconnection.com/devplmservices/RestPLMClientsEngine/RestPLMClientsEngine.svc/getCountries

* El campo Estado/departamento es un <select>, los valores se obtendrán del siguiente endpoint:
	https://www.plmconnection.com/devplmservices/RestPLMClientsEngine/RestPLMClientsEngine.svc/getStateByCountry?countryId={COUNTRYID}

	Nota: {COUNTRYID} es el identificador [CountryId] del campo País seleccionado. 

* El campo Delegación/Municipio es un <select>, los valores se obtendrán del siguiente endpoint:
	https://www.plmconnection.com/devplmservices/RestPLMClientsEngine/RestPLMClientsEngine.svc/getLocationsByState?stateId={STATEID}


	Nota: {STATEID} es el identificador [StateId] del campo Estado seleccionado. 

* Al presionar el botón actualizar y el formulario es válido los datos ingresados/seleccionados  deberán mostrarse en consola. 

### Consideraciones. 

* Cuando haya terminado deberás crear un repositorio de github y compartir la liga para poder evaluar. 

* La prueba esta relacionada con la forma de trabajar de PLM. ¡Buena suerte y esperamos tener noticias tuyas pronto!



