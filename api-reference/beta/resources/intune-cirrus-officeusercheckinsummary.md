---
title: officeUserCheckinSummary リソースの種類
description: チェックインのテナント統計 (stats) を記述するエンティティです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 374f5113a517b52ae7af6381f575ac60e5d00ae4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946582"
---
# <a name="officeusercheckinsummary-resource-type"></a>officeUserCheckinSummary リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

チェックインのテナント統計 (stats) を記述するエンティティです。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|succeededUserCount|Int32|成功したユーザーの合計は、過去 3 か月のアドインを確認します。|
|failedUserCount|Int32|障害が発生したユーザーの合計は、過去 3 か月のアドインを確認します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



