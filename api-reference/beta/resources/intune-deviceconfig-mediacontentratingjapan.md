---
title: mediaContentRatingJapan リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b1c79e68a530d176445b0395fdb7c4d50996485
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950887"
---
# <a name="mediacontentratingjapan-resource-type"></a>mediaContentRatingJapan リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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




