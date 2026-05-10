# 🎧 Kvsper - Portfólio Oficial

Site-portfólio profissional para o DJ **Kvsper**, com seções de **vídeos (sets/lives)** , **cartazes de eventos (flyers)** e **agenda de shows**. Desenvolvido com HTML, CSS e JavaScript puro – totalmente editável através do arquivo `data.js`.

![Visual do site](assets/screenshot.png)
*(adicione um print do seu site na pasta assets/screenshot.png depois)*

## ✨ Funcionalidades

- 🎨 **Visual dark/neon** com efeitos glow, responsivo para celular e desktop
- 📹 **Galeria de vídeos** – suporte a YouTube (embed) e vídeos locais (.mp4)
- 🖼️ **Galeria de cartazes** (flyers) – basta trocar as imagens na pasta `assets/flyers/`
- 📅 **Agenda de eventos** com data, local e informações extras
- 🔗 **Links para redes sociais** (Instagram, SoundCloud, etc.)
- 🛠️ **100% editável sem mexer no HTML** – tudo centralizado no `data.js`

## 📂 Estrutura de pastas

kvsper_portfolio/
├── index.html # página principal
├── data.js # TODOS os conteúdos (nome, vídeos, flyers, agenda, redes)
├── README.md # este arquivo
├── LICENSE # licença MIT
├── .gitignore # arquivos ignorados pelo Git
└── assets/
├── flyers/ # coloque suas imagens de cartazes aqui (.jpg, .png)
├── videos/ # (opcional) para vídeos locais .mp4
└── thumbs/ # (opcional) miniaturas para vídeos locais


## 🚀 Como usar localmente

1. Baixe todos os arquivos mantendo a estrutura de pastas.
2. Edite o `data.js` com suas informações (já parcialmente preenchido).
3. Coloque suas imagens de flyers dentro da pasta `assets/flyers/`.
4. Abra o arquivo `index.html` no seu navegador – funcionará imediatamente.

## ☁️ Como publicar online (gratuito)

### Opção 1: GitHub Pages (recomendado)
1. Crie um repositório no [GitHub](https://github.com).
2. Faça upload de todos os arquivos (pode arrastar a pasta inteira).
3. Vá em **Settings > Pages**, em "Branch" selecione `main` e clique em **Save**.
4. Seu site estará em `https://SEU_USUARIO.github.io/NOME_DO_REPOSITORIO/`

### Opção 2: Netlify (ainda mais rápido)
- Acesse [app.netlify.com/drop](https://app.netlify.com/drop)
- Arraste sua pasta inteira para dentro da página
- Pronto – site no ar em segundos!

## ✏️ Como editar meu conteúdo

Tudo fica no arquivo `data.js`. Exemplo com seus dados:

``javascript
const DJ_DATA = {
    name: "Kvsper",
    bio: "DJ e produtor musical...",
    
    social: [
        { url: "https://instagram.com/kvsper.dj", icon: "fab fa-instagram" },
        { url: "https://soundcloud.com/kv_sper", icon: "fab fa-soundcloud" }
    ],
    
    videos: [
        { title: "Live @ Club", type: "youtube", embed: "https://youtube.com/embed/..." }
    ],
    
    flyers: [
        { image: "assets/flyers/flyer1.jpg", caption: "Evento - 10 Maio" }
    ],
    
    events: [
        { date: "SÁBADO, 14 JUN 2025", location: "Clube X - Cidade", extra: "Abertura 23h" }
    ]
};


💡 Dica: Para adicionar um novo cartaz, coloque a imagem na pasta assets/flyers/ e adicione uma nova linha dentro do array flyers no data.js.

🎨 Personalização visual
Você pode alterar cores, fontes e tamanhos diretamente no <style> do index.html. Os principais pontos:

Cor neon: #ff66cc (magenta) e #33aaff (azul)

Fundo gradiente: radial-gradient no .bg-gradient

📄 Licença
Este projeto está sob a licença MIT – você pode usar, modificar e distribuir livremente, mantendo os créditos ao autor original.

Conteúdo artístico (vídeos, cartazes, áudio): Todos os direitos reservados ao artista Kvsper. Não reproduza sem autorização.

📬 Contato
Para bookings, parcerias ou contratações:

Email: kspbeatz@gmail.com

Instagram: @kvsper.dj

SoundCloud: KV_Sper


Desenvolvido com 💜 por Kvsper – 2025

🎧 "Music is the answer"


## Arquivo adicional: `data.js` (já pré-configurado com seus dados)

Para facilitar, aqui está o `data.js` já com suas informações. Basta copiar e substituir o existente:

``javascript
const DJ_DATA = {
    // INFORMAÇÕES PESSOAIS
    name: "Kvsper",
    bio: "DJ e produtor de música eletrônica. Sets energéticos que conectam house, techno e experiências únicas na pista.",

    // REDES SOCIAIS
    social: [
        { platform: "instagram", url: "https://instagram.com/kvsper.dj", icon: "fab fa-instagram" },
        { platform: "soundcloud", url: "https://soundcloud.com/kv_sper", icon: "fab fa-soundcloud" }
    ],

    // VÍDEOS - substitua pelos seus links do YouTube
    videos: [
        { title: "Live @ Club Set", type: "youtube", embed: "https://www.youtube.com/embed/dQw4w9WgXcQ" },
        { title: "Mix Session 2025", type: "youtube", embed: "https://www.youtube.com/embed/jfKfPfyJRdk" },
        { title: "Sunset Set", type: "youtube", embed: "https://www.youtube.com/embed/3JZ_D3ELwOQ" }
    ],

    // CARTAZES - coloque as imagens na pasta assets/flyers/
    flyers: [
        { image: "assets/flyers/flyer1.jpg", caption: "Próximo evento - Em breve" },
        { image: "assets/flyers/flyer2.jpg", caption: "Tour 2025 - Em breve" },
        { image: "assets/flyers/flyer3.jpg", caption: "Festival - Em breve" }
    ],

    // AGENDA - preencha com suas datas reais
    events: [
        { date: "SÁBADO, 24 MAIO 2025", location: "Club Vibe - São Paulo, SP", extra: "Abertura: 23h. Ingressos na porta." },
        { date: "SEXTA, 13 JUN 2025", location: "Factory House - Rio de Janeiro, RJ", extra: "Line-up especial + convidados." },
        { date: "SÁBADO, 05 JUL 2025", location: "Sunset Beach Club - Florianópolis, SC", extra: "Set ao pôr do sol." }
    ]
};

