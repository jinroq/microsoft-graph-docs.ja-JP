---
title: agreementFile リソースの種類
description: Azure Active Directory (AD の Azure) とテナントを管理する使用許諾契約書ファイルのカスタマイズ可能な条件を表します。 契約書のファイルについてのメタデータが含まれています (たとえば、名前、言語、既定のファイルであるかどうかと)。
localization_priority: Normal
ms.openlocfilehash: 446173e83d32af96f938cbee15964ea204a62f7e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511430"
---
# <a name="agreementfile-resource-type"></a>agreementFile リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (AD の Azure) とテナントを管理する使用許諾契約書ファイルのカスタマイズ可能な条件を表します。 契約書のファイルについてのメタデータが含まれています (たとえば、名前、言語、既定のファイルであるかどうかと)。

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
|fileData|[agreementFileData](agreementfiledata.md)|PDF 文書の使用の条件を表すデータです。 読み取り専用です。|
|fileName|String|契約ファイル (TOU.pdf など) の名前です。 読み取り専用です。|
|id|文字列|読み取り専用です。|
|isDefault|ブール値|クライアント基本設定と一致する、カルチャの場合、既定の契約書ファイルはかどうかを示します。 ファイルの [なし] は既定値としてマークすると、1 つ目は既定値として扱われます。 読み取り専用です。|
|language|String|形式 languagecode2 の国と regioncode2 の契約書ファイルのカルチャです。 languagecode2 は、小文字の ISO 639-1 から派生した 2 文字コードです。 国/regioncode2 では、ISO 3166 から派生し、通常は、2 つの大文字、または BCP 47 言語タグ (たとえば、EN-US)。 読み取り専用です。|

## <a name="relationships"></a>リレーションシップ
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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreementfile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
