---
title: windowsInformationProtectionResourceCollection リソースの種類
description: Windows 情報保護のリソース コレクション
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7b7e706e83753a49e7eece3d2efef95b7113a8cf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342090"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a>windowsInformationProtectionResourceCollection リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 情報保護のリソース コレクション

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|表示名|
|リソース|文字列コレクション|リソースのコレクション|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



