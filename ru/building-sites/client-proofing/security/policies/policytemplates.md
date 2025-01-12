---
title: "Шаблоны политик"
translation: building-sites/client-proofing/security/policies/policytemplates
---

## Что такое шаблоны политики?

Шаблоны политик определяют, какие разрешения _доступны_ для [Политики доступа](building-sites/client-proofing/security/policies "Политики"). Шаблон политики не определяет, дано ли разрешение (это делает Политика доступа), он просто определяет, какие разрешения должны проверяться. Наличие шаблона политики полезно, если необходимо сузить список доступных разрешений, которые вы хотите определить в политике доступа.

Хотя есть определенные совпадения между конкретными разрешениями, определенными в каждом шаблоне политики, каждый шаблон содержит _только_ уникальные разрешения. Каждый шаблон определяет разрешения, которые применяются к спискам контроля доступа (ACL) и для которых они предназначены. Каждый должен быть автономным.

### AdministratorTemplate

Определяет все разрешения для работы в панели управления MODX, т.е. какие действия могут быть предприняты из контекста. Обычно политики, основанные на этом шаблоне, не используются в других контекстах, кроме панели управления, если только пользователям не нужно запускать их процессоры (например, расширение интерфейса). [См. Все разрешения для политик администратора](building-sites/client-proofing/security/policies/permissions/administrator-policy "Разрешения - Политика администратора")

### ElementTemplate

Элемент определяет дополнительные разрешения, связанные с ACL Элемента.

### MediaSourceTemplate

Разрешения, связанные с доступом к источникам файлов.

### ObjectTemplate

Общие разрешения `xPDOObject` использующиеся для любого `modAccessibleObject`.

### ResourceTemplate

Определяет дополнительные разрешения, связанные с ACL группы ресурсов. [Все разрешения политики ресурсов](building-sites/client-proofing/security/policies/permissions/resource-policy "Разрешения - Ресурсная политика")

### ContextTemplate

Контекст определяет контекстный доступ, в тех случаях, когда действия администратора не задействованы.

## Смотрите также

1. [Политики - Шаблоны политик](building-sites/client-proofing/security/policies/policytemplates)
2. [Политики - Контроль доступа](building-sites/client-proofing/security/policies/acls)
