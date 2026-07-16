<h1>
  <img src="https://emojis.slackmojis.com/emojis/images/1531849430/4246/blob-sunglasses.gif?1531849430" width="30"/>
  Hey! Nice to see you.
</h1>

<p>
  Welcome to my page!<br/>
  I'm <b>Akhmad Fauzy</b>, a software engineer from
  <img src="https://cdn-icons-png.flaticon.com/512/197/197559.png" width="13"/>
  <b>Indonesia</b>.
</p>

<p>
  I build web, mobile, and backend systems — while trying to automate anything repetitive.
</p>

<h3>Things I code with</h3>

<p>
  <img alt="TypeScript" src="https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white"/>
  <img alt="Node.js" src="https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=node.js&logoColor=white"/>
  <img alt="React" src="https://img.shields.io/badge/-React-20232A?style=flat-square&logo=react&logoColor=61DAFB"/>
  <img alt="React Native" src="https://img.shields.io/badge/-React%20Native-20232A?style=flat-square&logo=react&logoColor=61DAFB"/>
  <img alt="Java" src="https://img.shields.io/badge/-Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white"/>
  <img alt="PostgreSQL" src="https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white"/>
  <img alt="Docker" src="https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
</p>

<h3>Things I find interesting</h3>

<p>
  Backend engineering · Automation · Go · Self-hosting · Software architecture
</p>

<p>
  Occasionally maintaining a homelab that started from “just one service.”
</p>

<h3>Homelab Architecture</h3>

```mermaid
flowchart LR
    subgraph Public["Public Internet"]
        Client[Client / Browser]
        Remote[Remote Device]
    end

    subgraph Cloud["Cloudflare"]
        Tunnel[Cloudflare Tunnel]
    end

    subgraph Home["Home Network / Homelab"]
        subgraph Gateway["Routing Layer"]
            NPM[Nginx Proxy Manager]
            AdGuard[AdGuard Home]
        end

        subgraph Services["Personal Services"]
            Website[www.avzy.my.id<br/>Web Resume]
            Other[Other Personal Services]
        end

        subgraph Access["Private Access"]
            SSH[SSH]
        end
    end

    subgraph Tailnet["Tailscale Network"]
        Tailscale[Tailscale]
    end

    Client -->|Public access| Tunnel
    Tunnel -->|Encrypted tunnel| NPM

    NPM --> Website
    NPM --> Other

    AdGuard -->|Local DNS resolution| NPM

    Remote -->|Outside home LAN| Tailscale
    Tailscale --> SSH
```

<h3>Where to find me</h3>

<p>
  <a href="https://linkedin.com/in/auzy">LinkedIn</a> ·
  <a href="https://www.avzy.my.id">Web</a>
</p>
