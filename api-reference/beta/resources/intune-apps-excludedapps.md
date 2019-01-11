---
title: excludedApps リソースの種類
description: Office365 アプリケーションの除外プロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b2ec66c83c13088fb289e271e604154195902ca5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821883"
---
# <a name="excludedapps-resource-type"></a>excludedApps リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Office365 アプリケーションの除外プロパティが含まれています。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|アクセス|ブール型|値かの MS Office のアクセスを除外する必要があります。|
|excel|ブール型|値かの MS Office Excel を除外する必要があります。|
|溝|ブール型|値か、ビジネスの Groove の MS Office の OneDrive を除外する必要があります。|
|infoPath|ブール型|値かの MS Office InfoPath を除外する必要があります。|
|lync|ブール型|値か、ビジネス - Lync の MS Office の Skype を除外する必要があります。|
|oneDrive|ブール型|値かの MS Office の OneDrive を除外する必要があります。|
|oneNote|ブール型|値かの MS Office OneNote を除外する必要があります。|
|outlook|ブール型|値かの MS Office Outlook を除外する必要があります。|
|powerPoint|ブール型|値かの MS Office PowerPoint を除外する必要があります。|
|publisher|ブール型|値かの MS Office の発行元を除外する必要があります。|
|sharePointDesigner|ブール型|値かの MS Office の SharePointDesigner を除外する必要があります。|
|visio|ブール型|値かの MS Office Visio を除外する必要があります。|
|単語|ブール型|値かの MS Office の Word を除外する必要があります。|

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





