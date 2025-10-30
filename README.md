# 👋🏻 Leonardo de Moura Fuseti

Estudante de Defesa Cibernetica no Polo Estacio Piumhi MG . Formação tecnica em Tecnico em Redes de Computadores no IFMG Bambui MG , intusiasta na programação gostando muito de Python e evoluindo dia a dia .

### Conecte-se comigo

[![Perfil DIO](https://img.shields.io/badge/-Meu%20Perfil%20na%20DIO-30A3DC?style=for-the-badge)](https://www.dio.me/users/mourafuseti)
[![E-mail](https://img.shields.io/badge/-Email-000?style=for-the-badge&logo=microsoft-outlook&logoColor=E94D5F)](mailto:mourafuseti@gmail.com)
[![LinkedIn](https://img.shields.io/badge/-LinkedIn-000?style=for-the-badge&logo=linkedin&logoColor=30A3DC)](https://www.linkedin.com/in/leonardo-moura-fuseti-4052b0359/)

### Habilidades

![HTML](https://img.shields.io/badge/HTML-000?style=for-the-badge&logo=html5&logoColor=30A3DC)
![CSS3](https://img.shields.io/badge/CSS3-000?style=for-the-badge&logo=css3&logoColor=E94D5F)
![JavaScript](https://img.shields.io/badge/JavaScript-000?style=for-the-badge&logo=javascript&logoColor=F0DB4F)
![Sass](https://img.shields.io/badge/SASS-000?style=for-the-badge&logo=sass&logoColor=CD6799)
![Bootstrap](https://img.shields.io/badge/bootstrap-000?style=for-the-badge&logo=bootstrap&logoColor=553C7B)
[![Git](https://img.shields.io/badge/Git-000?style=for-the-badge&logo=git&logoColor=E94D5F)](https://git-scm.com/doc)
[![GitHub](https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github&logoColor=30A3DC)](https://docs.github.com/)

### GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=mourafuseti&theme=transparent&bg_color=000&border_color=30A3DC&show_icons=true&icon_color=30A3DC&title_color=E94D5F&text_color=FFF)



![Python](https://img.shields.io/badge/python-3.8%2B-3670A0?logo=python&logoColor=ffdd54)
![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?logo=kalilinux)
![Root Required](https://img.shields.io/badge/Root-Required-red)
![License](https://img.shields.io/badge/license-All%20Rights%20Reserved-critical)
![Version](https://img.shields.io/badge/version-8.1-success)



---

```markdown
# SCANFULL v8.1 - Metaexploit GUI Wrapper



> Interface gráfica (GUI) em **Tkinter** para automatizar e simplificar o uso do **Metasploit
(metaexploit)** com exploits comuns em um clique.

---

## Autor
**Leonardo de Moura Fuseti**  
© 2025 - Todos os direitos reservados

---

## Descrição

O **SCANFULL v8.1** é uma ferramenta de interface gráfica desenvolvida em Python que permite executar
 exploits do Metasploit (`metaexploit`) de forma rápida e intuitiva, com foco em **testes de penetração éticos**.

A ferramenta automatiza:
- Configuração de `RHOST`, `LHOST` e `LPORT`
- Execução de exploits pré-configurados com 1 clique
- Exibição de logs em tempo real
- Salvamento automático de sessões e resultados

> **Aviso Legal**: Use apenas em ambientes autorizados. O autor não se responsabiliza por uso indevido.

---

## Recursos

| Funcionalidade                  | Status |
|-------------------------------|--------|
| Interface gráfica moderna       | ✅     |
| Exploits rápidos (1 clique)     | ✅     |
| Detecção automática de LHOST    | ✅     |
| Logs em tempo real              | ✅     |
| Salvamento automático de logs   | ✅     |
| Suporte a timeout de execução   | ✅     |
| Execução em thread (não trava)  | ✅     |

---

## Exploits Rápidos Disponíveis

| Nome                     | Módulo Metasploit                          | Payload                     |
|--------------------------|--------------------------------------------|-----------------------------|
| EternalBlue (MS17-010)   | `exploit/windows/smb/ms17_010_eternalblue` | `windows/meterpreter/reverse_tcp` |
| Struts2 RCE              | `exploit/multi/http/struts2_rest_xstream`  | `java/meterpreter/reverse_tcp`    |
| Tomcat Manager Upload    | `exploit/multi/http/tomcat_mgr_upload`     | `java/meterpreter/reverse_tcp`    |
| PHPMyAdmin Config Exec   | `exploit/unix/webapp/phpmyadmin_config_exec` | `php/meterpreter/reverse_tcp` |

---

## Requisitos

- **Sistema Operacional**: Kali Linux (recomendado)
- **Python**: `3.8` ou superior
- **Ferramentas**:
  ```bash
  metasploit-framework
  metaexploit (wrapper do msfconsole)
  ```
- **Permissões**: Execução como usuário com acesso ao Metasploit

---

## Instalação

1. **Clone ou baixe o script**
   ```bash
   wget https://seusite.com/scanfull.py
   chmod +x scanfull.py
   ```

2. **Instale dependências (se necessário)**
   ```bash
   sudo apt update
   sudo apt install metasploit-framework python3-tk
   ```

3. **(Opcional)** Adicione um ícone
   - Coloque `scanfull.ico` no mesmo diretório do script

---

## Uso

```bash
./scanfull.py
```

### Passos na Interface:

1. Preencha o **RHOST** (IP do alvo)
2. O **LHOST** é detectado automaticamente
3. Ajuste a **LPORT** (padrão: `4444`)
4. Clique em um dos **exploits rápidos**
5. Acompanhe os logs em tempo real
6. Logs são salvos em:  
   ```
   /home/kali/forcabruta/metaexploit_logs/
   ```

---

## Estrutura de Pastas

```
/home/kali/forcabruta/
└── metaexploit_logs/
    ├── metaexploit_192.168.1.100_20250405_143022.log
    └── ...
```

---

## Capturas de Tela

*(Adicione imagens aqui no futuro)*

---

## Solução de Problemas

| Problema                          | Solução |
|----------------------------------|--------|
| `metaexploit: command not found` | Instale o Metasploit: `sudo apt install metasploit-framework` |
| LHOST aparece como `127.0.0.1`   | Verifique conexão com a internet |
| Exploit não inicia               | Verifique se o serviço no alvo está ativo |
| Erro de timeout                  | Aumente o tempo ou verifique firewall/rede |

---

## Atualizações Futuras (Roadmap)

- [ ] Adicionar mais exploits
- [ ] Suporte a múltiplos alvos
- [ ] Exportar sessões Meterpreter
- [ ] Tema claro/escuro
- [ ] Integração com Nmap (scan automático)

---

## Licença

**Todos os direitos reservados** © 2025  
Proibida cópia, distribuição ou modificação sem autorização expressa do autor.

---

## Contato

**Leonardo de Moura Fuseti**  
- GitHub: [mourafuseti](https://github.com/mourafuseti) 
- Email: mourafuseti@hotmail.com

> **Pentest com ética. Conhecimento é poder. Use com responsabilidade.**


