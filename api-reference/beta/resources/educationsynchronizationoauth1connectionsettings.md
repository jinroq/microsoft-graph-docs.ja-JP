---
title: educationSynchronizationOAuth1ConnectionSettings リソース
description: データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 71e45033c022061b72c1ea0be815ff3e0b611475
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516673"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="416e4-103">educationSynchronizationOAuth1ConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="416e4-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="416e4-104">データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="416e4-104">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="416e4-105">[Microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="416e4-105">Derived from [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="416e4-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="416e4-106">Properties</span></span>

<span data-ttu-id="416e4-107">この型では、追加のプロパティは公開されません。</span><span class="sxs-lookup"><span data-stu-id="416e4-107">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="416e4-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="416e4-108">JSON representation</span></span>
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
