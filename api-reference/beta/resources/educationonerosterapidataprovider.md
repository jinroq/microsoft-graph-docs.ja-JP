---
title: educationOneRosterApiDataProvider リソース
description: OneRoster API は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 681a3331aba7bc84ac80911c4be8076d104f8a58
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938147"
---
# <a name="educationonerosterapidataprovider-resource"></a><span data-ttu-id="c4c83-103">educationOneRosterApiDataProvider リソース</span><span class="sxs-lookup"><span data-stu-id="c4c83-103">educationOneRosterApiDataProvider resource</span></span>

> <span data-ttu-id="c4c83-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4c83-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4c83-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4c83-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4c83-106">[OneRoster API](https://www.imsglobal.org/activity/onerosterlis)は、入力ソースとして使用するときに、学校のデータの同期プロファイルを設定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="c4c83-106">Used to set up the school data synchronization profile when the [OneRoster API](https://www.imsglobal.org/activity/onerosterlis) is used as the input source.</span></span>

<span data-ttu-id="c4c83-107">[EducationSynchronizationDataProvider](educationsynchronizationdataprovider.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="c4c83-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c4c83-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4c83-108">Properties</span></span>

| <span data-ttu-id="c4c83-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4c83-109">Property</span></span> | <span data-ttu-id="c4c83-110">種類</span><span class="sxs-lookup"><span data-stu-id="c4c83-110">Type</span></span> | <span data-ttu-id="c4c83-111">説明</span><span class="sxs-lookup"><span data-stu-id="c4c83-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c4c83-112">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="c4c83-112">**connectionUrl**</span></span> | <span data-ttu-id="c4c83-113">String</span><span class="sxs-lookup"><span data-stu-id="c4c83-113">String</span></span> | <span data-ttu-id="c4c83-114">OneRoster のインスタンスへの接続 URL です。</span><span class="sxs-lookup"><span data-stu-id="c4c83-114">The connection URL to the OneRoster instance.</span></span> |
| <span data-ttu-id="c4c83-115">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="c4c83-115">**schoolsIds**</span></span> | <span data-ttu-id="c4c83-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c4c83-116">String collection</span></span> |  <span data-ttu-id="c4c83-117">同期するのには学校の sourcedIds のリスト。</span><span class="sxs-lookup"><span data-stu-id="c4c83-117">The list of school sourcedIds to sync.</span></span> |
| <span data-ttu-id="c4c83-118">**プロバイダー**</span><span class="sxs-lookup"><span data-stu-id="c4c83-118">**providerName**</span></span> | <span data-ttu-id="c4c83-119">String</span><span class="sxs-lookup"><span data-stu-id="c4c83-119">String</span></span> | <span data-ttu-id="c4c83-120">[OneRoster 仕様](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA)で定義されているの OneRoster のサービス プロバイダーの名前です。</span><span class="sxs-lookup"><span data-stu-id="c4c83-120">The OneRoster Service Provider name as defined by the [OneRoster specification](https://www.imsglobal.org/oneroster-v11-final-best-practice-and-implementation-guide#AppA).</span></span> |
| <span data-ttu-id="c4c83-121">**connectionSettings**</span><span class="sxs-lookup"><span data-stu-id="c4c83-121">**connectionSettings**</span></span> | [<span data-ttu-id="c4c83-122">educationSynchronizationConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="c4c83-122">educationSynchronizationConnectionSettings</span></span>](educationsynchronizationconnectionsettings.md) | <span data-ttu-id="c4c83-123">OneRoster インスタンスの接続の設定です。</span><span class="sxs-lookup"><span data-stu-id="c4c83-123">Connection settings for the OneRoster instance.</span></span> <span data-ttu-id="c4c83-124">型[educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md)または[educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md)でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="c4c83-124">Should be of type [educationSynchronizationOAuth1ConnectionSettings](educationsynchronizationoauth1connectionsettings.md) or [educationSynchronizationOAuth2ClientCredentialsConnectionSettings](educationsynchronizationoauth2clientcredentialsconnectionsettings.md).</span></span> |
| <span data-ttu-id="c4c83-125">**カスタマイズ**</span><span class="sxs-lookup"><span data-stu-id="c4c83-125">**customizations**</span></span> | [<span data-ttu-id="c4c83-126">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="c4c83-126">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="c4c83-127">同期プロファイルを適用するオプションのカスタマイズ。</span><span class="sxs-lookup"><span data-stu-id="c4c83-127">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4c83-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4c83-128">JSON representation</span></span>
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
