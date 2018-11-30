---
title: agreementFile リソースの種類
description: Azure Active Directory (AD の Azure) とテナントを管理する使用許諾契約書ファイルのカスタマイズ可能な条件を表します。 契約書のファイルについてのメタデータが含まれています (たとえば、名前、言語、既定のファイルであるかどうかと)。
ms.openlocfilehash: f099715fd25fbae9d7b2a94d6de841b8766c30e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070279"
---
# <a name="agreementfile-resource-type"></a>agreementFile リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
|fileData|[agreementFileData](agreementfiledata.md)|PDF 文書の使用の条件を表すデータです。 読み取り専用。|
|fileName|String|契約ファイル (TOU.pdf など) の名前です。 読み取り専用。|
|id|String|読み取り専用。|
|isDefault|ブール値|クライアント基本設定と一致する、カルチャの場合、既定の契約書ファイルはかどうかを示します。 ファイルの [なし] は既定値としてマークすると、1 つ目は既定値として扱われます。 読み取り専用。|
|language|String|形式 languagecode2 の国と regioncode2 の契約書ファイルのカルチャです。 languagecode2 は、小文字の ISO 639-1 から派生した 2 文字コードです。 国/regioncode2 では、ISO 3166 から派生し、通常は、2 つの大文字、または BCP 47 言語タグ (たとえば、EN-US)。 読み取り専用。|

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementFile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
