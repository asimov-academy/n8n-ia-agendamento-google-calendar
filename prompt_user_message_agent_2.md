Crie uma nota de aviso sobre um evento de calendário.

Título: {{ $json["summary"] }}

Informações importantes:
- Data de início: {{ $json["start"]["dateTime"] }}
- Data de término: {{ $json["end"]["dateTime"] }}
- Organizador: {{ $json["organizer"]["email"] }}
- Participantes: {{ $json["attendees"].map(att => att.email + " (" + att.responseStatus + ")").join(", ") }}
- Link do evento: {{ $json["htmlLink"] }}
- Link da reunião: {{ $json["hangoutLink"] }}

Descrição:
{{ $json["description"] }}
