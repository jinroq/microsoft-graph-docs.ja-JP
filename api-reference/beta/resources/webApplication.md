---
title: webApplication リソースの種類
description: Web アプリケーションの設定を指定します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e57744c3825a669a9008cd05d649be0ec51b71ac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964152"
---
# <a name="webapplication-resource-type"></a><span data-ttu-id="78dde-103">webApplication リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78dde-103">webApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78dde-104">Web アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="78dde-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="78dde-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78dde-105">Properties</span></span>

| <span data-ttu-id="78dde-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78dde-106">Property</span></span> | <span data-ttu-id="78dde-107">型</span><span class="sxs-lookup"><span data-stu-id="78dde-107">Type</span></span> | <span data-ttu-id="78dde-108">説明</span><span class="sxs-lookup"><span data-stu-id="78dde-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="78dde-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="78dde-109">implicitGrantSettings</span></span>|[<span data-ttu-id="78dde-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="78dde-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="78dde-111">この web アプリケーションが OAuth 2.0 暗黙的フローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="78dde-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="78dde-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="78dde-112">logoutUrl</span></span>|<span data-ttu-id="78dde-113">String</span><span class="sxs-lookup"><span data-stu-id="78dde-113">String</span></span>| <span data-ttu-id="78dde-114">Microsoft の承認サービスで、[フロント チャネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[バック チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウト プロトコルを使ってユーザーのログアウトするのに使う URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="78dde-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="78dde-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="78dde-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="78dde-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="78dde-116">Boolean</span></span>| <span data-ttu-id="78dde-117">現在は廃止されています。</span><span class="sxs-lookup"><span data-stu-id="78dde-117">Deprecated.</span></span> <span data-ttu-id="78dde-118">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="78dde-118">Do not use.</span></span> | 
|<span data-ttu-id="78dde-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="78dde-119">redirectUris</span></span>|<span data-ttu-id="78dde-120">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="78dde-120">String collection</span></span>| <span data-ttu-id="78dde-121">サインインのためにユーザートークンが送信される Url、または OAuth 2.0 認証コードとアクセストークンがに送信されるリダイレクト Uri を指定します。</span><span class="sxs-lookup"><span data-stu-id="78dde-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="78dde-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78dde-122">JSON representation</span></span>
<span data-ttu-id="78dde-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78dde-123">Here is a JSON representation of the resource.</span></span>

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
