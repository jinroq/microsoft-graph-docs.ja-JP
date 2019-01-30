---
title: web リソースの種類
description: Web アプリケーションの設定を指定します。
localization_priority: Normal
ms.openlocfilehash: 7e03977481f0c021b7d67ec44fd4db275642cdf8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643511"
---
# <a name="web-resource-type"></a><span data-ttu-id="e6892-103">web リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6892-103">web resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6892-104">Web アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6892-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="e6892-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6892-105">Properties</span></span>

| <span data-ttu-id="e6892-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e6892-106">Property</span></span> | <span data-ttu-id="e6892-107">型</span><span class="sxs-lookup"><span data-stu-id="e6892-107">Type</span></span> | <span data-ttu-id="e6892-108">説明</span><span class="sxs-lookup"><span data-stu-id="e6892-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="e6892-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="e6892-109">implicitGrantSettings</span></span>|[<span data-ttu-id="e6892-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="e6892-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="e6892-111">この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e6892-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="e6892-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="e6892-112">logoutUrl</span></span>|<span data-ttu-id="e6892-113">String</span><span class="sxs-lookup"><span data-stu-id="e6892-113">String</span></span>| <span data-ttu-id="e6892-114">Microsoft の承認サービスで、[フロント チャネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[バック チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウト プロトコルを使ってユーザーのログアウトするのに使う URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="e6892-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="e6892-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="e6892-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="e6892-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6892-116">Boolean</span></span>| <span data-ttu-id="e6892-117">現在は廃止されています。</span><span class="sxs-lookup"><span data-stu-id="e6892-117">Deprecated.</span></span> <span data-ttu-id="e6892-118">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="e6892-118">Do not use.</span></span> | 
|<span data-ttu-id="e6892-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="e6892-119">redirectUris</span></span>|<span data-ttu-id="e6892-120">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e6892-120">String collection</span></span>| <span data-ttu-id="e6892-121">ユーザー トークンは、サインイン用に送信される Url または Uri を OAuth 2.0 の認証コードとアクセス トークンに送信のリダイレクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e6892-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e6892-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6892-122">JSON representation</span></span>
<span data-ttu-id="e6892-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e6892-123">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.web"
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
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/web.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
