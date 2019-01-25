---
title: educationOneRosterApiDataProvider リソース
description: OneRoster API は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 55a3cd0e20f15c4b7d44bc7aebdc19f202e044f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527984"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="5183b-103">educationOneRosterApiDataProvider リソース</span><span class="sxs-lookup"><span data-stu-id="5183b-103">educationOneRosterApiDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5183b-104">[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="5183b-104">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="5183b-105">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="5183b-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5183b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5183b-106">Properties</span></span>

| <span data-ttu-id="5183b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5183b-107">Property</span></span> | <span data-ttu-id="5183b-108">型</span><span class="sxs-lookup"><span data-stu-id="5183b-108">Type</span></span> | <span data-ttu-id="5183b-109">説明</span><span class="sxs-lookup"><span data-stu-id="5183b-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5183b-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="5183b-110">**connectionUrl**</span></span> | <span data-ttu-id="5183b-111">String</span><span class="sxs-lookup"><span data-stu-id="5183b-111">String</span></span> | <span data-ttu-id="5183b-112">OneRoster のインスタンスへの接続 URL です。</span><span class="sxs-lookup"><span data-stu-id="5183b-112">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="5183b-113">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="5183b-113">**schoolsIds**</span></span> | <span data-ttu-id="5183b-114">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5183b-114">String collection</span></span> |  <span data-ttu-id="5183b-115">同期するのには学校の sourcedIds のリスト。</span><span class="sxs-lookup"><span data-stu-id="5183b-115">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="5183b-116">ProviderName</span><span class="sxs-lookup"><span data-stu-id="5183b-116">**providerName**</span></span> | <span data-ttu-id="5183b-117">String</span><span class="sxs-lookup"><span data-stu-id="5183b-117">String</span></span> | <span data-ttu-id="5183b-118">[OneRoster 仕様](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)で定義されているの OneRoster のサービス プロバイダーの名前です。</span><span class="sxs-lookup"><span data-stu-id="5183b-118">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="5183b-119">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="5183b-119">**connectionSettings**</span></span> | [<span data-ttu-id="5183b-120">microsoft.graph.educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="5183b-120">microsoft.graph.educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="5183b-121">OneRoster インスタンスの接続の設定です。</span><span class="sxs-lookup"><span data-stu-id="5183b-121">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="5183b-122">型[microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)または[microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="5183b-122">Should be of type [microsoft.graph.educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="5183b-123">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="5183b-123">**customizations**</span></span> | [<span data-ttu-id="5183b-124">microsoft.graph.educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="5183b-124">microsoft.graph.educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="5183b-125">同期プロファイルを適用するオプションのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="5183b-125">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5183b-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5183b-126">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonerosterapidataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
