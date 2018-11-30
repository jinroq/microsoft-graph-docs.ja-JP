---
title: customSubjectAlternativeName リソースの種類
description: カスタムのサブジェクトの別名定義
ms.openlocfilehash: 14d6c24cd5e8c087b81fa51194301da522d169b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070303"
---
# <a name="customsubjectalternativename-resource-type"></a>customSubjectAlternativeName リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

カスタムのサブジェクトの別名定義
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|sanType|[subjectAlternativeNameType](../resources/intune-deviceconfig-subjectalternativenametype.md)|SAN のカスタム型です。 可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。|
|名前|String|SAN のカスタム名|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```





