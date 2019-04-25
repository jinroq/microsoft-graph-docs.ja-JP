---
title: mediaContentRatingGermany リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e3c59bf110c55492db49a81a557cef0b421e328
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572382"
---
# <a name="mediacontentratinggermany-resource-type"></a>mediaContentRatingGermany リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|movieRating|[ratingGermanyMoviesType](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|ドイツ向けに選択されている映画のレーティング。 可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。|
|tvRating|[ratingGermanyTelevisionType](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|ドイツ向けに選択されているテレビのレーティング。 可能な値は、`allAllowed`、`allBlocked`、`general`、`agesAbove6`、`agesAbove12`、`agesAbove16`、`adults` です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



