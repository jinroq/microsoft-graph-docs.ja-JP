---
title: educationOneRosterApiDataProvider リソース
description: OneRoster API は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。
author: mmast-msft
ms.openlocfilehash: 66c79c5e5d5ced4efcd635d2976e83887e545a9f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309570"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="dc98e-103">educationOneRosterApiDataProvider リソース</span><span class="sxs-lookup"><span data-stu-id="dc98e-103">educationOneRosterApiDataProvider resource</span></span>

> <span data-ttu-id="dc98e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dc98e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc98e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc98e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dc98e-106">[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="dc98e-106">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="dc98e-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="dc98e-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dc98e-108">Properties</span><span class="sxs-lookup"><span data-stu-id="dc98e-108">Properties</span></span>

| <span data-ttu-id="dc98e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc98e-109">Property</span></span> | <span data-ttu-id="dc98e-110">種類</span><span class="sxs-lookup"><span data-stu-id="dc98e-110">Type</span></span> | <span data-ttu-id="dc98e-111">説明</span><span class="sxs-lookup"><span data-stu-id="dc98e-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="dc98e-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="dc98e-112">**connectionUrl**</span></span> | <span data-ttu-id="dc98e-113">String</span><span class="sxs-lookup"><span data-stu-id="dc98e-113">String</span></span> | <span data-ttu-id="dc98e-114">OneRoster のインスタンスへの接続 URL です。</span><span class="sxs-lookup"><span data-stu-id="dc98e-114">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="dc98e-115">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="dc98e-115">**schoolsIds**</span></span> | <span data-ttu-id="dc98e-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dc98e-116">String collection</span></span> |  <span data-ttu-id="dc98e-117">同期するのには学校の sourcedIds のリスト。</span><span class="sxs-lookup"><span data-stu-id="dc98e-117">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="dc98e-118">**プロバイダー**</span><span class="sxs-lookup"><span data-stu-id="dc98e-118">**providerName**</span></span> | <span data-ttu-id="dc98e-119">String</span><span class="sxs-lookup"><span data-stu-id="dc98e-119">String</span></span> | <span data-ttu-id="dc98e-120">[OneRoster 仕様](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)で定義されているの OneRoster のサービス プロバイダーの名前です。</span><span class="sxs-lookup"><span data-stu-id="dc98e-120">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="dc98e-121">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="dc98e-121">**connectionSettings**</span></span> | [<span data-ttu-id="dc98e-122">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="dc98e-122">educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="dc98e-123">OneRoster インスタンスの接続の設定です。</span><span class="sxs-lookup"><span data-stu-id="dc98e-123">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="dc98e-124">型[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)または[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="dc98e-124">Should be of type [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="dc98e-125">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="dc98e-125">**customizations**</span></span> | [<span data-ttu-id="dc98e-126">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="dc98e-126">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="dc98e-127">同期プロファイルを適用するオプションのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="dc98e-127">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc98e-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc98e-128">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationoneRosterApiDataProvider",
    "connectionUrl": "String",
    "providerName": "String",
    "schoolsIds": [
        "String"
    ],
    "connectionSettings": {
        "@odata.type": "#microsoft.graph.educationSynchronizationOAuth1ConnectionSettings",
        "clientId": "String",
        "clientSecret": "String",
    },
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
