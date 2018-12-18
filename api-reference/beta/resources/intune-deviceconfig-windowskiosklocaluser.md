---
title: windowsKioskLocalUser リソースの種類
description: キオスクの構成にローカル ・ アカウントの識別に使用するクラス
author: tfitzmac
ms.openlocfilehash: 5ac98147172fd08fc9914a7d9302e3b074ca3246
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310823"
---
# <a name="windowskiosklocaluser-resource-type"></a>windowsKioskLocalUser リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

キオスクの構成にローカル ・ アカウントの識別に使用するクラス

[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|userName|String|この構成にキオスクがロックアウトされているローカル ユーザー|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```





