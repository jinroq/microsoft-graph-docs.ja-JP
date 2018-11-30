---
title: privacyProfile リソースの種類
description: 会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。
ms.openlocfilehash: fb9d5f929f1c9ae28687b80e987dc0909387f5d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074100"
---
# <a name="privacyprofile-resource-type"></a>privacyProfile リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

会社のプライバシー プロファイルを表します。このプライバシー プロファイルには、プライバシー ステートメントの URL と、プライバシー ステートメントに関する連絡先担当者が含まれます。

## <a name="properties"></a>プロパティ
| プロパティ   | 型|説明|
|:---------------|:--------|:----------|
|contactEmail|String| プライバシー ステートメントの連絡先担当者の有効な SMTP メール アドレス。 省略可。|
|statementUrl|String| http:// または https:// で始まる有効な URL 形式。 最大の長さは 255 文字です。 会社のプライバシー ステートメントに誘導する URL。 省略可。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privacyProfile"
}-->

```json
{
  "contactEmail": "string",
  "statementUrl": "string"
}
```