---
title: convertIdResult リソースの種類
description: TranslateExchangeIds 関数によって実行される ID 形式変換の結果です。
ms.openlocfilehash: 3a17399ffe44c43c78f7b50933b2e847a3e64f32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067806"
---
# <a name="convertidresult-resource-type"></a>convertIdResult リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

[TranslateExchangeIds](../api/user-translateexchangeids.md)関数によって実行される ID 形式変換の結果です。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
| sourceId | String | 変換された識別子です。 この値は、元、変換されていない識別子です。 |
| targetId | String | 変換後の識別子です。 この値は、変換が失敗した場合ではありません。 |
| errorDetails | [genericError](genericerror.md) | 変換エラーの原因を示すエラー オブジェクトです。 この値は、変換が成功した場合ではありません。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```