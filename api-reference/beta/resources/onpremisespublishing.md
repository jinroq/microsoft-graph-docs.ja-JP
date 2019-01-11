---
title: onPremisesPublishing リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 30ff6908a42a690e07d71b5d0c62fcb22dea3c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842540"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="c4a65-103">onPremisesPublishing リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4a65-103">onPremisesPublishing resource type</span></span>

> <span data-ttu-id="c4a65-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4a65-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4a65-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4a65-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="c4a65-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4a65-106">Properties</span></span>
| <span data-ttu-id="c4a65-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4a65-107">Property</span></span>     | <span data-ttu-id="c4a65-108">種類</span><span class="sxs-lookup"><span data-stu-id="c4a65-108">Type</span></span>   |<span data-ttu-id="c4a65-109">説明</span><span class="sxs-lookup"><span data-stu-id="c4a65-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4a65-110">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="c4a65-110">customDomainCertificate</span></span>|<span data-ttu-id="c4a65-111">String</span><span class="sxs-lookup"><span data-stu-id="c4a65-111">String</span></span>|<span data-ttu-id="c4a65-112">カスタムのドメインが使用しているときに、アプリケーションに関連付けられている証明書の詳細です。</span><span class="sxs-lookup"><span data-stu-id="c4a65-112">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="c4a65-113">既定のドメインを使用する場合は null にします。</span><span class="sxs-lookup"><span data-stu-id="c4a65-113">Null when using the default domain.</span></span>|
|<span data-ttu-id="c4a65-114">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="c4a65-114">externalAuthenticationType</span></span>|<span data-ttu-id="c4a65-115">String</span><span class="sxs-lookup"><span data-stu-id="c4a65-115">String</span></span>|<span data-ttu-id="c4a65-116">アプリケーションの使用可能な値は、事前認証の設定の詳細: `passthru`、 `aadPreAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="c4a65-116">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="c4a65-117">externalUrl</span><span class="sxs-lookup"><span data-stu-id="c4a65-117">externalUrl</span></span>|<span data-ttu-id="c4a65-118">String</span><span class="sxs-lookup"><span data-stu-id="c4a65-118">String</span></span>|<span data-ttu-id="c4a65-119">アプリケーションの公開済みの外部 url です。</span><span class="sxs-lookup"><span data-stu-id="c4a65-119">The published external url for the application.</span></span> <span data-ttu-id="c4a65-120">例えばhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="c4a65-120">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="c4a65-121">internalUrl</span><span class="sxs-lookup"><span data-stu-id="c4a65-121">internalUrl</span></span>|<span data-ttu-id="c4a65-122">String</span><span class="sxs-lookup"><span data-stu-id="c4a65-122">String</span></span>|<span data-ttu-id="c4a65-123">アプリケーションの内部の url です。</span><span class="sxs-lookup"><span data-stu-id="c4a65-123">The internal url of the application.</span></span> <span data-ttu-id="c4a65-124">例えばhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="c4a65-124">For example https://intranet/</span></span> |
|<span data-ttu-id="c4a65-125">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="c4a65-125">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="c4a65-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="c4a65-126">Boolean</span></span>|<span data-ttu-id="c4a65-127">アプリケーションをか現在発行されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c4a65-127">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="c4a65-128">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="c4a65-128">applicationServerTimeout</span></span>|<span data-ttu-id="c4a65-129">String</span><span class="sxs-lookup"><span data-stu-id="c4a65-129">String</span></span>|<span data-ttu-id="c4a65-130">コネクタが接続を閉じる前に、バックエンド アプリケーションからの応答を待機する期間。</span><span class="sxs-lookup"><span data-stu-id="c4a65-130">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="c4a65-131">使用可能な値は、 `default`、 `long`。</span><span class="sxs-lookup"><span data-stu-id="c4a65-131">Possible values are `default`, `long`.</span></span> <span data-ttu-id="c4a65-132">使用`long`場合、サーバーは要求に応答するのには 60 ~ 75 秒以上です。</span><span class="sxs-lookup"><span data-stu-id="c4a65-132">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="c4a65-133">`long`アプリケーションにアクセスできないし、エラー ・ ステータスは、「バックエンド ・ タイムアウト」です。</span><span class="sxs-lookup"><span data-stu-id="c4a65-133">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="c4a65-134">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="c4a65-134">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="c4a65-135">ブール型</span><span class="sxs-lookup"><span data-stu-id="c4a65-135">Boolean</span></span>|<span data-ttu-id="c4a65-136">アプリケーションが応答ヘッダー内の url を変換する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c4a65-136">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="c4a65-137">これには、適切なサイトの cookie の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="c4a65-137">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4a65-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4a65-138">JSON representation</span></span>

<span data-ttu-id="c4a65-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c4a65-139">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
