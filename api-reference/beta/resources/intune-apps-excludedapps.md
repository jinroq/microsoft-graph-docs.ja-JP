---
title: excludedApps リソースの種類
description: 除外された Office365 アプリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8dee0d5328f1f69c95159116bf913bc2abb959d7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571691"
---
# <a name="excludedapps-resource-type"></a>excludedApps リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

除外された Office365 アプリのプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|接続|Boolean|MS Office へのアクセスを除外する必要があるかどうかを示す値。|
|シート|Boolean|MS Office Excel を除外するかどうかを指定します。|
|スペース|Boolean|MS Office OneDrive for business-Groove を除外する必要があるかどうかを示す値。|
|もと|Boolean|MS Office InfoPath を除外する必要があるかどうかを示す値。|
|lync|Boolean|MS Office Skype for business-Lync を除外する必要があるかどうかを示す値。|
|スペース|Boolean|MS Office OneDrive を除外する必要があるかどうかを示す値。|
|ノート|Boolean|MS Office OneNote を除外する必要があるかどうかの値。|
|outlook|Boolean|MS Office Outlook を除外する必要があるかどうかを示す値。|
|しまう|Boolean|microsoft Office PowerPoint を除外するかどうかを指定します。|
|publisher|Boolean|MS Office Publisher を除外する必要があるかどうかの値。|
|sharepointdesigner|Boolean|MS Office sharepointdesigner を除外するかどうかを指定します。|
|teams|Boolean|MS Office Teams を除外する必要があるかどうかの値。|
|visio|Boolean|MS Office Visio を除外する必要があるかどうかを示す値。|
|段落|Boolean|MS Office Word を除外する必要があるかどうかを示す値。|

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
  "teams": true,
  "visio": true,
  "word": true
}
```




