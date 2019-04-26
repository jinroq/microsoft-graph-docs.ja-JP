---
title: educationOneRosterApiDataProvider リソース
description: OneRoster API が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4ac232f71600f701efd8d085386fa9070773b475
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334190"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="b27d9-103">educationOneRosterApiDataProvider リソース</span><span class="sxs-lookup"><span data-stu-id="b27d9-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b27d9-104">[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="b27d9-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="b27d9-105">[educationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="b27d9-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b27d9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b27d9-106">Properties</span></span>

| <span data-ttu-id="b27d9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b27d9-107">Property</span></span> | <span data-ttu-id="b27d9-108">型</span><span class="sxs-lookup"><span data-stu-id="b27d9-108">Type</span></span> | <span data-ttu-id="b27d9-109">説明</span><span class="sxs-lookup"><span data-stu-id="b27d9-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b27d9-110">**connectionurl**</span><span class="sxs-lookup"><span data-stu-id="b27d9-110">**connectionUrl**</span></span> | <span data-ttu-id="b27d9-111">String</span><span class="sxs-lookup"><span data-stu-id="b27d9-111">String</span></span> | <span data-ttu-id="b27d9-112">OneRoster インスタンスへの接続 URL。</span><span class="sxs-lookup"><span data-stu-id="b27d9-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="b27d9-113">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="b27d9-113">**schoolsIds**</span></span> | <span data-ttu-id="b27d9-114">String collection</span><span class="sxs-lookup"><span data-stu-id="b27d9-114">String collection</span></span> |  <span data-ttu-id="b27d9-115">同期する school sourcedids のリスト。</span><span class="sxs-lookup"><span data-stu-id="b27d9-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="b27d9-116">**プロバイダー**</span><span class="sxs-lookup"><span data-stu-id="b27d9-116">**providerName**</span></span> | <span data-ttu-id="b27d9-117">String</span><span class="sxs-lookup"><span data-stu-id="b27d9-117">String</span></span> | <span data-ttu-id="b27d9-118">[OneRoster 仕様](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)で定義されている OneRoster サービスプロバイダー名。</span><span class="sxs-lookup"><span data-stu-id="b27d9-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="b27d9-119">**connectionsettings**</span><span class="sxs-lookup"><span data-stu-id="b27d9-119">**connectionSettings**</span></span> | [<span data-ttu-id="b27d9-120">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="b27d9-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="b27d9-121">OneRoster インスタンスの接続設定。</span><span class="sxs-lookup"><span data-stu-id="b27d9-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="b27d9-122">[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)または[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)の種類である必要があります。</span><span class="sxs-lookup"><span data-stu-id="b27d9-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="b27d9-123">**ユーザー**</span><span class="sxs-lookup"><span data-stu-id="b27d9-123">**customizations**</span></span> | [<span data-ttu-id="b27d9-124">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="b27d9-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="b27d9-125">同期プロファイルに適用されるカスタマイズ (オプション)。</span><span class="sxs-lookup"><span data-stu-id="b27d9-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b27d9-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b27d9-126">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
