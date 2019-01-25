---
title: onPremisesPublishing リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508182"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="4ef7a-103">onPremisesPublishing リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4ef7a-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="4ef7a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ef7a-104">Properties</span></span>
| <span data-ttu-id="4ef7a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ef7a-105">Property</span></span>     | <span data-ttu-id="4ef7a-106">型</span><span class="sxs-lookup"><span data-stu-id="4ef7a-106">Type</span></span>   |<span data-ttu-id="4ef7a-107">説明</span><span class="sxs-lookup"><span data-stu-id="4ef7a-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ef7a-108">customDomainCertificate</span><span class="sxs-lookup"><span data-stu-id="4ef7a-108">customDomainCertificate</span></span>|<span data-ttu-id="4ef7a-109">String</span><span class="sxs-lookup"><span data-stu-id="4ef7a-109">String</span></span>|<span data-ttu-id="4ef7a-110">カスタムのドメインが使用しているときに、アプリケーションに関連付けられている証明書の詳細です。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="4ef7a-111">既定のドメインを使用する場合は null にします。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="4ef7a-112">externalAuthenticationType</span><span class="sxs-lookup"><span data-stu-id="4ef7a-112">externalAuthenticationType</span></span>|<span data-ttu-id="4ef7a-113">String</span><span class="sxs-lookup"><span data-stu-id="4ef7a-113">String</span></span>|<span data-ttu-id="4ef7a-114">アプリケーションの使用可能な値は、事前認証の設定の詳細: `passthru`、 `aadPreAuthentication`。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="4ef7a-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="4ef7a-115">externalUrl</span></span>|<span data-ttu-id="4ef7a-116">String</span><span class="sxs-lookup"><span data-stu-id="4ef7a-116">String</span></span>|<span data-ttu-id="4ef7a-117">アプリケーションの公開済みの外部 url です。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-117">The published external url for the application.</span></span> <span data-ttu-id="4ef7a-118">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="4ef7a-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="4ef7a-119">internalUrl</span></span>|<span data-ttu-id="4ef7a-120">String</span><span class="sxs-lookup"><span data-stu-id="4ef7a-120">String</span></span>|<span data-ttu-id="4ef7a-121">アプリケーションの内部の url です。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-121">The internal url of the application.</span></span> <span data-ttu-id="4ef7a-122">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-122">For example https://intranet/</span></span> |
|<span data-ttu-id="4ef7a-123">isOnPremPublishingEnabled</span><span class="sxs-lookup"><span data-stu-id="4ef7a-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="4ef7a-124">ブール値</span><span class="sxs-lookup"><span data-stu-id="4ef7a-124">Boolean</span></span>|<span data-ttu-id="4ef7a-125">アプリケーションをか現在発行されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="4ef7a-126">applicationServerTimeout</span><span class="sxs-lookup"><span data-stu-id="4ef7a-126">applicationServerTimeout</span></span>|<span data-ttu-id="4ef7a-127">String</span><span class="sxs-lookup"><span data-stu-id="4ef7a-127">String</span></span>|<span data-ttu-id="4ef7a-128">コネクタが接続を閉じる前に、バックエンド アプリケーションからの応答を待機する期間。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="4ef7a-129">使用可能な値は、`default`、`long` です。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="4ef7a-130">使用`long`場合、サーバーは要求に応答するのには 60 ~ 75 秒以上です。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="4ef7a-131">`long`アプリケーションにアクセスできないし、エラー ・ ステータスは、「バックエンド ・ タイムアウト」です。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="4ef7a-132">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="4ef7a-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="4ef7a-133">ブール値</span><span class="sxs-lookup"><span data-stu-id="4ef7a-133">Boolean</span></span>|<span data-ttu-id="4ef7a-134">アプリケーションが応答ヘッダー内の url を変換する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="4ef7a-135">これには、適切なサイトの cookie の設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4ef7a-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4ef7a-136">JSON representation</span></span>

<span data-ttu-id="4ef7a-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4ef7a-137">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
