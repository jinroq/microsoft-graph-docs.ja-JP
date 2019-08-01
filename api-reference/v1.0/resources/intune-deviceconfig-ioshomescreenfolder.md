---
title: iosHomeScreenFolder リソースの種類
description: ホーム画面上のアプリのページが含まれるフォルダー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a22b20049c886b7cb1de2f7737b269fbd411749
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031521"
---
# <a name="ioshomescreenfolder-resource-type"></a>iosHomeScreenFolder リソースの種類

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ホーム画面上のアプリのページが含まれるフォルダー


[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承|
|pages|[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) コレクション|アプリケーションの種類にする必要がある、ホーム画面レイアウト アイコンで構成されるページ。 このコレクションには、最大で 500 個の要素を含めることができます。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```



