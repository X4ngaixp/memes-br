# 🚀 Como Fazer Deploy da Pinterest Memes API

## 📋 Situação Atual
✅ **API funcionando localmente** em `http://localhost:5000`
✅ **Repositório Git criado** e commitado  
✅ **20 memes sendo extraídos** do Pinterest
❌ **Railway limitado** (só databases no plano gratuito)

---

## 🌟 **OPÇÃO 1: RENDER (Recomendado - 100% Gratuito)**

### **Passo a Passo:**

1. **Criar conta no GitHub** (se não tiver):
   - Acesse: https://github.com
   - Crie uma conta gratuita

2. **Fazer upload do código para GitHub**:
   ```bash
   # No seu terminal (na pasta do projeto):
   git remote add origin https://github.com/SEU-USUARIO/pinterest-memes-api.git
   git branch -M main
   git push -u origin main
   ```
   
   **OU use a interface do GitHub:**
   - Clique em "Upload files"
   - Arraste todos os arquivos da pasta `memes br`
   - Commit as changes

3. **Deploy no Render**:
   - Acesse: https://render.com
   - Faça login com GitHub
   - Clique "New" → "Web Service"
   - Conecte seu repositório GitHub
   - Configure:
     - **Name**: `pinterest-memes-api`
     - **Build Command**: `pip install -r requirements.txt`
     - **Start Command**: `python pinterest_memes_api.py`
   - Clique "Create Web Service"

4. **Aguarde o deploy** (2-3 minutos)

5. **Sua API estará em**: `https://pinterest-memes-api.onrender.com`

---

## 🌟 **OPÇÃO 2: VERCEL (Simples)**

1. **Instalar Vercel CLI**:
   ```bash
   npm install -g vercel
   ```

2. **Deploy**:
   ```bash
   cd "C:\Users\xangai\Documents\memes br"
   vercel
   ```

3. **Seguir instruções** no terminal

---

## 🌟 **OPÇÃO 3: NGROK (Para teste rápido)**

1. **Instalar ngrok**: https://ngrok.com/download

2. **Executar API localmente**:
   ```bash
   python pinterest_memes_api.py
   ```

3. **Em outro terminal**:
   ```bash
   ngrok http 5000
   ```

4. **Usar a URL pública** que aparece (ex: `https://abc123.ngrok.io`)

---

## 🔧 **Atualizar Google Sites após Deploy**

Depois que sua API estiver online, atualize o JavaScript no Google Sites:

```javascript
// ALTERE ESTA LINHA:
const API_BASE_URL = 'http://localhost:5000';

// PARA SUA URL DO RENDER:
const API_BASE_URL = 'https://pinterest-memes-api.onrender.com';
```

---

## 📱 **Teste Final**

Depois do deploy, teste sua API:

1. **Status**: `https://sua-api.onrender.com/`
2. **Memes**: `https://sua-api.onrender.com/api/memes/br?count=5`
3. **Batch**: `https://sua-api.onrender.com/api/memes/br/batch?count=8`

---

## 🎯 **Resumo - Qual Escolher?**

| Opção | Tempo | Dificuldade | Duração | HTTPS |
|-------|-------|-------------|---------|-------|
| **Render** | 5 min | ⭐⭐ | Permanente | ✅ |
| **Vercel** | 3 min | ⭐ | Permanente | ✅ |
| **Ngrok** | 1 min | ⭐ | Temporário | ✅ |

**🏆 Recomendação: Render** (gratuito e permanente)

---

## ⚡ **Solução SUPER RÁPIDA - Ngrok**

Se quiser testar AGORA:

1. **Baixe ngrok**: https://ngrok.com/download
2. **Execute no terminal**:
   ```bash
   # Terminal 1 (deixe rodando):
   python pinterest_memes_api.py
   
   # Terminal 2:
   ngrok http 5000
   ```
3. **Copie a URL** (ex: `https://abc123.ngrok.io`)
4. **Use no Google Sites**!

---

## 🔄 **Próximos Passos**

1. ✅ **Escolha uma opção** de deploy
2. ✅ **Faça o deploy** da API  
3. ✅ **Atualize o Google Sites** com a nova URL
4. ✅ **Teste** os memes carregando
5. ✅ **Compartilhe** seu site funcionando! 🎉

---

**🎭 Sua API do Pinterest está pronta! Escolha uma opção e vamos colocar online!** 