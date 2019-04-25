---
title: educationSynchronizationOAuth1ConnectionSettings リソース
description: OAuth1 を使用してデータプロバイダーに接続する場合は、この接続設定の種類を使用してプロファイルを設定する必要があります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 71e45033c022061b72c1ea0be815ff3e0b611475
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542823"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a>educationSynchronizationOAuth1ConnectionSettings リソース

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

OAuth1 を使用してデータプロバイダーに接続する場合は、この接続設定の種類を使用してプロファイルを設定する必要があります。

[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。

## <a name="properties"></a>プロパティ

この種類では、追加のプロパティは公開されていません。

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationoauth1connectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
