---
title: agreementFile リソースの種類
description: テナントが azure Active Directory (azure AD) を使用して管理する、カスタマイズ可能な使用許諾契約書ファイルを表します。 このファイルには、アグリーメントファイルのメタデータが含まれます (たとえば、名前、言語、および既定のファイルであるかどうか)。
localization_priority: Normal
ms.openlocfilehash: b914feecfc91d71c525711f725bf4a533d44a6b1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328619"
---
# <a name="agreementfile-resource-type"></a>agreementFile リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントが azure Active Directory (azure AD) を使用して管理する、カスタマイズ可能な使用許諾契約書ファイルを表します。 このファイルには、アグリーメントファイルのメタデータが含まれます (たとえば、名前、言語、および既定のファイルであるかどうか)。

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementFile](../api/agreementfile-get.md) | [agreementFile](agreementfile.md) | Read properties and relationships of an **agreementFile** object. |
| [Update](../api/agreementfile-update.md) | [agreementFile](agreementfile.md) | Update an **agreementFile** object. |
| [Delete](../api/agreementfile-delete.md) | None | Delete an **agreementFile** object. |
-->

## <a name="properties"></a>プロパティ
| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|fileData|[agreementFileData](agreementfiledata.md)|使用条件を表すデータ。 PDF ドキュメント。 読み取り専用です。|
|fileName|文字列型 (String)|アグリーメントファイルの名前 (たとえば、「お持ちの形式」)。 読み取り専用です。|
|id|String|読み取り専用です。|
|isDefault|ブール型 (Boolean)|クライアントの優先度に一致するカルチャがない場合に、これが既定のアグリーメントファイルであるかどうかを示します。 ファイルが既定として設定されていない場合は、最初のファイルが既定として扱われます。 読み取り専用です。|
|language|String|languagecode2-country/regioncode2 という形式の、アグリーメントファイルのカルチャ。 languagecode2 は、ISO 639-1 から派生した、小文字の2文字のコードです。 country/regioncode2 は ISO 3166 から派生し、通常は2つの大文字または BCP-47 language タグ (例: en-us) で構成されます。 読み取り専用です。|

## <a name="relationships"></a>関係
なし。


## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFile"
}-->

```json
{
  "fileData": {"@odata.type": "microsoft.graph.agreementFileData"},
  "fileName": "String",
  "id": "String (identifier)",
  "isDefault": true,
  "language": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
