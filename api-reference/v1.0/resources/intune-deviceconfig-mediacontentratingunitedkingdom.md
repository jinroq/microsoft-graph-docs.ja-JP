---
title: mediaContentRatingUnitedKingdom リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8bdcd67bbc81cb5436c6be22c395a6c9804b0637
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951594"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a>mediaContentRatingUnitedKingdom リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

まだ文書化されていません
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|movieRating|[ratingUnitedKingdomMoviesType](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|評価の英国を選択したムービーです。 可能な値は、`allAllowed`、`allBlocked`、`general`、`universalChildren`、`parentalGuidance`、`agesAbove12Video`、`agesAbove12Cinema`、`agesAbove15`、`adults` です。|
|tvRating|[ratingUnitedKingdomTelevisionType](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|テレビの視聴制限が英国を選択します。 可能な値は、`allAllowed`、`allBlocked`、`caution` です。|

## <a name="relationships"></a>関係
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



