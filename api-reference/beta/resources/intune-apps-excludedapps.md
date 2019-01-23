---
title: excludedApps リソースの種類
description: Office365 アプリケーションの除外プロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d3cd9a159597689a64070181640415a6ce2fc61
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395679"
---
# <a name="excludedapps-resource-type"></a>excludedApps リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Office365 アプリケーションの除外プロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|アクセス|Boolean|値かの MS Office のアクセスを除外する必要があります。|
|excel|Boolean|値かの MS Office Excel を除外する必要があります。|
|溝|Boolean|値か、ビジネスの Groove の MS Office の OneDrive を除外する必要があります。|
|infoPath|Boolean|値かの MS Office InfoPath を除外する必要があります。|
|lync|Boolean|値か、ビジネス - Lync の MS Office の Skype を除外する必要があります。|
|oneDrive|Boolean|値かの MS Office の OneDrive を除外する必要があります。|
|oneNote|Boolean|値かの MS Office OneNote を除外する必要があります。|
|outlook|Boolean|値かの MS Office Outlook を除外する必要があります。|
|powerPoint|Boolean|値かの MS Office PowerPoint を除外する必要があります。|
|publisher|Boolean|値かの MS Office の発行元を除外する必要があります。|
|sharePointDesigner|Boolean|値かの MS Office の SharePointDesigner を除外する必要があります。|
|visio|Boolean|値かの MS Office Visio を除外する必要があります。|
|単語|Boolean|値かの MS Office の Word を除外する必要があります。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludedApps",
  "access": true,
  "excel": true,
  "groove": true,
  "infoPath": true,
  "lync": true,
  "oneDrive": true,
  "oneNote": true,
  "outlook": true,
  "powerPoint": true,
  "publisher": true,
  "sharePointDesigner": true,
  "visio": true,
  "word": true
}
```




