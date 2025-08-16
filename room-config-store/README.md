### Room Config Store
This script creates a config store for each room as hardcoded inside the variables. It uses a jinja2 template to return the value corresponding to the path list sent as field input.

Eg:
The following input into the script can be used to send the same command to different IR blasters situated across rooms
```
- "{{ room }}"
- ir_entity
```

This can be used in place of a key value store/hashmap for dynamically sending commands and runs to similar entities across rooms without script duplication
