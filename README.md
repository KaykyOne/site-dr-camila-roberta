# Site Dra. Camila Roberta

Site institucional de uma clínica odontológica em Campinas, com foco em odontologia estética, harmonização orofacial e atendimento humanizado.

## Visão geral

O projeto é um site estático em uma única página, com navegação por âncoras para as principais seções:

- Início
- A Clínica
- Tratamentos
- Diferenciais
- Depoimentos
- Sobre a Dra.
- Clínica
- Contato

O layout prioriza apresentação visual, chamadas para WhatsApp, galeria de fotos, depoimentos e informações de contato.

## Domínio temporário

O texto `TROCARPELOREAL` é um marcador provisório para tudo que depende do domínio público do site. Ele deve ser substituído em todos os pontos em que a URL final aparecer, como:

- `og:url` no `index.html`
- `canonical` no `index.html`
- `loc` no `sitemap.xml`

Enquanto o domínio final não for definido, o projeto mantém esse marcador para evitar URLs erradas ou antigas no código.

## Estrutura do projeto

- `index.html` - página principal do site.
- `css/` - estilos do tema, plugins e variáveis.
- `js/` - scripts de comportamento, animações, galeria, carrossel e integração visual.
- `img/` - imagens do site, separadas por categoria.
- `fonts/` - fontes e arquivos auxiliares do tema, se aplicável.
- `sitemap.xml` - mapa do site para SEO.

## Dependências front-end

O site usa bibliotecas e plugins já incluídos localmente:

- Bootstrap
- jQuery
- Owl Carousel
- Magnific Popup
- Isotope
- Stellar
- CounterUp
- Waypoints
- ScrollIt
- Particles.js

Também há carregamento de fonte externa via Google Fonts.

## Imagens e formatos

Parte dos assets de imagem foi convertida para `.webp` para reduzir peso e manter performance. No `index.html`, os caminhos já foram atualizados para os arquivos convertidos quando eles existem.

### Pastas que já usam `.webp`

- `img/banners/`
- `img/diferenciais/`
- `img/especialidades/`
- `img/fotos/`
- `img/numbers/`
- `img/doutoras/`

### Arquivos que continuam em outro formato

Os arquivos abaixo ainda permanecem em `.png` porque não havia versão `.webp` correspondente no momento da atualização:

- `img/favicon.png`
- `img/botao_whatsapp.png`
- `img/logo/logo_completa.png`
- `img/banners/avatart.png`

## Como executar localmente

Como é um site estático, basta abrir o `index.html` em um navegador. Para evitar limitações de acesso a recursos locais, também é possível servir a pasta por um servidor simples.

Exemplos:

- Abrir o `index.html` diretamente no navegador.
- Usar uma extensão de live server no editor.
- Usar qualquer servidor estático local da sua preferência.

## Manutenção

- Quando converter novas imagens para `.webp`, atualize os respectivos `src` e `data-background` no `index.html`.
- Se mudar a URL pública do site, revise os campos `og:url` e `canonical`, que ainda podem exigir ajuste final.
- Mantenha os nomes dos arquivos consistentes para evitar quebrar galeria, banners e seções com background.

## SEO e compartilhamento

O projeto inclui metadados básicos de SEO e Open Graph, como título, descrição, imagem de compartilhamento e canonical. Quando o domínio final for informado, substitua o marcador `TROCARPELOREAL` em todos os pontos de URL antes de publicar.

## Observações

- O site foi montado para funcionar como landing page institucional.
- A navegação interna é feita por âncoras e atributos `data-scroll-index`.
- Vários elementos visuais dependem dos arquivos de imagem dentro de `img/`.