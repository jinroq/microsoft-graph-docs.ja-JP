---
title: windowsUniversalAppXAppAssignmentSettings リソースの種類
description: Windows ユニバーサル AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ebb9649460fbfa6da717ba099786eb7d4c2807da
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987007"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a>windowsUniversalAppXAppAssignmentSettings リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows ユニバーサル AppX のモバイル アプリケーションをグループに割り当てるときに使用するプロパティが含まれています。

[mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|useDeviceContext|ブール型 (Boolean)|Windows ユニバーサル AppX のモバイル アプリケーションの実行コンテキストのデバイスを使用するかどうかを指定します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```





