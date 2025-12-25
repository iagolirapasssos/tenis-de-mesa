# 🏓 Tênis de Mesa - Video Hub

> Plataforma moderna de vídeos educacionais de tênis de mesa com playlists dinâmicas via YouTube API

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
![YouTube API](https://img.shields.io/badge/YouTube-API%20v3-red.svg)

## 📋 Sobre o Projeto

O **Tênis de Mesa Video Hub** é uma aplicação web progressiva (PWA) que organiza e exibe vídeos educacionais de tênis de mesa do YouTube em categorias técnicas específicas. Com design moderno e interface intuitiva, facilita o aprendizado e aperfeiçoamento de técnicas do esporte.

### ✨ Características Principais

- 🎨 **Design Moderno**: Interface glassmorphism com gradientes vibrantes
- 📱 **Responsivo**: Funciona perfeitamente em desktop, tablet e mobile
- 🔍 **Busca Inteligente**: Sistema de busca em tempo real
- ♾️ **Carregamento Infinito**: Carregue mais vídeos sob demanda
- 🎯 **20 Categorias Técnicas**: Desde fundamentos até técnicas avançadas
- 🌐 **PWA**: Pode ser instalado como aplicativo
- 🎬 **Player Integrado**: Assista vídeos sem sair da plataforma
- 💾 **Sessão Persistente**: API Key salva durante a sessão

## 🚀 Tecnologias Utilizadas

- **HTML5** - Estrutura semântica
- **Tailwind CSS** - Framework CSS via CDN
- **JavaScript (Vanilla)** - Lógica da aplicação
- **YouTube Data API v3** - Busca e exibição de vídeos
- **Service Worker** - Cache e funcionalidade offline (PWA)
- **SessionStorage** - Armazenamento de API Key

## 📦 Estrutura do Projeto

```
table-tennis-video-hub/
│
├── index.html           # Página principal
├── app.js              # Lógica da aplicação
├── manifest.json       # Configuração PWA
├── service-worker.js   # Service Worker para PWA
└── README.md          # Documentação
```

## 🎯 Categorias Disponíveis

1. **Saques (Serves)** - Técnicas de saque
2. **Recepção de Saque** - Como receber saques
3. **Forehand Drive** - Drive de forehand
4. **Backhand Drive** - Drive de backhand
5. **Topspin** - Técnicas de topspin
6. **Loop contra Backspin** - Loop em bola cortada
7. **Bloqueio** - Técnicas de bloqueio
8. **Push / Jogo Curto** - Jogo curto na mesa
9. **Footwork** - Movimentação e deslocamento
10. **Estratégia e Tática** - Aspectos táticos
11. **Pino Longo - Técnicas** - Como usar pino longo
12. **Pino Longo - Jogar Contra** - Como enfrentar pino longo
13. **Pino Curto / Médio** - Borrachas de pino curto
14. **Defesa / Chopper** - Estilo defensivo
15. **Equipamentos** - Raquetes e borrachas
16. **Treinos e Drills** - Exercícios de treinamento
17. **Análise Profissional** - Análise de jogos profissionais
18. **Conteúdo Avançado** - Técnicas avançadas
19. **Iniciantes** - Fundamentos para iniciantes
20. **Shorts Técnicos** - Vídeos curtos técnicos

## 🔧 Instalação e Configuração

### Pré-requisitos

- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Chave da YouTube Data API v3

### Obtendo a API Key

1. Acesse o [Google Cloud Console](https://console.cloud.google.com/)
2. Crie um novo projeto ou selecione um existente
3. Ative a **YouTube Data API v3**
4. Vá em "Credenciais" e crie uma **API Key**
5. (Opcional) Restrinja a chave para uso apenas da YouTube Data API v3

### Executando o Projeto

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/table-tennis-video-hub.git
cd table-tennis-video-hub
```

2. Abra o arquivo `index.html` em um servidor web local:
```bash
# Usando Python 3
python -m http.server 8000

# Usando Node.js (http-server)
npx http-server

# Ou simplesmente abra o index.html no navegador
```

3. Acesse no navegador: `http://localhost:8000`

4. Insira sua YouTube API Key quando solicitado

## 💡 Como Usar

1. **Primeira Vez**: Insira sua API Key do YouTube quando o modal aparecer
2. **Navegar**: Clique em qualquer categoria na barra lateral
3. **Buscar**: Digite no campo de busca para encontrar vídeos específicos
4. **Assistir**: Clique em qualquer vídeo para reproduzi-lo no player integrado
5. **Carregar Mais**: Clique no botão "Carregar Mais Vídeos" para ver mais conteúdo
6. **Trocar API**: Use o botão "Trocar API Key" no topo da sidebar

## 🎨 Recursos Visuais

- **Glassmorphism**: Efeito de vidro moderno com blur
- **Gradientes Dinâmicos**: Cores vibrantes (azul → roxo → rosa)
- **Animações Suaves**: Transições e hover effects
- **Cards Interativos**: Efeito de elevação e bordas animadas
- **Loading States**: Spinners e feedback visual
- **Dark Mode**: Design otimizado para tema escuro

## 📱 PWA (Progressive Web App)

O projeto pode ser instalado como aplicativo:

1. No Chrome/Edge: Clique no ícone de instalação na barra de endereços
2. No Safari (iOS): "Adicionar à Tela de Início"
3. Funciona offline após a primeira visita

## 🔒 Segurança e Privacidade

- ✅ API Key armazenada apenas no navegador (sessionStorage)
- ✅ Sem envio de dados para servidores externos
- ✅ Conexão segura com YouTube via HTTPS
- ✅ Sem cookies ou rastreamento de usuários

## ⚠️ Limitações da API

A YouTube Data API v3 tem quotas diárias:

- **10.000 unidades/dia** (conta gratuita)
- Cada busca consome aproximadamente 100 unidades
- ~100 buscas por dia no plano gratuito

**Dica**: Use a API Key com moderação ou considere upgrade para quotas maiores.

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um Fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/MinhaFeature`)
3. Commit suas mudanças (`git commit -m 'Adiciona MinhaFeature'`)
4. Push para a branch (`git push origin feature/MinhaFeature`)
5. Abra um Pull Request

## 📝 Melhorias Futuras

- [ ] Sistema de favoritos com localStorage persistente
- [ ] Filtros por canal/duração/data
- [ ] Modo de visualização lista/grid
- [ ] Playlists personalizadas
- [ ] Sistema de notas/comentários
- [ ] Integração com outras plataformas de vídeo
- [ ] Tradução automática de títulos
- [ ] Estatísticas de visualização

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Autor

Desenvolvido com ❤️ para a comunidade de tênis de mesa

## 🙏 Agradecimentos

- YouTube Data API v3
- Tailwind CSS
- Comunidade de tênis de mesa
- Todos os criadores de conteúdo educacional

---

**⭐ Se este projeto foi útil, considere dar uma estrela no GitHub!**

## 📞 Suporte

Encontrou um bug ou tem uma sugestão? Abra uma [issue](https://github.com/seu-usuario/table-tennis-video-hub/issues)!

---

**🏓 Bons treinos!**
