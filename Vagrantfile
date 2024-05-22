
Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/xenial64"

  config.vm.provision "shell", inline: <<-SHELL

    echo "-- Insertar datos de ejemplo en la tabla 'pacientes'" > /home/vagrant/datos_pacientes.sql
    echo "INSERT INTO gestion_clinica_veterinaria.pacientes (idPaciente, nombre, especie, raza, edad, dueño) VALUES" >> /home/vagrant/datos_pacientes.sql
    echo "(202401, 'Dona', 'Gato', 'Carey', 6, 'Ana')," >> /home/vagrant/datos_pacientes.sql
    echo "(202402, 'Gizmo', 'Perro', 'Labrador', 11, 'Pepe')," >> /home/vagrant/datos_pacientes.sql
    echo "(202403, 'Silvestro', 'Gato', 'Bombay', 9, 'Gilito');" >> /home/vagrant/datos_pacientes.sql

  SHELL
 
end
