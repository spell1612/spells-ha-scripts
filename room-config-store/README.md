### Room Config Store
This script creates a config store for each room hardcoded inside the variables block. It uses a jinja2 template to return the value corresponding to the path list sent as field input.

Eg:
Input the following into the script to get the appropriate entity_id as response, which can then be used to send the same command to different IR blasters situated across any room
```
- "{{ room }}"
- ir_entity
```

This can be used in place of a key value store/hashmap for dynamically sending commands and runs to similar entities across rooms without script duplication
