---
title: officeUserCheckinSummary リソースの種類
description: テナントのチェックイン統計を記述するエンティティ。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 9ee53bbdbb02a3d5716f49941ec108e23a09ae88
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949270"
---
# <a name="officeusercheckinsummary-resource-type"></a>officeUserCheckinSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

テナントのチェックイン統計を記述するエンティティ。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|succeededUserCount|Int32|過去3か月間の成功したユーザーチェックインの合計数。|
|failedUserCount|Int32|過去3か月間のユーザーチェックに失敗した合計数。|

## <a name="relationships"></a>関係
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



