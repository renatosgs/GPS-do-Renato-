# 🚗 RadarBot Web Brasil (SP • PR • SC)

<p align="center">
  <img src="https://img.shields.io/badge/Status-100%25%20Funcional-success?style=for-the-badge&logo=checkmarx" alt="Status">
  <img src="https://img.shields.io/badge/Plataforma-Web%20%7C%20Mobile%20PWA-00f2fe?style=for-the-badge&logo=googlechrome" alt="Platform">
  <img src="https://img.shields.io/badge/Tecnologias-HTML5%20%7C%20JS%20%7C%20Leaflet-orange?style=for-the-badge&logo=javascript" alt="Tech">
  <img src="https://img.shields.io/badge/Licen%C3%A7a-MIT-blue?style=for-the-badge" alt="License">
</p>

<p align="center">
  <b>Um detector de radares inteligente e velocímetro digital em tempo real inspirado no Radarbot e Waze, projetado especificamente para as rodovias e capitais de São Paulo (SP), Paraná (PR) e Santa Catarina (SC).</b>
</p>

---

## 📸 Demonstração do Painel (HUD)

- 🏎️ **Velocímetro Digital Neon:** Display automotivo de alta visibilidade para uso diurno e noturno.
- 🛑 **Placa de Velocidade Oficial:** Ícone circular no padrão brasileiro com limite regulamentado da via (40, 50, 60, 70, 80, 90, 100, 110, 120 km/h).
- 🔊 **Alertas por Voz em Português (Web Speech API):** Anúncio falado com antecedência em metros (*"Atenção: Radar fixo a 500 metros, velocidade máxima 80 quilômetros por hora"*).
- 🚨 **Alerta de Excesso de Velocidade:** O velocímetro pisca em vermelho com bips sonoros e alerta imediato de redução.
- 🗺️ **Mapa Noturno (Leaflet + CartoDB Dark):** Mostra os pontos de fiscalização com marcadores coloridos e rastreamento da direção do carro (*heading*).

---

## 🛣️ Cobertura da Base de Dados Embutida

A base inicial já vem pré-carregada com os pontos de radar mais críticos das três unidades federativas:

### 🔵 São Paulo (SP)
* **Capitais e Avenidas:** Marginal Tietê (Expressa e Local), Marginal Pinheiros, Av. 23 de Maio, Av. Paulista, Radial Leste.
* **Rodovias Principais:** Rodovia dos Bandeirantes (SP-348), Rodovia Anhanguera (SP-330), Rodovia Castelo Branco (SP-280), Rodovia Ayrton Senna (SP-070), Rodovia Presidente Dutra (BR-116), Rodovia dos Imigrantes (SP-160), Rodovia Anchieta (SP-150), Rodovia Régis Bittencourt (BR-116 Serra do Cafezal), Rodovia Dom Pedro I (SP-065).

### 🟢 Paraná (PR)
* **Curitiba e Região Metropolitana:** Linha Verde (BR-476 Norte e Sul), Av. das Torres (Comendador Franco), Av. Marechal Floriano Peixoto, Contorno Leste e Contorno Sul (BR-116).
* **Rodovias Principais:** BR-277 (Curitiba ➔ Morretes / Serra do Mar e Curitiba ➔ Campo Largo / Ponta Grossa / Cascavel / Foz do Iguaçu), BR-376 (Curitiba ➔ Tijucas do Sul / Serra de Guaratuba), Rodovia do Café, BR-369 (Londrina / Cambé), Av. Colombo (Maringá).

### 🟡 Santa Catarina (SC)
* **Eixo Litoral BR-101:** Joinville (Acesso Norte e Sul), Navegantes, Itajaí, Balneário Camboriú (Morro do Boi), Itapema (Túnel), Biguaçu, São José, Palhoça (Morro dos Cavalos), Tubarão e Criciúma.
* **Florianópolis e Serra:** BR-282 (Via Expressa Continental de Florianópolis e Chapecó), Av. Beira-Mar Norte, SC-401 (Norte da Ilha), SC-405 (Sul da Ilha / Aeroporto), BR-470 (Blumenau / Vale do Itajaí), BR-280 (Guaramirim / Jaraguá do Sul).

---

## 🚀 Como Publicar Gratuitamente no GitHub Pages

O navegador exige uma conexão segura **HTTPS** para autorizar o acesso contínuo ao GPS do celular. O GitHub Pages oferece isso nativamente e sem custos:

1. No seu GitHub, clique em **New Repository** e dê um nome (ex: `radarbot-web`).
2. Marque como **Public** e faça o envio do arquivo `index.html` e deste `README.md`.
3. No seu repositório, clique na aba **Settings** (Configurações) no topo.
4. No menu lateral esquerdo, clique em **Pages**.
5. Na seção **Build and deployment > Source**, selecione:
   - **Branch:** `main` (ou `master`)
   - **Folder:** `/ (root)`
6. Clique no botão **Save**.
7. Aguarde cerca de 1 a 2 minutos. O GitHub exibirá o link público:
   ```text
   https://seu-usuario.github.io/radarbot-web/
