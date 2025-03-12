# Ansible Role: Vector

Эта роль устанавливает и настраивает [Vector](https://vector.dev/) для сбора логов.

## Переменные

| Переменная             | Значение по умолчанию | Описание                           |
|------------------------|----------------------|------------------------------------|
| `vector_version`       | `""`           | Версия Vector                     |
| `vector_config_path`   | `"/etc/vector/vector.yaml"` | Путь до конфигурации  |
| `vector_config_dir`    | `"/etc/vector"`      | Директория конфигурации           |

## Использование

Пример playbook:

```yaml
- name: Install Vector
  hosts: vector_group
  roles:
    - vector-role
