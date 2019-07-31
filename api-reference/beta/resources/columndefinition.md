---
author: JeremyKelley
description: 以下は、columnDefinition リソースの JSON 表記です。
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 7f60d33f8fbfe76c9dfd0ca02c98df96ca6ab380
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973301"
---
# <a name="columndefinition-resource-type"></a>columnDefinition リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a>JSON 表記

以下は、columnDefinition リソースの JSON 表記です。

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
型に関連するプロパティ (boolean、演算、choice、currency、dateTime、lookup、number、個人、グループ、テキスト) は相互に排他的です。1つの列に指定できるのは1つだけです。

| プロパティ名           | 種類    | 説明
|:------------------------|:--------|:-----------------------------------------
| **columnGroup**         | string  | サイト列の場合、この列が属するグループの名前。 関連する列を整理するのに役立ちます。
| **説明**         | string  | 列に関するユーザー向けの説明。
| **displayName**         | string  | 列を示すユーザー向けの名前。
| **enforceUniqueValues** | ブール値 | True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。
| **hidden**              | ブール値 | この列がユーザー インターフェイスに表示されるかどうかを指定します。
| **id**                  | string  | 列の一意識別子。
| **indexed**             | ブール値 | 列の値を、並べ替えと検索に使用できるかどうかを指定します。
| **name**                | string  | [listItem][] の [fields][] に表示される、列を示す API 向けの名前。 ユーザー向けの名前については **displayName** をご覧ください。
| **readOnly**            | bool    | 列の値を変更できるかどうかを指定します。
| **required**            | boolean | 列の値が省略不可であるかどうかを指定します。
| **boolean**       | [booleanColumn][]       | この列にはブール値が格納されます。
| **calculated**    | [calculatedColumn][]    | この列のデータは、他の列に基づいて計算されます。
| **choice**        | [choiceColumn][]        | この列には、選択肢リストからのデータが格納されます。
| **currency**      | [currencyColumn][]      | この列には通貨値が格納されます。
| **dateTime**      | [dateTimeColumn][]      | この列には日時の値が格納されます。
| **defaultValue**  | [defaultColumnValue][]  | この列の既定値です。
| **地理位置情報**   | [geolocationColumn][]   | この列には、地理位置情報が格納されます。
| **lookup**        | [lookupColumn][]        | この列のデータは、サイト内の別のソースから検索されます。
| **number**        | [numberColumn][]        | この列には数値が格納されます。
| **personOrGroup** | [personOrGroupColumn][] | この列にはユーザーまたはグループの値が格納されます。
| **text**          | [textColumn][]          | この列にはテキスト値が格納されます。

>**注:** これらのプロパティは、SharePoint の[SPFieldType][]列挙に対応しています。
最も一般的なフィールドの種類は上記の表で表されていますが、このベータ版 API にはまだ不足しています。
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

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": []
}
-->
