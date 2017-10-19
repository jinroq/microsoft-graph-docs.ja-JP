---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: e5942ddee4b505243cb64121862ce9e89e52d245
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="columndefinition-resource"></a>ColumnDefinition リソース

## <a name="json-representation"></a>JSON 表記

以下は、ColumnDefinition リソースの JSON 表記です。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.columnDefinition",
       "keyProperty": "id", "optionalProperties": [ ] } -->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": "true",
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a>プロパティ

**columnDefinition** リソースには以下のプロパティがあります。

| プロパティ名           | 種類    | 説明
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | string  | サイト列の場合、この列が属するグループの名前。 関連する列を整理するのに役立ちます。
| **description**         | string  | 列に関するユーザー向けの説明。
| **displayName**         | string  | 列を示すユーザー向けの名前。
| **enforceUniqueValues** | boolean | True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。
| **hidden**              | boolean | この列がユーザー インターフェイスに表示されるかどうかを指定します。
| **id**                  | string  | 列の一意識別子。
| **indexed**             | boolean | 列の値を、並べ替えと検索に使用できるかどうかを指定します。
| **name**                | string  | [listItem][] の [fields][] に表示される、列を示す API 向けの名前。 ユーザー向けの名前については **displayName** をご覧ください。
| **readOnly**            | bool    | 列の値を変更できるかどうかを指定します。
| **required**            | boolean | 列の値が省略不可であるかどうかを指定します。

列には、さまざまな種類のデータを保持できます。
次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。
これらのプロパティは相互に排他的で、各列でいずれか 1 つだけを指定できます。

| プロパティ名     | 種類                    | 説明
|:------------------|:------------------------|:-------------------------------
| **boolean**       | [booleanColumn][]       | この列にはブール値が格納されます。
| **calculated**    | [calculatedColumn][]    | この列のデータは、他の列に基づいて計算されます。
| **choice**        | [choiceColumn][]        | この列には、選択肢リストからのデータが格納されます。
| **currency**      | [currencyColumn][]      | この列には通貨値が格納されます。
| **dateTime**      | [dateTimeColumn][]      | この列には日時の値が格納されます。
| **defaultValue**  | [defaultColumnValue][]  | この列の既定値です。
| **lookup**        | [lookupColumn][]        | この列のデータは、サイト内の別のソースから検索されます。
| **number**        | [numberColumn][]        | この列には数値が格納されます。
| **personOrGroup** | [personOrGroupColumn][] | この列にはユーザーまたはグループの値が格納されます。
| **text**          | [textColumn][]          | この列にはテキスト値が格納されます。

注: これらのプロパティは SharePoint の [SPFieldType][] 列挙体に対応しています。
上記ではほとんどの一般的な種類のフィールドを示しましたが、このベータ版 API に含まれないものもあります。
そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。

## <a name="remarks"></a>備考

`hidden` 列の ColumnDefinitions とフィールドの値は、既定では表示されません。
**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。
[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。

[booleanColumn]: booleanColumn.md
[calculatedColumn]: calculatedColumn.md
[choiceColumn]: choiceColumn.md
[currencyColumn]: currencyColumn.md
[dateTimeColumn]: dateTimeColumn.md
[defaultColumnValue]: defaultColumnValue.md
[lookupColumn]: lookupColumn.md
[numberColumn]: numberColumn.md
[personOrGroupColumn]: personOrGroupColumn.md
[textColumn]: textColumn.md
[fieldValueSet]: fieldValueSet.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/en-us/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
