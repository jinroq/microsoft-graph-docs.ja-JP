---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0543aec86312d90a5896ed3f06f004c87d8e6a58
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574181"
---
# <a name="mediacontentratingjapan-resource-type"></a>mediaContentRatingJapan リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|movieRating|[ratingJapanMoviesType](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|日本向けに選択されている映画のレーティング。 使用可能な値: `allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`agesAbove15`、`agesAbove18`。|
|tvRating|[ratingJapanTelevisionType](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|日本向けに選択されているテレビのレーティング。 可能な値は、`allAllowed`、`allBlocked`、`explicitAllowed` です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



