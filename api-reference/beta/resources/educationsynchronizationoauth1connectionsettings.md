---
title: educationSynchronizationOAuth1ConnectionSettings リソース
description: データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
localization_priority: Normal
ms.openlocfilehash: 30c4abce27b1b9593346bcb0392581eb83c7830e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894153"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="e76ab-103">educationSynchronizationOAuth1ConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="e76ab-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

> <span data-ttu-id="e76ab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e76ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e76ab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e76ab-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e76ab-106">データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="e76ab-106">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="e76ab-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="e76ab-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e76ab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e76ab-108">Properties</span></span>

<span data-ttu-id="e76ab-109">この型では、追加のプロパティは公開されません。</span><span class="sxs-lookup"><span data-stu-id="e76ab-109">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e76ab-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e76ab-110">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
    "clientId": "String",
    "clientSecret": "String"
}
```
