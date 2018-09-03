---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
ms.openlocfilehash: 2fd6c08e1cfc28a77019d174763b9d698519b6a2
ms.sourcegitcommit: 9e4dc7745eb1bbbe595afd8c7f3db4c19c6bb4ac
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2018
ms.locfileid: "23271316"
---
# <a name="columndefinition-resource"></a>ColumnDefinition リソース

## <a name="json-representation"></a>JSON 表記

以下は、ColumnDefinition リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

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

| プロパティ名           | 型    | 説明
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | 文字列  | サイト列の場合、この列が属するグループの名前。 関連する列を整理するのに役立ちます。
| **説明**         | 文字列  | 列に関するユーザー向けの説明。
| **displayName**         | 文字列  | 列を示すユーザー向けの名前。
| **enforceUniqueValues** | ブール値 | True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。
| **隠し**              | ブール値 | この列がユーザー インターフェイスに表示されるかどうかを指定します。
| **ID**                  | 文字列  | 列の一意識別子。
| **インデックス済**             | ブール値 | 列の値を、並べ替えと検索に使用できるかどうかを指定します。
| **名前**                | 文字列  | [listItem][] の [fields][] に表示される、列を示す API 向けの名前。 ユーザー向けの名前については **displayName** をご覧ください。
| **readOnly**            | ブール値    | 列の値を変更できるかどうかを指定します。
| **必須です**            | ブール値 | 列の値が省略不可であるかどうかを指定します。

列には、さまざまな種類のデータを保持できます。
次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。
これらのプロパティは相互に排他的で、各列でいずれか 1 つだけを指定できます。

| プロパティ名     | 型                    | 説明
|:------------------|:------------------------|:-------------------------------
| **ブール値**       | [booleanColumn][]       | この列にはブール値が格納されます。
| **計算済み**    | [calculatedColumn][]    | この列のデータは、他の列に基づいて計算されます。
| **選択**        | [choiceColumn][]        | この列には、選択肢リストからのデータが格納されます。
| **通貨**      | [currencyColumn][]      | この列には通貨値が格納されます。
| **dateTime**      | [dateTimeColumn][]      | この列には日時の値が格納されます。
| **defaultValue**  | [defaultColumnValue][]  | この列の既定値です。
| **参照**        | [lookupColumn][]        | この列のデータは、サイト内の別のソースから検索されます。
| **数**        | [numberColumn][]        | この列には数値が格納されます。
| **personOrGroup** | [personOrGroupColumn][] | この列にはユーザーまたはグループの値が格納されます。
| **テキスト**          | [textColumn][]          | この列にはテキスト値が格納されます。

注: これらのプロパティは SharePoint の [SPFieldType][] 列挙体に対応しています。
ほとんどの一般的なフィールドの種類を上記に示しましたが、この API には含まれないものもあります。
そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。

## <a name="remarks"></a>備考

列の ColumnDefinitions とフィールドの値は、既定では表示されません。`hidden`
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
