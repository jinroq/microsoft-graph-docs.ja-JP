---
title: webApplication リソースの種類
description: Web アプリケーションの設定を指定します。
localization_priority: Normal
ms.openlocfilehash: cdb210d5193167138ecec216b1e4084554f05c78
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348415"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="594a7-103">webApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="594a7-103">webApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="594a7-104">Web アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="594a7-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="594a7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="594a7-105">Properties</span></span>

| <span data-ttu-id="594a7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="594a7-106">Property</span></span> | <span data-ttu-id="594a7-107">型</span><span class="sxs-lookup"><span data-stu-id="594a7-107">Type</span></span> | <span data-ttu-id="594a7-108">説明</span><span class="sxs-lookup"><span data-stu-id="594a7-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="594a7-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="594a7-109">implicitGrantSettings</span></span>|[<span data-ttu-id="594a7-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="594a7-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="594a7-111">この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="594a7-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="594a7-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="594a7-112">logoutUrl</span></span>|<span data-ttu-id="594a7-113">String</span><span class="sxs-lookup"><span data-stu-id="594a7-113">String</span></span>| <span data-ttu-id="594a7-114">Microsoft の承認サービスで、[フロント チャネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[バック チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウト プロトコルを使ってユーザーのログアウトするのに使う URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="594a7-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="594a7-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="594a7-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="594a7-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="594a7-116">Boolean</span></span>| <span data-ttu-id="594a7-117">現在は廃止されています。</span><span class="sxs-lookup"><span data-stu-id="594a7-117">Deprecated.</span></span> <span data-ttu-id="594a7-118">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="594a7-118">Do not use.</span></span> | 
|<span data-ttu-id="594a7-119">redirecturis</span><span class="sxs-lookup"><span data-stu-id="594a7-119">redirectUris</span></span>|<span data-ttu-id="594a7-120">String collection</span><span class="sxs-lookup"><span data-stu-id="594a7-120">String collection</span></span>| <span data-ttu-id="594a7-121">サインインのためにユーザートークンが送信される url、または OAuth 2.0 認証コードとアクセストークンがに送信されるリダイレクト uri を指定します。</span><span class="sxs-lookup"><span data-stu-id="594a7-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="594a7-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="594a7-122">JSON representation</span></span>
<span data-ttu-id="594a7-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="594a7-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
}-->

```json
{
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "oauth2AllowImplicitFlow": false,
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
