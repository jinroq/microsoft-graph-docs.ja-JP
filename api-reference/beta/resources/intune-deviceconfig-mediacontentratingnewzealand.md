---
title: mediaContentRatingNewZealand リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48698cf0f35fc39c8e385d391344914ea34745ea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950880"
---
# <a name="mediacontentratingnewzealand-resource-type"></a>mediaContentRatingNewZealand リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|movieRating|[ratingNewZealandMoviesType](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|ニュージーランドで選択されている映画のレーティング。 使用可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`mature`、`agesAbove13`、`agesAbove15`、`agesAbove16`、`agesAbove18`、`restricted`、`agesAbove16Restricted` です。|
|tvRating|[ratingNewZealandTelevisionType](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|ニュージーランド用に選択されているテレビのレーティング。 可能な値は、`allAllowed`、`allBlocked`、`general`、`parentalGuidance`、`adults` です。|

## <a name="relationships"></a>関係
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




