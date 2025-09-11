## Our project
A truly decentralized social media. People own their own data, connecting to peers without centralized server. 

<script type="module">
  import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
  mermaid.initialize({ startOnLoad: true });
</script>
<pre class="mermaid">
graph LR

subgraph "User 1"
USER_1(User 1):::User <--> DB_11[(pp-node 1)]:::Private1
end

DB_11 <--> DB_21[(pp-node 1)]:::Private1
USER_1 <--> DB_21
DB_11 <--> USER_2(User 2):::User

subgraph "User 2"
DB_21 <--> USER_2
end

USER_1 <--> DB_41[(pp-node 1)]:::Private2
DB_41 <--> USER_3(User 3):::User

USER_1 <--> DB_PUBLIC[(Optional centralized public node)]:::Public
USER_2 <--> DB_PUBLIC
DB_PUBLIC <--> USER_3
DB_PUBLIC <--> DB_42[(pp-node 2)]:::Public

subgraph "User 3"
USER_3
end

subgraph "User 4"
DB_41 <--> USER_4(User 4):::User
DB_42 <--> USER_4
end

DB_PUBLIC <--> USER_N(Other users):::User

linkStyle 0 stroke:lightcoral;
linkStyle 1 stroke:lightcoral;
linkStyle 2 stroke:lightcoral;
linkStyle 3 stroke:lightcoral;
linkStyle 4 stroke:lightcoral;
linkStyle 5 stroke:yellowgreen;
linkStyle 6 stroke:yellowgreen;
linkStyle 11 stroke:yellowgreen;
classDef Private1 fill:LightCoral,color:White,stroke:Gray
classDef Private2 fill:yellowgreen,color:White
classDef Public fill:LightGray,color:Black,stroke:Gray
classDef User fill:CadetBlue,color:white,stroke:DarkCyan
</pre>

## Roadmap
- Decentralized node with simple social actions based on texts and images. 
- Readonly app works offline to read news. 
- Optional centralized data service for people without data safety concern. 

## Download
First release coming out later 2025

## About us
We are a small group of hobbyists who believe the online freedom of speech is essential.

## Join us
- Discord: [Join us](https://discord.gg/Ma8KrwS4zU)
- Github: [Visit us](https://github.com/people-post)
- X: [Follow us](https://x.com/Brief495318)
