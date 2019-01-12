---
title: educationSynchronizationOAuth1ConnectionSettings リソース
description: データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 80921488e1a5e0dd3e4ab4e21b2ea08e05ad9cee
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990265"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="1eca2-103">educationSynchronizationOAuth1ConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="1eca2-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

> <span data-ttu-id="1eca2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1eca2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1eca2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1eca2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1eca2-106">データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="1eca2-106">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="1eca2-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="1eca2-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1eca2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1eca2-108">Properties</span></span>

<span data-ttu-id="1eca2-109">この型では、追加のプロパティは公開されません。</span><span class="sxs-lookup"><span data-stu-id="1eca2-109">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1eca2-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1eca2-110">JSON representation</span></span>
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
