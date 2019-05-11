---
title: excludedApps リソースの種類
description: 除外された Office365 アプリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37abd83b34fde565aa78e62454c4ce7d47ea192a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950411"
---
# <a name="excludedapps-resource-type"></a>excludedApps リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

除外された Office365 アプリのプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|接続|Boolean|MS Office へのアクセスを除外する必要があるかどうかを示す値。|
|シート|Boolean|MS Office Excel を除外するかどうかを指定します。|
|スペース|Boolean|MS Office OneDrive for Business-Groove を除外する必要があるかどうかを示す値。|
|もと|Boolean|MS Office InfoPath を除外する必要があるかどうかを示す値。|
|lync|Boolean|MS Office Skype for Business-Lync を除外する必要があるかどうかを示す値。|
|スペース|Boolean|MS Office OneDrive を除外する必要があるかどうかを示す値。|
|ノート|Boolean|MS Office OneNote を除外する必要があるかどうかの値。|
|outlook|Boolean|MS Office Outlook を除外する必要があるかどうかを示す値。|
|しまう|Boolean|MICROSOFT Office PowerPoint を除外するかどうかを指定します。|
|publisher|Boolean|MS Office Publisher を除外する必要があるかどうかの値。|
|sharePointDesigner|Boolean|MS Office SharePointDesigner を除外するかどうかを指定します。|
|teams|Boolean|MS Office Teams を除外する必要があるかどうかの値。|
|visio|Boolean|MS Office Visio を除外する必要があるかどうかを示す値。|
|段落|Boolean|MS Office Word を除外する必要があるかどうかを示す値。|

## <a name="relationships"></a>関係
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




