---
title: educationSynchronizationOAuth1ConnectionSettings リソース
description: データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
ms.openlocfilehash: 17bfbed14bf22d8b30d82766985d64595204d05b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072189"
---
# <a name="educationsynchronizationoauth1connectionsettings-resource"></a><span data-ttu-id="ce65e-103">educationSynchronizationOAuth1ConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="ce65e-103">educationSynchronizationOAuth1ConnectionSettings resource</span></span>

> <span data-ttu-id="ce65e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ce65e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ce65e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce65e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ce65e-106">データ プロバイダーへの接続に使用する OAuth1 がある場合は、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="ce65e-106">When OAuth1 is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="ce65e-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="ce65e-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ce65e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce65e-108">Properties</span></span>

<span data-ttu-id="ce65e-109">この型では、追加のプロパティは公開されません。</span><span class="sxs-lookup"><span data-stu-id="ce65e-109">No additional properties are exposed by this type.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce65e-110">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce65e-110">JSON representation</span></span>
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
