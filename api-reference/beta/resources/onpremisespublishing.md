---
title: onPremisesPublishing リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff5ca6afc76ab60ab82f045d0309832e34e8d708
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840769"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="83286-103">onPremisesPublishing リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83286-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83286-104">**OnPremisesPublishing**オブジェクトは、社内[アプリケーション](application.md)を発行するための一連のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="83286-104">An **onPremisesPublishing** object represents the set of properties for publishing of on-premises [application](application.md).</span></span>

## <a name="properties"></a><span data-ttu-id="83286-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83286-105">Properties</span></span>

| <span data-ttu-id="83286-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83286-106">Property</span></span>|<span data-ttu-id="83286-107">型</span><span class="sxs-lookup"><span data-stu-id="83286-107">Type</span></span>|<span data-ttu-id="83286-108">説明</span><span class="sxs-lookup"><span data-stu-id="83286-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83286-109">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="83286-109">customDomainCertificate</span></span>|<span data-ttu-id="83286-110">String</span><span class="sxs-lookup"><span data-stu-id="83286-110">String</span></span>|<span data-ttu-id="83286-111">カスタムドメインが使用されているときに、アプリケーションに関連付けられている証明書の詳細。</span><span class="sxs-lookup"><span data-stu-id="83286-111">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="83286-112">既定のドメインを使用する場合は Null。</span><span class="sxs-lookup"><span data-stu-id="83286-112">Null when using the default domain.</span></span>|
|<span data-ttu-id="83286-113">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="83286-113">externalAuthenticationType</span></span>|<span data-ttu-id="83286-114">String</span><span class="sxs-lookup"><span data-stu-id="83286-114">String</span></span>|<span data-ttu-id="83286-115">詳細アプリケーションの事前認証設定の可能な値は`passthru`、、 `aadPreAuthentication`です。</span><span class="sxs-lookup"><span data-stu-id="83286-115">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="83286-116">externalUrl</span><span class="sxs-lookup"><span data-stu-id="83286-116">externalUrl</span></span>|<span data-ttu-id="83286-117">String</span><span class="sxs-lookup"><span data-stu-id="83286-117">String</span></span>|<span data-ttu-id="83286-118">アプリケーションの公開された外部 url。</span><span class="sxs-lookup"><span data-stu-id="83286-118">The published external url for the application.</span></span> <span data-ttu-id="83286-119">例えばhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="83286-119">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="83286-120">internalUrl</span><span class="sxs-lookup"><span data-stu-id="83286-120">internalUrl</span></span>|<span data-ttu-id="83286-121">String</span><span class="sxs-lookup"><span data-stu-id="83286-121">String</span></span>|<span data-ttu-id="83286-122">アプリケーションの内部 url。</span><span class="sxs-lookup"><span data-stu-id="83286-122">The internal url of the application.</span></span> <span data-ttu-id="83286-123">例えばhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="83286-123">For example https://intranet/</span></span> |
|<span data-ttu-id="83286-124">Isonprem発行が有効</span><span class="sxs-lookup"><span data-stu-id="83286-124">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="83286-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="83286-125">Boolean</span></span>|<span data-ttu-id="83286-126">アプリケーションが現在公開されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="83286-126">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="83286-127">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="83286-127">applicationServerTimeout</span></span>|<span data-ttu-id="83286-128">String</span><span class="sxs-lookup"><span data-stu-id="83286-128">String</span></span>|<span data-ttu-id="83286-129">この時間が経過すると、コネクタは、接続を閉じる前にバックエンドアプリケーションからの応答を待機します。</span><span class="sxs-lookup"><span data-stu-id="83286-129">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="83286-130">可能な値`default`は`long`、です。</span><span class="sxs-lookup"><span data-stu-id="83286-130">Possible values are `default`, `long`.</span></span> <span data-ttu-id="83286-131">サーバー `long`が要求に応答するのに60-75 秒以上かかる場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="83286-131">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="83286-132">また、 `long`アプリケーションにアクセスできず、エラー状態が "バックエンドタイムアウト" になっているかどうかを試してみてください。</span><span class="sxs-lookup"><span data-stu-id="83286-132">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="83286-133">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="83286-133">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="83286-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="83286-134">Boolean</span></span>|<span data-ttu-id="83286-135">アプリケーションが応答ヘッダー内の url を変換する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="83286-135">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="83286-136">これには、cookie の正しいサイトの設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="83286-136">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83286-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83286-137">JSON representation</span></span>

<span data-ttu-id="83286-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="83286-138">Here is a JSON representation of the resource.</span></span>

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
2019-02-04 14:57:30 UTC -->
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
