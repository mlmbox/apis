# V2

```text
Основные изменения связаны с добавлением маркетинговой валюты MSG.
В связи с чем в API вызовов добавлены ответы по 2 валютам (MTS и MSG).
```

### Обновлены функции установки курса для маркетинговой валюты  "MTS-USDT" -> "MSG-USDT":
https://github.com/mlmbox/apis/blob/main/mlmbox/admin/asset/v1/asset_pair.proto#L12-L14

### Обновлена модель "mlmbox.type.Account":
https://github.com/mlmbox/apis/blob/main/mlmbox/type/account.proto

- В старой версии отображаются 2 поля по валюте MTS 
  - repeated mlmbox.type.Bonus bonuses = 15;
  - mlmbox.type.Farming.State farming_state = 16;

- В новой версии отображается массив по всем используюмых валют:
  - repeated Assets assets = 24;

### Обновлена модель "mlmbox.type.Binary":
https://github.com/mlmbox/apis/blob/main/mlmbox/type/binary.proto#L38

- В старой версии отображаются статистика в MTS валюте в поле "self_bonuses"
- В новой версии отображается массив по всем используюмых валютам "assets":

### Апгрейд "Account.Info" -> "Account.InfoV2":
https://github.com/mlmbox/apis/blob/main/mlmbox/client/account/v1/account.proto#L19

### Апгрейд "Account.BonusesInfo" -> "Account.BonusesInfoV2":
https://github.com/mlmbox/apis/blob/main/mlmbox/client/account/v1/account.proto#L31

### Апгрейд "Binary.Info" -> "Binary.InfoV2":
https://github.com/mlmbox/apis/blob/main/mlmbox/client/binary/v1/binary.proto#L11

### Апгрейд "Farming.Info" -> "Farming.InfoV2":
https://github.com/mlmbox/apis/blob/main/mlmbox/client/farming/v1/farming.proto#L12