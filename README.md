# Universal BIOS Recovery Image for Alder Lake-N (ICL)

Этот репозиторий содержит "Золотой Дамп" (Gold Dump) BIOS для ноутбуков на базе процессора Intel N100 (Alder Lake-N). 

## Характеристики образа:
*   **Регион ME:** Обновлен до версии **16.50.0.1175** (состояние: Clean/RGN).
*   **Descriptor:** Полностью разблокирован (Unlocked). Допускает прошивку через `flashrom` без программатора (если запущен с правами суперпользователя).
*   **DMI Данные:** Очищены. Серийный номер заменен на заглушку `SERIAL-NUMBR`.
*   **Анонимность:** Удалены UUID и ключи активации Windows (MSDM).

## Кому это нужно?
1. Тем, у кого "окирпичился" ноутбук после неудачного обновления.
2. Тем, у кого наблюдаются странные задержки или выключения через 30 минут (проблемы с ME-регионом).
3. Тем, кто хочет иметь чистую базу для моддинга BIOS.

## Как использовать:
1. Прошейте `bin/Gold_Final.bin` с помощью программатора (CH341A и др.) или через `flashrom`.
2. После первой загрузки используйте утилиты AMI (AMIDEEFI/AMIDEWIN), чтобы восстановить свой родной серийный номер:
   `AMIDEWINx64.exe /SS "ВАШ_СЕРИЙНИК"`


`Model: ICL Alder Lake-N (N100) Laptop
Version: ME 16.50.0.1175 (Clean/RGN)
Status: Descriptor Unlocked (flashrom ready)
DMI: Removed (Serial Number: SERIAL-NUMBR)
Verification: Structurally identical to factory dump, tested via UEFITool.`