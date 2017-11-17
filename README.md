# generator

Generador de formularios en cobnfig/application.rb

config.load_defaults 5.1
config.autoload_paths += %W( #{config.root}/lib )

Fomr resultante:

<%= form.text_field :name, id: :person_name, label: "Su Nombre:"%>
    <%= form.text_field :lastname, id: :person_lastname, label: "Su Apellido:"%>
    <%= form.text_field :address, id: :person_address, label: "Dirección:", small: "Introduzca su dirección completa, con CP incluido"%>
    <%= form.number_field :age, id: :person_age%>
    <%= form.submit "Enviar" %>
