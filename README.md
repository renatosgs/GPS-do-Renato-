# 🚗 RadarBot Web Brasil (SP • PR • SC)

<p align="center">
  <img src="https://img.shields.io/badge/Status-100%25%20Funcional-success?style=for-the-badge&logo=checkmarx" alt="Status">
  <img src="https://img.shields.io/badge/Plataforma-Web%20%7C%20Mobile-00f2fe?style=for-the-badge&logo=googlechrome" alt="Platform">
  <img src="https://img.shields.io/badge/Tecnologias-HTML5%20%7C%20JS%20%7C%20Leaflet-orange?style=for-the-badge&logo=javascript" alt="Tech">
  <img src="https://img.shields.io/badge/iOS%20%7C%20Android-Compatible-10b981?style=for-the-badge&logo=apple" alt="Mobile">
  <img src="https://img.shields.io/badge/Licen%C3%A7a-MIT-blue?style=for-the-badge" alt="License">
</p>

<p align="center">
  <b>Detector de radares inteligente + velocímetro digital em tempo real, inspirado no Radarbot e Waze, projetado especificamente para as rodovias e capitais de São Paulo (SP), Paraná (PR) e Santa Catarina (SC).</b>
</p>

<p align="center">
  <a href="#-demonstração-do-painel-hud">Demonstração</a> •
  <a href="#-cobertura-da-base-de-dados">Cobertura</a> •
  <a href="#-como-publicar-gratuitamente-no-github-pages">Publicar</a> •
  <a href="#-como-ativar-o-gps-no-iphone-passo-a-passo">GPS no iPhone</a> •
  <a href="#-como-usar">Como Usar</a> •
  <a href="#-importação-de-dados">Importar</a> •
  <a href="#-tecnologias-utilizadas">Tecnologias</a> •
  <a href="#-faq--solução-de-problemas">FAQ</a>
</p>

---

## 📖 Índice

- [Demonstração do Painel (HUD)](#-demonstração-do-painel-hud)
- [Cobertura da Base de Dados](#-cobertura-da-base-de-dados)
- [Como Publicar no GitHub Pages](#-como-publicar-gratuitamente-no-github-pages)
- [Como Ativar o GPS no iPhone](#-como-ativar-o-gps-no-iphone-passo-a-passo)
- [Como Usar](#-como-usar)
- [Importação de Dados](#-importação-de-dados)
- [Arquitetura Técnica](#-arquitetura-técnica)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Compatibilidade de Navegadores](#-compatibilidade-de-navegadores)
- [FAQ / Solução de Problemas](#-faq--solução-de-problemas)
- [Roadmap Futuro](#-roadmap-futuro)
- [Aviso Legal](#️-aviso-legal)
- [Licença](#-licença)
- [Créditos](#-créditos-e-agradecimentos)
- [Estrutura do Repositório](#-estrutura-do-repositório)

---

## 📸 Demonstração do Painel (HUD)

- 🏎️ **Velocímetro Digital Neon** — Display automotivo de alta visibilidade para uso diurno e noturno, com suavização de leitura e destaque de excesso de velocidade.
- 🛑 **Placa de Velocidade Oficial** — Ícone circular no padrão brasileiro (borda vermelha) exibindo o limite regulamentado da via (40 a 120 km/h).
- 🔊 **Alertas por Voz em Português** — Anúncio falado com antecedência em metros: *"Atenção: Radar fixo à frente a 500 metros. Limite de 80 quilômetros por hora."*
- 🚨 **Alerta de Excesso de Velocidade** — Velocímetro pisca em vermelho com 4 bips agudos e alerta imediato de redução.
- 🗺️ **Mapa Noturno (Leaflet + CartoDB Dark Matter)** — Mostra os pontos de fiscalização com marcadores coloridos, popups informativos e rastreamento da direção do carro.
- 📍 **GPS em Tempo Real** — Detecta velocidade, rumo e precisão; funciona para caminhada, bicicleta, moto e carro.
- 🚗 **Modo Simulação** — 6 rotas pré-configuradas para testar sem sair de casa, com slider de 30 a 150 km/h.
- 📂 **Base Editável** — Importa/exporta CSV e JSON, cadastra radares manualmente, pesquisa e remove pontos.

---

## 🛣️ Cobertura da Base de Dados

A base inicial já vem pré-carregada com **57 pontos de radar críticos** das três unidades federativas:

### 🔵 São Paulo (SP) — 22 pontos
- **Capital e Avenidas:** Marginal Tietê (Expressa e Local), Marginal Pinheiros, Av. 23 de Maio, Av. Paulista.
- **Rodovias Principais:** Rodovia dos Bandeirantes (SP-348), Rodovia Anhanguera (SP-330), Rodovia Castelo Branco (SP-280), Rodovia Ayrton Senna (SP-070), Rodovia Presidente Dutra (BR-116), Rodovia dos Imigrantes (SP-160), Rodovia Anchieta (SP-150), Rodovia Régis Bittencourt (BR-116), Rodovia Dom Pedro I (SP-065).

### 🟢 Paraná (PR) — 16 pontos
- **Curitiba e RMC:** Linha Verde (BR-476 Norte e Sul), Av. das Torres (Comendador Franco), Av. Marechal Floriano Peixoto, Contorno Leste e Contorno Sul (BR-116).
- **Rodovias Principais:** BR-277 (Serra do Mar, Campo Largo, Cascavel, Foz do Iguaçu), BR-376 (Tijucas do Sul, Serra de Guaratuba), Rodovia do Café, BR-369 (Londrina / Cambé), Av. Colombo (Maringá).

### 🟡 Santa Catarina (SC) — 19 pontos
- **Eixo Litoral BR-101:** Joinville, Navegantes, Itajaí, Balneário Camboriú (Morro do Boi), Itapema (Túnel), Biguaçu, São José, Palhoça (Morro dos Cavalos), Tubarão e Criciúma.
- **Florianópolis e Serra:** BR-282 (Via Expressa Continental e Chapecó), Av. Beira-Mar Norte, SC-401, SC-405, BR-470 (Blumenau), BR-280 (Guaramirim).

---

## 🚀 Como Publicar Gratuitamente no GitHub Pages

O navegador exige **HTTPS** para autorizar o GPS contínuo do celular. O GitHub Pages oferece isso nativamente e sem custos:

### Passo a Passo

1. No GitHub, clique em **New Repository** e crie um (ex: `radarbot-web`).
2. Marque como **Public** e envie os arquivos `index.html` e `README.md`.
3. Acesse a aba **Settings** do repositório.
4. No menu lateral esquerdo, clique em **Pages**.
5. Em **Build and deployment → Source**, selecione:
   - **Branch:** `main` (ou `master`)
   - **Folder:** `/ (root)`
6. Clique em **Save**.
7. Aguarde **1 a 2 minutos**. O link público aparecerá:

```text
https://seu-usuario.github.io/radarbot-web/
