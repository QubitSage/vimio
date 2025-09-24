# 🚀 Guia de Deploy - Villa La Colline

## 📦 **Arquivos Gerados**

**Arquivo principal**: `villa-la-colline-deploy.zip` (861KB)

### **Conteúdo do pacote:**
```
dist/
├── index.html (3.2KB) - Página principal
├── favicon.ico (15KB) - Ícone do site
└── assets/
    ├── index-XelMMipz.css (94KB) - Estilos CSS
    ├── index-ncDy5YWJ.js (201KB) - JavaScript React
    ├── slide1-CVGkBy4_.jpg (202KB) - Foto sala de estar
    ├── slide2-C3hzfB_q.jpg (121KB) - Foto mesa de jantar
    ├── slide3-C20EXVHW.jpg (164KB) - Foto sala integrada
    ├── slide4-C8Nrkng1.jpg (198KB) - Foto sala com lareira
    └── slide5-DOS_IR_d.jpg (111KB) - Foto mesa de jantar 2
```

## 🌐 **Opções de Hospedagem**

### **1. Netlify (Recomendado - Gratuito)**
1. Acesse [netlify.com](https://netlify.com)
2. Faça login/cadastro
3. Arraste o arquivo ZIP na área "Deploy"
4. Seu site estará online em segundos
5. Configure domínio personalizado (opcional)

### **2. Vercel (Gratuito)**
1. Acesse [vercel.com](https://vercel.com)
2. Conecte com GitHub ou faça upload direto
3. Arraste a pasta `dist/` 
4. Deploy automático

### **3. GitHub Pages (Gratuito)**
1. Crie repositório no GitHub
2. Faça upload dos arquivos da pasta `dist/`
3. Ative GitHub Pages nas configurações
4. Site disponível em `username.github.io/repo-name`

### **4. Servidor Próprio (cPanel/FTP)**
1. Extraia o arquivo ZIP
2. Faça upload da pasta `dist/` via FTP
3. Aponte o domínio para a pasta
4. Configure SSL/HTTPS

## ⚙️ **Configurações Importantes**

### **🔧 Servidor Web**
- **Tipo**: Site estático (HTML/CSS/JS)
- **HTTPS**: Obrigatório (Meta Pixel requer SSL)
- **Compressão**: Ativar GZIP para melhor performance
- **Cache**: Configurar cache para assets (imagens, CSS, JS)

### **📱 Headers Recomendados**
```
# .htaccess (Apache) ou nginx.conf
# Cache para assets
<IfModule mod_expires.c>
    ExpiresActive On
    ExpiresByType image/jpg "access plus 1 month"
    ExpiresByType image/jpeg "access plus 1 month"
    ExpiresByType text/css "access plus 1 month"
    ExpiresByType application/javascript "access plus 1 month"
</IfModule>

# Compressão GZIP
<IfModule mod_deflate.c>
    AddOutputFilterByType DEFLATE text/plain
    AddOutputFilterByType DEFLATE text/html
    AddOutputFilterByType DEFLATE text/css
    AddOutputFilterByType DEFLATE application/javascript
</IfModule>
```

## 🎯 **Verificação Pós-Deploy**

### **✅ Checklist Essencial**
- [ ] Site carrega corretamente
- [ ] Todas as imagens aparecem
- [ ] Slideshow funciona
- [ ] Formulário de cotação funciona
- [ ] WhatsApp abre corretamente
- [ ] Galeria de fotos funciona
- [ ] Mapa carrega
- [ ] Site responsivo (mobile/tablet)
- [ ] Meta Pixel funcionando

### **🔍 Testes Importantes**

**1. Teste de Conversão**
- Preencha o formulário
- Clique em "COTE JÁ"
- Verifique se abre WhatsApp
- Confirme se Meta Pixel registra evento "Lead"

**2. Teste Mobile**
- Acesse pelo celular
- Teste navegação touch
- Verifique formulário mobile
- Confirme velocidade de carregamento

**3. Teste Meta Pixel**
- Instale extensão "Meta Pixel Helper"
- Acesse o site
- Verifique eventos: PageView, Lead, ViewContent
- Confirme no Meta Business Manager

## 📊 **Monitoramento**

### **🎯 Meta Pixel (Configurado)**
- **ID**: 1497289184608755
- **Eventos**: PageView, Lead, ViewContent, InitiateCheckout
- **Status**: ✅ Ativo

### **📈 Google Analytics (Opcional)**
Para adicionar GA4:
1. Crie conta no Google Analytics
2. Substitua `GA_MEASUREMENT_ID` no index.html
3. Faça novo deploy

### **🔥 Hotjar (Opcional)**
Para adicionar heatmaps:
1. Crie conta no Hotjar
2. Substitua `YOUR_HOTJAR_ID` no index.html
3. Faça novo deploy

## 🚀 **Performance**

### **📊 Métricas Atuais**
- **Tamanho total**: 861KB (otimizado)
- **Imagens**: Comprimidas para web
- **CSS/JS**: Minificados
- **Carregamento**: < 3 segundos

### **⚡ Otimizações Aplicadas**
- Lazy loading para imagens
- CSS e JS minificados
- Imagens otimizadas (JPEG, qualidade 85%)
- Fonte Lora carregada via Google Fonts

## 🔒 **Segurança**

### **✅ Implementado**
- Meta tags de segurança
- HTTPS obrigatório para Meta Pixel
- Validação de formulário
- Sanitização de inputs

### **🛡️ Recomendações**
- Sempre usar HTTPS
- Configurar CSP (Content Security Policy)
- Monitorar tentativas de spam
- Backup regular do site

## 📞 **Suporte**

### **🐛 Problemas Comuns**

**Meta Pixel não funciona:**
- Verifique se site está em HTTPS
- Confirme ID do pixel: 1497289184608755
- Use Meta Pixel Helper para debug

**WhatsApp não abre:**
- Verifique número: +55 11 93394-1595
- Teste em diferentes dispositivos
- Confirme se mensagem está formatada

**Site lento:**
- Ative compressão GZIP
- Configure cache do navegador
- Use CDN se necessário

### **📧 Contato**
Para suporte técnico, consulte a documentação da plataforma de hospedagem escolhida.

---

## 🎯 **Próximos Passos**

1. **Deploy do site** (escolha uma opção acima)
2. **Teste todas as funcionalidades**
3. **Verificar Meta Pixel no Business Manager**
4. **Criar primeira campanha** (use o guia META_CAMPAIGNS_GUIDE.md)
5. **Monitorar conversões e otimizar**

**Seu site está pronto para gerar leads e conversões! 🚀**
