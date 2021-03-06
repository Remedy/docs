## finance.set1cCashShiftTransactionId: Изменение id транзакций в системе 1С

> Пример запроса:

```php
<?php
$url = 'https://joinposter.com/api/finance.set1cCashShiftTransactionId'
 . '?token=687409:4164553abf6a031302898da7800b59fb';

$finance = [
    'id' => [
        [
            'shift_tr_id_id' => 32,
            'id_1c'   => 'b80ffc81-0fc9-11e7-9ab4-ace01035e460',
        ],
    ],
];

$data = sendRequest($url, 'post', $finance);
```

> Пример ответа:

```json
{  
  "success":1
}
```

Метод изменяет id транзакций в системе 1С

### HTTP запрос

`GET https://joinposter.com/api/finance.set1cCashShiftTransactionId`

### POST-параметры запроса finance.set1cCashShiftTransactionId

Параметр | Описание
-------- | --------
id | Массив объектов

В свою очередь, каждый объект должен содержать следующие свойства:

Параметр | Описание
-------- | --------
shift_tr_id_id | Id транзакций
id_1c | Id транзакций в системе 1С

### Параметры ответа finance.set1cCashShiftTransactionId

Параметр | Описание
-------- | --------
success | 1, если id транзакций в системе 1С успешно изменены
