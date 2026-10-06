MER - Consultório Dr. Roberto

1- Entidades

    Paciente: Cliente do consultório odontológico.

    Procedimento: Tratamentos disponíveis (ex: Limpeza, Clareamento, Canal, Lentes).

    Consulta: Agendamento e atendimento do paciente.

2- Atributos

    Paciente:

        id_paciente (PK - Primary Key)

        nome

        telefone

        cpf

    Procedimento:

        id_procedimento (PK - Primary Key)

        nome_procedimento

        duracao_estimada

        valor

    Consulta:

        id_consulta (PK - Primary Key)

        data_hora

        status (Ex: "Agendada", "Realizada", "Cancelada")

        id_paciente (FK - Foreign Key)

        id_procedimento (FK - Foreign Key)

3- Relacionamentos

    Paciente -> Consulta: 1 Paciente agenda 1 ou várias Consultas (1:N).

    Consulta -> Procedimento: 1 Consulta realiza 1 ou vários Procedimentos (1:N).