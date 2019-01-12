---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a1866a6bf0c8d1849eb2fbf478b4f5d14fa3e5c0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916937"
---
# <a name="mediacontentratingnewzealand-resource-type"></a>mediaContentRatingNewZealand リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|movieRating|[ratingNewZealandMoviesType](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|評価のニュージーランドを選択したムービーです。 可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。|
|tvRating|[ratingNewZealandTelevisionType](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|テレビの視聴制限がニュージーランドを選択します。 可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```





