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
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="45cb0-103">educationSynchronizationOAuth1ConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="45cb0-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45cb0-104">OAuth1 を使用してデータプロバイダーに接続する場合は、この接続設定の種類を使用してプロファイルを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="45cb0-104">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="45cb0-105">[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="45cb0-105">Derived from [microsoft.graph.educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="45cb0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45cb0-106">Properties</span></span>

<span data-ttu-id="45cb0-107">この種類では、追加のプロパティは公開されていません。</span><span class="sxs-lookup"><span data-stu-id="45cb0-107">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="45cb0-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45cb0-108">JSON representation</span></span>
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
