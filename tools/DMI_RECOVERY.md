### [Внимание: После прошивки Gold-образа ваш ID будет SERIAL-NUMBR. Чтобы вернуть родные данные:]

# Для Windows (AMIDEWIN):
1. *   **Скачайте пакет AMI DMI Edit.**
2. *   **Запустите командную строку от имени Администратора.**

# Выполните:
1. *   **AMIDEWINx64.exe /SS "ВАШ_СЕРИЙНИК" (System Serial)**
2. *   **AMIDEWINx64.exe /SU AUTO (Генерация нового UUID)**
3. *   **AMIDEWINx64.exe /BS "СЕРИЙНИК_МАТЕРИНКИ" (Baseboard Serial)**

# Для EFI Shell (AMIDEEFI) — Рекомендуется:
1. *   **Закиньте AMIDEEFIx64.efi на флешку с файловой системой FAT32.**
2. *   **Загрузитесь в Built-in EFI Shell.**

# Введите:
*   `amideefi64.efi` /**SS "ВАШ_СЕРИЙНИК"**