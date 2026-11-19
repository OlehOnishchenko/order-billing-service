# Release Notes v1.1.0

Основні зміни у версії v1.1.0:

## Added
* Додано спеціальний тариф доставки `80.0` для міста `"Kyiv"`.
* Додано параметр `taxRate` (за замовчуванням `0.20`) у функцію розрахунку стандартного рахунку[cite: 1].
* Додано дві окремі функції (`processStandardInvoice` та `processTaxExemptInvoice`) замість однієї спільної[cite: 1].

## Changed
* Збільшено вартість доставки за кілограм ваги з `12.0` до `15.0`[cite: 1].
* Переписано код файлу `billing.js` під Data Coupling (прибрано зайві залежності між функціями)[cite: 1].

## Breaking Changes
* Змінено параметри функцій: у `calculateDeliveryCost` тепер передається рядок `city` замість усього об'єкта `customerProfile`[cite: 1].
* Видалено глобальну змінну `GLOBAL_TAX_RATE`[cite: 1].
* Видалено стару функцію `processInvoice` та прапорець `modeFlag`[cite: 1].
