---
title: genericError リソースの種類
description: 汎用のエラーです。
localization_priority: Normal
ms.openlocfilehash: 744266ef8ffb17c4af4168d6239e5a5a30561936
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823570"
---
# <a name="genericerror-resource-type"></a>genericError リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

汎用のエラーです。

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:---------|:-----|:------------|
| message | String | エラー メッセージ。 |
| code | String | エラー コード。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
