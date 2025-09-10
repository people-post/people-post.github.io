## Our project
A truly decentralized social media. People own their own data, connecting to peers without centralized server. 

<script type="module">
  import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
  mermaid.initialize({ startOnLoad: true });
</script>
<pre class="mermaid">
graph LR
USER_1(User 1) <--> DB_11[(11)]:::Private1
DB_11 <--> DB_21[(21)]:::Private1
USER_1 <--> DB_21
DB_11 <--> USER_2(User 2)
DB_21 <--> USER_2
USER_1 <--> DB_41[(41)]:::Private2
DB_41 <--> USER_3(User 3)
DB_41 <--> USER_4(User 4)
USER_1 <--> DB_PUBLIC[(Public)]
USER_2 <--> DB_PUBLIC
DB_PUBLIC <--> USER_3
DB_PUBLIC <--> DB_42[(42)]
DB_42 <--> USER_4
DB_PUBLIC <--> USER_N(Other users)

linkStyle 0 stroke:lightcoral;
linkStyle 1 stroke:lightcoral;
linkStyle 2 stroke:lightcoral;
linkStyle 3 stroke:lightcoral;
linkStyle 4 stroke:lightcoral;
linkStyle 5 stroke:yellowgreen;
linkStyle 6 stroke:yellowgreen;
linkStyle 7 stroke:yellowgreen;
classDef Private1 fill:lightcoral,color:white
classDef Private2 fill:yellowgreen,color:white
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
Discord: https://discord.gg/Ma8KrwS4zU
