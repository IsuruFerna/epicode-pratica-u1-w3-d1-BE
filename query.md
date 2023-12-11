```
SELECT * FROM clienti WHERE nome = 'Mario';

SELECT nome, cognome FROM clienti WHERE anno_di_nascita = 1982;

SELECT numero_fattura FROM fatture WHERE iva = 20;

SELECT * FROM prodotti
WHERE EXTRACT(YEAR FROM data_attivazione) = 2017
AND in_produzione = true OR in_comercio = true;

SELECT * FROM fatture
JOIN clienti ON fatture.id_cliente = clienti.numero_cliente
WHERE importo < 1000;

SELECT numero_fattura, importo, iva, data_fatturata, denominazione from fatture
JOIN fornitori USING(numero_fornitore);

```
