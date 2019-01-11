---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: 5db835b9720f9fa711d683dd505e8325b27d79d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844493"
---
# <a name="columndefinition-resource-type"></a>columnDefinition リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

## <a name="json-representation"></a>JSON 表記

ColumnDefinition リソースの JSON 表現は、ここで。

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
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a>プロパティ

列には、さまざまな種類のデータを保持できます。
次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。
タイプに関連するプロパティ (ブール値、計算された、選択、通貨、日時、検索、番号、personOrGroup、テキスト) は相互に排他的な--列のみが指定されているそれらの 1 つです。

| プロパティ名           | Type    | 説明
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | 文字列  | サイト列の場合、この列が属するグループの名前。 関連する列を整理するのに役立ちます。
| **description**         | 文字列  | 列に関するユーザー向けの説明。
| **displayName**         | 文字列  | 列を示すユーザー向けの名前。
| **enforceUniqueValues** | boolean | True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。
| **hidden**              | boolean | この列がユーザー インターフェイスに表示されるかどうかを指定します。
| **id**                  | string  | 列の一意識別子。
| **indexed**             | boolean | 列の値を、並べ替えと検索に使用できるかどうかを指定します。
| **name**                | 文字列  | [listItem][] の [fields][] に表示される、列を示す API 向けの名前。 ユーザー向けの名前については **displayName** をご覧ください。
| **readOnly**            | bool    | 列の値を変更できるかどうかを指定します。
| **required**            | boolean | 列の値が省略不可であるかどうかを指定します。
| **boolean**       | [booleanColumn][]       | この列にはブール値が格納されます。
| **calculated**    | [calculatedColumn][]    | この列のデータは、他の列に基づいて計算されます。
| **choice**        | [choiceColumn][]        | この列には、選択肢リストからのデータが格納されます。
| **currency**      | [currencyColumn][]      | この列には通貨値が格納されます。
| **dateTime**      | [dateTimeColumn][]      | この列には日時の値が格納されます。
| **defaultValue**  | [defaultColumnValue][]  | この列の既定値です。
| **地理位置情報**   | [geolocationColumn][]   | この列は、地理位置情報を格納します。
| **lookup**        | [lookupColumn][]        | この列のデータは、サイト内の別のソースから検索されます。
| **number**        | [numberColumn][]        | この列には数値が格納されます。
| **personOrGroup** | [personOrGroupColumn][] | この列にはユーザーまたはグループの値が格納されます。
| **text**          | [textColumn][]          | この列にはテキスト値が格納されます。

>**注:** これらのプロパティは、SharePoint の[SPFieldType][]の列挙体に対応しています。
最も一般的なフィールドの種類は上記の表に表示されるときにこのベータ版の API がまだないです。
そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。

## <a name="remarks"></a>備考

`hidden` 列の ColumnDefinitions とフィールドの値は、既定では表示されません。
**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。
[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
