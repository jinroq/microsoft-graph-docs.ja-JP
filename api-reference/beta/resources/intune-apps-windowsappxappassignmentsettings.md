---
title: windowsAppXAppAssignmentSettings リソースの種類
description: Windows AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。
ms.openlocfilehash: ce65e3fbc841e2df6dc378b7f440fd588c7bf1d5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068408"
---
# <a name="windowsappxappassignmentsettings-resource-type"></a>windowsAppXAppAssignmentSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。

[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|useDeviceContext|ブール型 (Boolean)|Windows AppX のモバイル アプリケーションの実行コンテキストのデバイスを使用するかどうかを指定します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





