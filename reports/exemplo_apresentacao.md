---
marp: true
title: Modelo para detecção de deficiência de recombinação homologa (HRD)
footer: 'Sprint DASA - 4o semestre'
---

<style>
	footer {
		position: fixed;
		bottom: 10px;
		left: 1050px;
		width: 400px;
	}

	footer img {
		vertical-align: middle;
	}
</style>


Modelo para detecção de deficiência de recombinação homologa (HRD)
===

![width:300px](img/capa.png)

###### Equipe....

---

Qual é o problema? 
===

- o problema é.... 

---

Datasets
===

A distribuição dos valores do dataset ....

```
Positivo                                               3295
Negativo                                               1135
Name: count, dtype: int64
```

---

Exemplo de trecho de código
===

- talvez seja relevante...

```python
merged_df['TeveAcesso'] = np.where(
    merged_df['Decisao'] == 'Acesso Concedido', 'Acesso Concedido',
    np.where(
        merged_df['Decisao'] == 'Acesso Parcialmente Concedido', 'Acesso Parcialmente Concedido', 'Acesso Negado'
        )
)
```

---

Exemplo de apresentação dos resultados
===


```python
F1 Score: 0.6859388509722292 Accuracy: 0.8428165007112376
```

```python
              precision    recall  f1-score   support

           0       0.89      0.76      0.82       507
           1       1.00      0.22      0.36        83
           2       0.82      0.96      0.88       816

    accuracy                           0.84      1406
   macro avg       0.90      0.64      0.69      1406
weighted avg       0.86      0.84      0.83      1406
```

---

Considerações finais e próximas atividades
===

* os resultados obtidos com o algoritmo xxxxx 
* ....

