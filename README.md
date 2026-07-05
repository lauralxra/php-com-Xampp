# php-com-Xampp
Este repositório reúne os principais comandos para instalar, iniciar, parar e gerenciar o XAMPP no Pop!_OS. Também apresenta exemplos para controlar os serviços Apache e MySQL, abrir o painel gráfico e acessar os projetos hospedados no diretório htdocs, servindo como um guia rápido para desenvolvimento local com PHP.

# XAMPP no Pop!_OS / Linux

## Iniciar todos os serviços

```bash
sudo /opt/lampp/lampp start
```

---

## Parar todos os serviços

```bash
sudo /opt/lampp/lampp stop
```

---

## Reiniciar todos os serviços

```bash
sudo /opt/lampp/lampp restart
```

---

## Verificar o status dos serviços

```bash
sudo /opt/lampp/lampp status
```

Exemplo de saída:

```text
Apache is running.
MySQL is running.
ProFTPD is running.
```

---

# Controlar serviços individualmente

## Apache

### Iniciar

```bash
sudo /opt/lampp/lampp startapache
```

### Parar

```bash
sudo /opt/lampp/lampp stopapache
```

### Reiniciar

```bash
sudo /opt/lampp/lampp restartapache
```

---

## MySQL (MariaDB)

### Iniciar

```bash
sudo /opt/lampp/lampp startmysql
```

### Parar

```bash
sudo /opt/lampp/lampp stopmysql
```

### Reiniciar

```bash
sudo /opt/lampp/lampp restartmysql
```

---

## FTP (ProFTPD)

### Iniciar

```bash
sudo /opt/lampp/lampp startftp
```

### Parar

```bash
sudo /opt/lampp/lampp stopftp
```

### Reiniciar

```bash
sudo /opt/lampp/lampp restartftp
```

---

# Abrir o painel gráfico do XAMPP

```bash
sudo /opt/lampp/manager-linux-x64.run
```

---

# Local dos projetos

Os arquivos PHP devem ficar em:

```text
/opt/lampp/htdocs
```

Exemplo:

```bash
cd /opt/lampp/htdocs
sudo mkdir meu_projeto
```

Acesse no navegador:

```
http://localhost/meu_projeto
```

---

# Testar se o Apache está funcionando

Abra no navegador:

```
http://localhost
```

Se aparecer a página do XAMPP, o Apache está funcionando corretamente.

---

# Comandos úteis

| Ação | Comando |
|------|----------|
| Iniciar tudo | `sudo /opt/lampp/lampp start` |
| Parar tudo | `sudo /opt/lampp/lampp stop` |
| Reiniciar tudo | `sudo /opt/lampp/lampp restart` |
| Status | `sudo /opt/lampp/lampp status` |
| Iniciar Apache | `sudo /opt/lampp/lampp startapache` |
| Parar Apache | `sudo /opt/lampp/lampp stopapache` |
| Reiniciar Apache | `sudo /opt/lampp/lampp restartapache` |
| Iniciar MySQL | `sudo /opt/lampp/lampp startmysql` |
| Parar MySQL | `sudo /opt/lampp/lampp stopmysql` |
| Reiniciar MySQL | `sudo /opt/lampp/lampp restartmysql` |
| Abrir interface gráfica | `sudo /opt/lampp/manager-linux-x64.run` |
