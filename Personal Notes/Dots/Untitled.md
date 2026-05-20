```mermaid
flowchart LR
    start_sequence((Start)) --> gather_ingredients{Gather Ingredients}
    gather_ingredients --> bread[Do I have Bread?]
    bread -->|No| get_bread{Get Bread}
    bread -->|Yes| do_i_peanut_butter[Do I have Peanut Butter?]
    get_bread -->   do_i_peanut_butter
    do_i_peanut_butter -->|No| get_peanut_butter{Get Peanut Butter}
    do_i_peanut_butter -->|Yes| assemble{Assemble Sandwich}
    get_peanut_butter --> assemble{Assemble Sandwich}
    assemble --> end_sequence((END))
````


```mermaid
flowchart LR
	A(Are you Deaf?) --> B((can you hear?))
	B -->|yes| C(not Deaf)
	B -->|no| D(Deaf)
	C & D --> E((Have Fun?))
	E --> F{Yes} 
```

