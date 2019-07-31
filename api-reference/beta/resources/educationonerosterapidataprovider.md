---
title: educationOneRosterApiDataProvider リソース
description: OneRoster API が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca94043fdf215d47a1ccaf16f3a667f1178c1d57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972636"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="3ab3e-103">educationOneRosterApiDataProvider リソース</span><span class="sxs-lookup"><span data-stu-id="3ab3e-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ab3e-104">[ONEROSTER API](https://www.imsglobal.org/activity/onerosterlis)が入力ソースとして使用されている場合に、学校データ同期プロファイルを設定するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="3ab3e-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="3ab3e-105">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="3ab3e-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3ab3e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ab3e-106">Properties</span></span>

| <span data-ttu-id="3ab3e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3ab3e-107">Property</span></span> | <span data-ttu-id="3ab3e-108">型</span><span class="sxs-lookup"><span data-stu-id="3ab3e-108">Type</span></span> | <span data-ttu-id="3ab3e-109">説明</span><span class="sxs-lookup"><span data-stu-id="3ab3e-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="3ab3e-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="3ab3e-110">**connectionUrl**</span></span> | <span data-ttu-id="3ab3e-111">String</span><span class="sxs-lookup"><span data-stu-id="3ab3e-111">String</span></span> | <span data-ttu-id="3ab3e-112">OneRoster インスタンスへの接続 URL。</span><span class="sxs-lookup"><span data-stu-id="3ab3e-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="3ab3e-113">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="3ab3e-113">**schoolsIds**</span></span> | <span data-ttu-id="3ab3e-114">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3ab3e-114">String collection</span></span> |  <span data-ttu-id="3ab3e-115">同期する school sourcedIds のリスト。</span><span class="sxs-lookup"><span data-stu-id="3ab3e-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="3ab3e-116">**プロバイダー**</span><span class="sxs-lookup"><span data-stu-id="3ab3e-116">**providerName**</span></span> | <span data-ttu-id="3ab3e-117">String</span><span class="sxs-lookup"><span data-stu-id="3ab3e-117">String</span></span> | <span data-ttu-id="3ab3e-118">[OneRoster 仕様](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)で定義されている OneRoster サービスプロバイダー名。</span><span class="sxs-lookup"><span data-stu-id="3ab3e-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="3ab3e-119">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="3ab3e-119">**connectionSettings**</span></span> | [<span data-ttu-id="3ab3e-120">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="3ab3e-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="3ab3e-121">OneRoster インスタンスの接続設定。</span><span class="sxs-lookup"><span data-stu-id="3ab3e-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="3ab3e-122">[EducationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)または[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)の種類である必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ab3e-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="3ab3e-123">**ユーザー**</span><span class="sxs-lookup"><span data-stu-id="3ab3e-123">**customizations**</span></span> | [<span data-ttu-id="3ab3e-124">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="3ab3e-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="3ab3e-125">同期プロファイルに適用されるカスタマイズ (オプション)。</span><span class="sxs-lookup"><span data-stu-id="3ab3e-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ab3e-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3ab3e-126">JSON representation</span></span>
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
