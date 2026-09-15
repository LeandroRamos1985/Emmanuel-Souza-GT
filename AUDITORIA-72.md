# Auditoria real dos 72 itens — Emmanuel Souza

Data: 15/09/2026. **45 aprovados · 25 atenção · 0 falhou · 2 não aplicáveis.** Score estrito: 64.3% dos critérios aplicáveis. Cobertura 72/72. Atenção não equivale a aprovação; este score não é a nota Lighthouse.

Estado: demonstração pública no GitHub Pages verificada. A demonstração não afirma CRM/LeadPilot ou analytics ativos. Não foi realizada alteração do site/domínio atual do cliente. Formulário oferece WhatsApp real sem alegar entrega quando não há gateway. Operação definitiva com envio de leads exige endpoint e revisão dos documentos/disclosures pelo titular.

## Evidências reais
- evidence/browser-audit.json: nove cenários de navegador, 34 rotas, três formulários e zero links internos quebrados; erros HTTP de teste 500/404 deliberados. O teste preliminar registrou também uma requisição de favicon padrão; o reteste final não registrou erro HTTP.
- evidence/responsive-final.json: 21 cenários, zero overflow, zero erros JavaScript e zero respostas HTTP de erro.
- evidence/tracking-final.json: espaços, consentimento, honeypot, UTMs e confirmação local testados; zero erros JavaScript e zero violações Axe WCAG 2.2 no mobile.
- evidence/seo-audit.json: 33 títulos e descrições únicos, canonical/hreflang, schema e sitemap.
- evidence/lighthouse-desktop.html/json e lighthouse-mobile.html/json: desempenho 100/95, acessibilidade e boas práticas 100/100. SEO 66/66 por noindex deliberado. LCP ~0,52/2,93 s; CLS <0,001; TBT 0.
- evidence/external-links.json: destinos externos e limites HTTP 403/406 registrados; não certifica recebimento de canais.
- Capturas mobile-final.png e desktop-final.png; dispositivos emulados, sem validação em telefone físico.
- FONTES-DO-CLIENTE.md e MEDIA-VERIFICADA.md: dados profissionais, licença oficial atual, mídia escolhida, pesquisa de reutilização, licença e limites.
- evidence/github-pages-live.json e github-pages-mobile.png: HTTPS público, três idiomas, vídeo e controle de pausa verificados.

## Os 72 itens

| Nº | Critério | Status | Evidência / limite |
|---|---|---|---|
| 1 | CTA principal na primeira dobra | Aprovado | CTA principal para WhatsApp na primeira dobra em 21 cenários, incluindo 320 px; capturas e coordenadas em responsive-final.json. |
| 2 | CTAs claros e consistentes | Aprovado | Serviços de moradia/alto padrão e temporada selecionam o objetivo do contato; seleção de comprar, vender e investir disponível no formulário. |
| 3 | CTA fixo no mobile, quando adequado | Aprovado | WhatsApp fixo no mobile; vídeo em seção separada e controle acessível por rolagem. Testes reais de pausa e retomada. |
| 4 | Promessa/expectativa de tempo de resposta, quando aplicável | Não aplicável | Prazo de resposta não fornecido; não foi inventado. |
| 5 | Página de obrigado após conversão | Atenção | Obrigado nos três idiomas somente após confirmação explícita do servidor local. Gateway real não conectado. |
| 6 | Formulários com validação e estados de erro/sucesso | Atenção | Nome vazio/espaços, e-mail inválido, consentimento, HTTP 500 e retry testados. Atendimento real depende de endpoint. |
| 7 | Links e URLs amigáveis/personalizados | Aprovado | 35 arquivos HTML estáticos, caminhos relativos e diretórios legíveis; 34 rotas renderizadas, entrada redireciona a PT-BR. |
| 8 | Seção de cases/resultados quando houver material autorizado | Não aplicável | Não há cases individuais autorizados e conferidos para reprodução. Link ao perfil profissional, sem resultados fabricados. |
| 9 | Avaliações reais e verificáveis | Atenção | Link aos relatos publicados na fonte do cliente. Não foram certificados depoimentos ou notas individualmente; não exibimos citações ou estrelas. |
| 10 | Mapas, endereço e rotas | Aprovado | Escritório 500 Celebration Ave. conferido no site fornecido; Maps e rotas HTTP 200. Sem embed antecipado. |
| 11 | Responsividade completa para celular, tablet e desktop | Aprovado | 21 cenários: 320/360/375/390/768/1024/1440 px × três idiomas. Zero overflow. |
| 12 | Meta title único por página | Aprovado | 33 páginas por idioma/conteúdo/utilidade com títulos únicos; seo-audit.json. |
| 13 | Meta description única por página | Aprovado | 33 descrições únicas verificadas por código, sem copiar snippets do site antigo. |
| 14 | H1 único e hierarquia correta de H2/H3 | Aprovado | Um H1 por página renderizada; estrutura H2/H3. Axe sem violações nos nove cenários principais. |
| 15 | Títulos e conteúdo sem duplicações desnecessárias | Aprovado | Conteúdo próprio em três idiomas e seis regiões por idioma; sem duplicação dos blocos editoriais antigos. |
| 16 | Alt text contextual nas imagens | Aprovado | Retrato e marca identificados nos alts; vídeo editorial descrito por idioma; palavra decorativa oculta de leitores de tela. |
| 17 | Breadcrumbs quando fizerem sentido | Aprovado | 18 páginas de comunidades com retorno útil; links conferidos em navegador. |
| 18 | FAQ + dados estruturados de FAQ somente quando aplicáveis | Aprovado | FAQ visível e funcional com quatro perguntas por idioma; sem FAQ Schema artificial ou promessa de retorno. |
| 19 | URLs amigáveis | Aprovado | Slugs consistentes de regiões, idiomas e páginas legais. |
| 20 | Canonical tags | Aprovado | Canonical absoluto preparado para o endereço deste repositório GitHub; 33 páginas conferidas. Demonstração permanece noindex. |
| 21 | robots.txt | Aprovado | robots.txt bloqueia rastreamento da demonstração; não é o robots de um futuro domínio oficial. |
| 22 | sitemap.xml | Aprovado | Sitemap com 27 URLs de conteúdo para esta demonstração. Rotas obrigado e 404 excluídas. Noindex mantido deliberadamente. |
| 23 | Página 404 personalizada | Aprovado | 404 própria na raiz e em três idiomas; HTTP 404 real testado e retorno ao início adequado ao subdiretório GitHub. |
| 24 | Favicon | Aprovado | Favicon ES em SVG local e referência em todos os heads do site. |
| 25 | Open Graph | Atenção | OG por página, imagem absoluta e twitter card preparados. Scrapers/redes sociais não foram certificados. |
| 26 | Imagem adequada para compartilhamento social | Aprovado | Composição própria de marca 1200×630 JPEG, cerca de 35 KB. |
| 27 | Dados estruturados LocalBusiness ou tipo mais específico aplicável | Aprovado | RealEstateAgent JSON-LD parseado nas 33 páginas; telefone, endereço, corretor e brokerage cruzados com fontes. Sem avaliação ou inventário fictício. |
| 28 | Google Search Console configurável após domínio/verificação | Atenção | Search Console não conectado; demonstração não solicita indexação. Verificação depende do domínio oficial e da conta do titular. |
| 29 | Verificação automática de links quebrados | Atenção | Zero links internos quebrados. WA/Maps HTTP 200; site do cliente 406 e Homes 403 no cliente HTTP. Site atual renderizado em navegador; proteções externas limitam automação. |
| 30 | Indexabilidade das páginas verificada | Atenção | Noindex/robots de demonstração conferidos. Indexação do futuro domínio oficial depende de migração e configuração próprias. |
| 31 | Compressão e otimização automática de imagens | Aprovado | Retrato PNG 169.810 bytes convertido para WebP 31.626 bytes. Posters otimizados; derivação proporcional documentada. |
| 32 | Formatos modernos de imagem quando adequados | Aprovado | WebP para retrato/posters, SVG para favicon e JPEG para compartilhamento social. |
| 33 | Lazy loading | Aprovado | Retrato abaixo da dobra lazy; vídeo preload metadata e variante mobile específica. |
| 34 | Teste de PageSpeed/Lighthouse | Aprovado | Lighthouse real 13.4.1: relatórios HTML/JSON desktop e mobile preservados. |
| 35 | Core Web Vitals | Atenção | LCP desktop ~0,52 s e mobile ~2,93 s; CLS <0,001, TBT 0. INP e CWV de campo não medidos; mobile LCP acima de 2,5 s no ensaio. |
| 36 | Otimização de carregamento de fontes, CSS e JavaScript | Aprovado | CSS ~12 KB, JS ~5,8 KB, adaptador ~1,1 KB, fonte local ~48 KB com swap. Sem framework em runtime. |
| 37 | HTTPS/SSL | Aprovado | HTTPS público confirmado com resposta 200 no GitHub Pages. |
| 38 | Headers e configurações básicas de segurança | Atenção | Sem segredos em front-end; links externos noopener. GitHub Pages não oferece aplicação de headers arbitrários. Backend/gateway não auditado. |
| 39 | Proteção anti-spam/bot nos formulários | Atenção | Honeypot bloqueou envio no teste; defesa server-side e rate limit dependem do gateway real. |
| 40 | Tratamento seguro dos dados enviados | Atenção | Payload não entra em analytics/storage. Endpoint remoto exige HTTPS, timeout e confirmação. Recebimento/retensão real dependem do serviço conectado. |
| 41 | Política de Privacidade | Atenção | Políticas próprias em EN/PT-BR/ES. Titular deve revisar fornecedores, retenção e base jurídica conforme operação real. |
| 42 | Cookies/consentimento quando juridicamente necessário | Aprovado | Analytics opcional só carrega após configuração e consentimento. Recusa e preferências testadas; nenhum pixel ativo na demonstração. |
| 43 | Dados empresariais/profissionais no rodapé | Atenção | Nome, Talent Realty Solutions, licença SL3520316, endereço e canais reais no rodapé. Disclosures finais precisam da revisão da imobiliária. |
| 44 | Google Analytics ou solução equivalente | Atenção | Campo analyticsId GA4 configurável, sem ID ou conta fornecidos. Não se afirma recepção ativa. |
| 45 | Eventos de conversão configurados | Atenção | Eventos locais de CTA/WA/telefone/e-mail/externos/formulário preparados; conta de recebimento analytics não conectada. |
| 46 | Cliques em WhatsApp monitoráveis | Atenção | Evento whatsapp_click em links WA e fallback. Canal publicado e URL HTTP 200; recepção no GA4 ainda não configurada. |
| 47 | Envios de formulário monitoráveis | Atenção | Sucesso capturado depois do aceite explícito do servidor de teste. Nenhuma entrega real ao CRM. |
| 48 | Origem/campanha do lead preservada quando possível | Aprovado | UTM source/campaign whitelisted no payload real do teste; parâmetros pessoais não entram em eventos. Sem persistência entre sessões. |
| 49 | Integração com CRM do LeadPilot | Atenção | Adaptador e payload preparados. Não há credenciais/endpoint/documentação do LeadPilot disponíveis; integração ativa não certificada. |
| 50 | Teste real dos eventos antes da publicação | Atenção | Eventos UI e payload testados em navegador contra servidor local. GA4/LeadPilot ponta a ponta pendentes. |
| 51 | Logo e identidade visual | Aprovado | Marca real preservada, composição nova marfim/verde/bronze e tipografia editorial. Layout distinto do Allan. |
| 52 | Informações reais do negócio | Aprovado | FONTES-DO-CLIENTE.md documenta site próprio, perfil profissional e portal oficial ao vivo. Sem estatísticas não conferidas. |
| 53 | Telefone/WhatsApp conferidos | Aprovado | Telefone +14076071138 e WhatsApp wa.me/14076071138 coincidem com o site atual; número usado em todos os links. |
| 54 | Endereço e horários conferidos | Atenção | Endereço conferido na fonte do cliente. Horários não fornecidos e não inventados; confirmação operacional ainda cabe ao titular. |
| 55 | Serviços/especialidades conferidos | Aprovado | Compra/venda, moradia/temporada/alto padrão e regiões correspondem à fonte profissional. |
| 56 | Fotos reais autorizadas | Aprovado | Retrato e logo reais da fonte fornecida para o projeto; vídeo Pexels licenciado. Pesquisa prévia e limitações em MEDIA-VERIFICADA.md. |
| 57 | Informações da equipe/profissionais conferidas | Aprovado | Identidade e brokerage cruzadas; SL3520316 Current / Active, expiração 09/30/2027, no portal regulatório ao vivo em 15/09/2026. |
| 58 | Avaliações reais sem fabricação por IA | Aprovado | Sem depoimentos, notas, estrelas ou Review Schema gerados. Encaminhamento aos relatos na fonte do próprio corretor. |
| 59 | Conteúdo adaptado ao segmento e localização | Aprovado | Orlando/Central Florida, seis regiões e três jornadas, com textos próprios EN/PT-BR/ES. |
| 60 | Revisão de informações sensíveis ou regulamentadas | Atenção | Licença profissional conferida no órgão oficial ao vivo. Evitadas promessas e taxas antigas; política/disclosures precisam de aprovação profissional. |
| 61 | Teste desktop | Aprovado | Edge real, desktop 1440 px e capturas da página completa. |
| 62 | Teste mobile | Aprovado | Edge com sete larguras e viewport mobile emulado. Não são aparelhos físicos. |
| 63 | Teste de todos os formulários | Atenção | Formulários dos três idiomas testados com erro, sucesso local, UTMs, nome, consentimento e honeypot. Entrega ao titular/CRM não conectada. |
| 64 | Teste de todos os CTAs | Aprovado | Navegação, CTAs internos, FAQ, idiomas, comunidades, legal e objetivos exercitados; zero links internos quebrados. Canais externos sem envio de mensagens. |
| 65 | Teste dos links externos | Atenção | HTTP e renderização externa conferidos com limites de proteção 403/406; não se certifica disponibilidade contínua dos fornecedores. |
| 66 | Teste de WhatsApp, telefone e e-mail | Atenção | WA/tel/mailto com dados reais e destinos corretos; sem ligação, mensagem ou e-mail de teste ao corretor. Recebimento operacional não certificado. |
| 67 | Auditoria SEO | Aprovado | 33 títulos/descrições únicos, canonical/hreflang/OG, schema válido e sitemap 27 URLs; noindex da demonstração verificado. |
| 68 | Auditoria de acessibilidade básica | Aprovado | Axe: zero violações em nove cenários e mobile com WCAG 2.2. Lighthouse acessibilidade 100/100; menu Escape, labels e movimento reduzido testados. |
| 69 | Auditoria de performance | Aprovado | Performance Lighthouse 100 desktop / 95 mobile; boas práticas 100/100. Relatórios reais locais; nenhuma nota de campo inventada. |
| 70 | Auditoria de segurança | Atenção | Revisão de código, ausência de segredos, adapter HTTPS e separação de dados/eventos. Não constitui pentest do GitHub, CRM ou backend. |
| 71 | Verificação de domínio/SSL | Aprovado | Repositório e site HTTPS público conferidos. Não houve mudança no DNS ou no domínio oficial do cliente. |
| 72 | Site Quality Score final | Aprovado | 72 critérios classificados individualmente. Atenção não conta como aprovação; integração não disponível não recebe falso sucesso. |
