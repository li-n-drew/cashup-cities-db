# Данные для города: Москва (msk)

## Необходимые файлы:

1. `company_networks.json` - данные о сетях магазинов
2. `company_locations.json` - данные о точках магазинов

## Формат данных:

### company_networks.json
```json
[
  {
    "network_id": "magnit",
    "network_name": "Магнит",
    "main_category": "Супермаркеты",
    "total_locations": 150
  }
]
```

### company_locations.json
```json
[
  {
    "location_id": "magnit_001",
    "network_id": "magnit",
    "name": "Магнит на Невском",
    "latitude": 59.939095,
    "longitude": 30.315868,
    "category": "Супермаркеты",
    "address": "Невский пр., 100",
    "phone": "+7 999 123-45-67",
    "rating": 4.5,
    "working_hours": "09:00-23:00"
  }
]
```

## Примечания:
- Все локации должны иметь координаты (latitude, longitude)
- Координаты должны быть в пределах города
- Для генерации тестовых данных можно использовать скрипт `generate-test-data.js`
