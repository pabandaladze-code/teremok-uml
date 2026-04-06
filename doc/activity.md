
---

### 📄 `doc/activity.md`
```markdown
# Activity Diagram

```plantuml
@startuml
skinparam conditionStyle inside
title Алгоритм заселения

start

:Зверь запрашивает вход;

if (Это Медведь?) then (да)
  #pink:Теремок разрушен
  stop
else (нет)
  :Проверить лимит веса;
  if (Вес превышен?) then (да)
    :Отказать
  else (нет)
    :Заселить
  endif
endif

stop
@enduml
