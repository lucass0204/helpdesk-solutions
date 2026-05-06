# 🛠️ Problema: Computador sem acesso à internet

## 📌 Descrição

Usuário relata que está conectado ao Wi-Fi, porém não consegue acessar sites.

## 🔍 Diagnóstico

* Teste com `ping 8.8.8.8` → sem resposta
* Verificação com `ipconfig` mostrou IP inválido

## 🧠 Possível causa

Falha na obtenção de IP automático (DHCP)

## ✅ Solução

1. Abrir o Prompt de Comando como administrador
2. Executar:

   * ipconfig /release
   * ipconfig /renew
3. Testar novamente a conexão

## 📈 Resultado

Conexão restabelecida com sucesso
