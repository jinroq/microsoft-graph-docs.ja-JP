---
title: governanceRuleSetting リソースの種類
description: ロールの設定で構成されたルールを表します。
ms.openlocfilehash: 486b5163c59772c971cfc1d61a98817b7f0c16f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070678"
---
# <a name="governancerulesetting-resource-type"></a>governanceRuleSetting リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ロールの設定で構成されたルールを表します。


## <a name="properties"></a>プロパティ
|プロパティ      | 型         |説明|
|:-------------|:-------------|:----------|
|ruleIdentifier|String        |ルールの id です。 たとえば、``ExpirationRule``と``MfaRule``。|
|setting       |String        |ルールの設定をします。 値は、Parameter_Name:Parameter_Value の形式でのペアの一覧を JSON 文字列です。 たとえば、`{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}` では、|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRuleSetting"
}-->


```json
{
  "ruleIdentifier": "String",
  "setting": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRuleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->