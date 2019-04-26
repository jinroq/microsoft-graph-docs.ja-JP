---
title: onPremisesPublishing リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568866"
---
# <a name="onpremisespublishing-resource-type"></a><span data-ttu-id="35f50-103">onPremisesPublishing リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35f50-103">onPremisesPublishing resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a><span data-ttu-id="35f50-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35f50-104">Properties</span></span>
| <span data-ttu-id="35f50-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35f50-105">Property</span></span>     | <span data-ttu-id="35f50-106">型</span><span class="sxs-lookup"><span data-stu-id="35f50-106">Type</span></span>   |<span data-ttu-id="35f50-107">説明</span><span class="sxs-lookup"><span data-stu-id="35f50-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35f50-108">customdomaincertificate</span><span class="sxs-lookup"><span data-stu-id="35f50-108">customDomainCertificate</span></span>|<span data-ttu-id="35f50-109">String</span><span class="sxs-lookup"><span data-stu-id="35f50-109">String</span></span>|<span data-ttu-id="35f50-110">カスタムドメインが使用されているときに、アプリケーションに関連付けられている証明書の詳細。</span><span class="sxs-lookup"><span data-stu-id="35f50-110">Details of the certificate associated with the applicaiton when a custom domain is in use.</span></span> <span data-ttu-id="35f50-111">既定のドメインを使用する場合は Null。</span><span class="sxs-lookup"><span data-stu-id="35f50-111">Null when using the default domain.</span></span>|
|<span data-ttu-id="35f50-112">externalauthenticationtype</span><span class="sxs-lookup"><span data-stu-id="35f50-112">externalAuthenticationType</span></span>|<span data-ttu-id="35f50-113">String</span><span class="sxs-lookup"><span data-stu-id="35f50-113">String</span></span>|<span data-ttu-id="35f50-114">詳細アプリケーションの事前認証設定の可能な値は`passthru`、、 `aadPreAuthentication`です。</span><span class="sxs-lookup"><span data-stu-id="35f50-114">Details the pre-authentication setting for the application Possible values are: `passthru`, `aadPreAuthentication`.</span></span>|
|<span data-ttu-id="35f50-115">externalUrl</span><span class="sxs-lookup"><span data-stu-id="35f50-115">externalUrl</span></span>|<span data-ttu-id="35f50-116">String</span><span class="sxs-lookup"><span data-stu-id="35f50-116">String</span></span>|<span data-ttu-id="35f50-117">アプリケーションの公開された外部 url。</span><span class="sxs-lookup"><span data-stu-id="35f50-117">The published external url for the application.</span></span> <span data-ttu-id="35f50-118">例えばhttps://intranet-contoso.msappproxy.net/</span><span class="sxs-lookup"><span data-stu-id="35f50-118">For example https://intranet-contoso.msappproxy.net/</span></span>  |
|<span data-ttu-id="35f50-119">internalUrl</span><span class="sxs-lookup"><span data-stu-id="35f50-119">internalUrl</span></span>|<span data-ttu-id="35f50-120">String</span><span class="sxs-lookup"><span data-stu-id="35f50-120">String</span></span>|<span data-ttu-id="35f50-121">アプリケーションの内部 url。</span><span class="sxs-lookup"><span data-stu-id="35f50-121">The internal url of the application.</span></span> <span data-ttu-id="35f50-122">例えばhttps://intranet/</span><span class="sxs-lookup"><span data-stu-id="35f50-122">For example https://intranet/</span></span> |
|<span data-ttu-id="35f50-123">isonprem発行が有効</span><span class="sxs-lookup"><span data-stu-id="35f50-123">isOnPremPublishingEnabled</span></span>|<span data-ttu-id="35f50-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f50-124">Boolean</span></span>|<span data-ttu-id="35f50-125">アプリケーションが現在公開されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="35f50-125">Indicates if the application is currently being published or not.</span></span>|
|<span data-ttu-id="35f50-126">applicationservertimeout</span><span class="sxs-lookup"><span data-stu-id="35f50-126">applicationServerTimeout</span></span>|<span data-ttu-id="35f50-127">String</span><span class="sxs-lookup"><span data-stu-id="35f50-127">String</span></span>|<span data-ttu-id="35f50-128">この時間が経過すると、コネクタは、接続を閉じる前にバックエンドアプリケーションからの応答を待機します。</span><span class="sxs-lookup"><span data-stu-id="35f50-128">The duration the connector will wait for a response from the backend application before closing the connection.</span></span> <span data-ttu-id="35f50-129">可能な値`default`は`long`、です。</span><span class="sxs-lookup"><span data-stu-id="35f50-129">Possible values are `default`, `long`.</span></span> <span data-ttu-id="35f50-130">サーバー `long`が要求に応答するのに60-75 秒以上かかる場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="35f50-130">Use `long` if your server takes more than 60-75 seconds to respond to requests.</span></span> <span data-ttu-id="35f50-131">また、 `long`アプリケーションにアクセスできず、エラー状態が "バックエンドタイムアウト" になっているかどうかを試してみてください。</span><span class="sxs-lookup"><span data-stu-id="35f50-131">Also try `long` if you are unable to access the application and the error status is "Backend Timeout".</span></span>|
|<span data-ttu-id="35f50-132">isTranslateHostHeaderEnabled</span><span class="sxs-lookup"><span data-stu-id="35f50-132">isTranslateHostHeaderEnabled</span></span>|<span data-ttu-id="35f50-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="35f50-133">Boolean</span></span>|<span data-ttu-id="35f50-134">アプリケーションが応答ヘッダー内の url を変換する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="35f50-134">Indicates if the application should translate urls in the reponse headers.</span></span> <span data-ttu-id="35f50-135">これには、cookie の正しいサイトの設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="35f50-135">This includes setting the correct site for cookies.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35f50-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35f50-136">JSON representation</span></span>

<span data-ttu-id="35f50-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="35f50-137">Here is a JSON representation of the resource.</span></span>

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
