---
title: excludedApps リソースの種類
description: 除外された Office365 アプリのプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d90954bda8a5bd6c9bfdeb6af0d2946b48215d00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553051"
---
# <a name="excludedapps-resource-type"></a>excludedApps リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

除外された Office365 アプリのプロパティが含まれています。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|接続|ブール値|MS Office へのアクセスを除外する必要があるかどうかを示す値。|
|シート|ブール値|MS Office Excel を除外するかどうかを指定します。|
|スペース|ブール値|MS Office OneDrive for business-Groove を除外する必要があるかどうかを示す値。|
|もと|ブール値|MS Office InfoPath を除外する必要があるかどうかを示す値。|
|lync|ブール値|MS Office Skype for business-Lync を除外する必要があるかどうかを示す値。|
|スペース|ブール値|MS Office OneDrive を除外する必要があるかどうかを示す値。|
|ノート|ブール値|MS Office OneNote を除外する必要があるかどうかの値。|
|outlook|ブール値|MS Office Outlook を除外する必要があるかどうかを示す値。|
|しまう|ブール値|microsoft Office PowerPoint を除外するかどうかを指定します。|
|publisher|ブール値|MS Office Publisher を除外する必要があるかどうかの値。|
|sharepointdesigner|ブール値|MS Office sharepointdesigner を除外するかどうかを指定します。|
|teams|ブール値|MS Office Teams を除外する必要があるかどうかの値。|
|visio|ブール値|MS Office Visio を除外する必要があるかどうかを示す値。|
|段落|ブール値|MS Office Word を除外する必要があるかどうかを示す値。|

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





