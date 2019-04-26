---
title: onPremisesPublishing リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 8531a68ad56dad0f44ef8cd55e9fabeff47a6c2e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341801"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="5c1da-103">onPremisesPublishing リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c1da-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="5c1da-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c1da-104">Properties</span></span>
| <span data-ttu-id="5c1da-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c1da-105">Property</span></span>     | <span data-ttu-id="5c1da-106">型</span><span class="sxs-lookup"><span data-stu-id="5c1da-106">Type</span></span>   |<span data-ttu-id="5c1da-107">説明</span><span class="sxs-lookup"><span data-stu-id="5c1da-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c1da-108">customdomaincertificate</span><span class="sxs-lookup"><span data-stu-id="5c1da-108">customDomainCertificate</span></span>|<span data-ttu-id="5c1da-109">String</span><span class="sxs-lookup"><span data-stu-id="5c1da-109">String</span></span>|<span data-ttu-id="5c1da-110">カスタムドメインが使用されているときに、アプリケーションに関連付けられている証明書の詳細。</span><span class="sxs-lookup"><span data-stu-id="5c1da-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="5c1da-111">既定のドメインを使用する場合は Null。</span><span class="sxs-lookup"><span data-stu-id="5c1da-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="5c1da-112">externalauthenticationtype</span><span class="sxs-lookup"><span data-stu-id="5c1da-112">externalAuthenticationType</span></span>|<span data-ttu-id="5c1da-113">String</span><span class="sxs-lookup"><span data-stu-id="5c1da-113">String</span></span>|<span data-ttu-id="5c1da-114">詳細アプリケーションの事前認証設定の可能な値は`passthru`、、 `aadPreAuthentication`です。</span><span class="sxs-lookup"><span data-stu-id="5c1da-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="5c1da-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="5c1da-115">externalUrl</span></span>|<span data-ttu-id="5c1da-116">String</span><span class="sxs-lookup"><span data-stu-id="5c1da-116">String</span></span>|<span data-ttu-id="5c1da-117">アプリケーションの公開された外部 url。</span><span class="sxs-lookup"><span data-stu-id="5c1da-117">The published external url for the application.</span></span> <span data-ttu-id="5c1da-118">例えばhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="5c1da-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="5c1da-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="5c1da-119">internalUrl</span></span>|<span data-ttu-id="5c1da-120">String</span><span class="sxs-lookup"><span data-stu-id="5c1da-120">String</span></span>|<span data-ttu-id="5c1da-121">アプリケーションの内部 url。</span><span class="sxs-lookup"><span data-stu-id="5c1da-121">The internal url of the application.</span></span> <span data-ttu-id="5c1da-122">例えばhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="5c1da-122">For example https://intranet/</span></span> |
|<span data-ttu-id="5c1da-123">isonprem発行が有効</span><span class="sxs-lookup"><span data-stu-id="5c1da-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="5c1da-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c1da-124">Boolean</span></span>|<span data-ttu-id="5c1da-125">アプリケーションが現在公開されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c1da-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="5c1da-126">applicationservertimeout</span><span class="sxs-lookup"><span data-stu-id="5c1da-126">applicationServerTimeout</span></span>|<span data-ttu-id="5c1da-127">String</span><span class="sxs-lookup"><span data-stu-id="5c1da-127">String</span></span>|<span data-ttu-id="5c1da-128">この時間が経過すると、コネクタは、接続を閉じる前にバックエンドアプリケーションからの応答を待機します。</span><span class="sxs-lookup"><span data-stu-id="5c1da-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="5c1da-129">可能な値`default`は`long`、です。</span><span class="sxs-lookup"><span data-stu-id="5c1da-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="5c1da-130">サーバー `long`が要求に応答するのに60-75 秒以上かかる場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="5c1da-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="5c1da-131">また、 `long`アプリケーションにアクセスできず、エラー状態が "バックエンドタイムアウト" になっているかどうかを試してみてください。</span><span class="sxs-lookup"><span data-stu-id="5c1da-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="5c1da-132">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="5c1da-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="5c1da-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c1da-133">Boolean</span></span>|<span data-ttu-id="5c1da-134">アプリケーションが応答ヘッダー内の url を変換する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5c1da-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="5c1da-135">これには、cookie の正しいサイトの設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5c1da-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c1da-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c1da-136">JSON representation</span></span>

<span data-ttu-id="5c1da-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5c1da-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
