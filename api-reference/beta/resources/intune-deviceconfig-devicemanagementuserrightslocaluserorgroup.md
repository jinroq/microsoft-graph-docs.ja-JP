---
title: deviceManagementUserRightsLocalUserOrGroup リソースの種類
description: ローカル ユーザーまたはグループのユーザー権利の設定の使用に関する情報を表します。
ms.openlocfilehash: bf81a36a8e102bea4c3e8fb56e45bf7822cf31a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070641"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>deviceManagementUserRightsLocalUserOrGroup リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ローカル ユーザーまたはグループのユーザー権利の設定の使用に関する情報を表します。
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|名前|String|ローカル ユーザーまたはグループの名前です。|
|説明|String|ローカル ユーザーまたはグループの管理の説明です。|
|securityIdentifier|String|このローカル ユーザーまたはグループのセキュリティ識別子 (例: * S-1-5-32-544)。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





