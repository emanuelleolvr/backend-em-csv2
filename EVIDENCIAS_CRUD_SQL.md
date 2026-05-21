# Evidências - INSERT, UPDATE e DELETE no banco db_em

## Identificação

Nome: Emanuele Oliveira Pinezzi
Turma: 3A  
Data: 21/05/2026

---

# 1. SELECT final - Leituras do dia 2026-04-04

```sql
SELECT *
FROM leituras
WHERE timestamp >= '2026-04-04'
AND timestamp < '2026-04-05'
ORDER BY timestamp ASC;
```

```text
COLE AQUI O RESULTADO
```

---

# 2. SELECT final - Conferência do UPDATE

```sql
SELECT *
FROM leituras
WHERE station_id = 'EM-ARACATUBA-01'
AND timestamp = '2026-04-04 09:00:00';
```

```text
COLE AQUI O RESULTADO
```

---

# 3. SELECT final - Conferência do DELETE

```sql
SELECT *
FROM leituras
WHERE station_id = 'EM-ARACATUBA-01'
AND timestamp = '2026-04-04 11:00:00';
```

```text
Sem registros encontrados.
```

---

# 4. SELECT final - Todas as leituras ordenadas

```sql
SELECT *
FROM leituras
ORDER BY id ASC;
```

```text
COLE AQUI O RESULTADO
```

---

# 5. Teste pela API

```text
http://localhost:3000/api/leituras/data/2026-04-04
```

```json
COLE AQUI O JSON DA API
```

---

# 6. Conclusão

Resposta:

```text
INSERT adiciona novos registros na tabela.
UPDATE altera registros existentes.
DELETE remove registros da tabela.
O WHERE é importante para alterar ou excluir apenas os dados desejados.
```