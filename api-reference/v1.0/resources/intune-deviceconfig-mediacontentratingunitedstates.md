---
title: mediaContentRatingUnitedStates リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: baa5d98f0fcb1d267221c95c0b27be988d3a197f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572319"
---
# <a name="mediacontentratingunitedstates-resource-type"></a>mediaContentRatingUnitedStates リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|movieRating|[ratingUnitedStatesMoviesType](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|米国向けに選択されている映画のレーティング。 可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`parentalGuidance13`、`restricted`、`adults` です。|
|tvRating|[ratingUnitedStatesTelevisionType](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|米国向けに選択されているテレビのレーティング。 可能な値は、`allAllowed`、`allBlocked`、`childrenAll`、`childrenAbove7`、`general`、`parentalGuidance`、`childrenAbove14`、`adults` です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



