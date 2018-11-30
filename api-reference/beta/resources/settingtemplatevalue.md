---
title: settingTemplateValue リソースの種類
description: 設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。
ms.openlocfilehash: afc872f3e3d8d02acae639b967cdaf9375bb60cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069805"
---
# <a name="settingtemplatevalue-resource-type"></a>settingTemplateValue リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|defaultValue|文字列|設定の既定値です。 読み取り専用です。|
|説明|文字列|設定の説明です。 読み取り専用。|
|name|文字列|設定の名前。 読み取り専用。|
|type|文字列|設定の種類です。 読み取り専用。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
