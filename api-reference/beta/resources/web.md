---
title: web リソースの種類
description: Web アプリケーションの設定を指定します。
localization_priority: Normal
ms.openlocfilehash: 7e03977481f0c021b7d67ec44fd4db275642cdf8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527669"
---
# <a name="web-resource-type"></a><span data-ttu-id="aad2d-103">web リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aad2d-103">web resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aad2d-104">Web アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="aad2d-104">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="aad2d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aad2d-105">Properties</span></span>

| <span data-ttu-id="aad2d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aad2d-106">Property</span></span> | <span data-ttu-id="aad2d-107">型</span><span class="sxs-lookup"><span data-stu-id="aad2d-107">Type</span></span> | <span data-ttu-id="aad2d-108">説明</span><span class="sxs-lookup"><span data-stu-id="aad2d-108">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="aad2d-109">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="aad2d-109">implicitGrantSettings</span></span>|[<span data-ttu-id="aad2d-110">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="aad2d-110">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="aad2d-111">この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="aad2d-111">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="aad2d-112">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="aad2d-112">logoutUrl</span></span>|<span data-ttu-id="aad2d-113">String</span><span class="sxs-lookup"><span data-stu-id="aad2d-113">String</span></span>| <span data-ttu-id="aad2d-114">[前方チャンネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[背面チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウトのプロトコルを使用してユーザーをログアウトするマイクロソフトの承認のサービスによって使用される URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="aad2d-114">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="aad2d-115">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="aad2d-115">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="aad2d-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="aad2d-116">Boolean</span></span>| <span data-ttu-id="aad2d-117">現在は廃止されています。</span><span class="sxs-lookup"><span data-stu-id="aad2d-117">Deprecated.</span></span> <span data-ttu-id="aad2d-118">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="aad2d-118">Do not use.</span></span> | 
|<span data-ttu-id="aad2d-119">redirectUris</span><span class="sxs-lookup"><span data-stu-id="aad2d-119">redirectUris</span></span>|<span data-ttu-id="aad2d-120">String コレクション</span><span class="sxs-lookup"><span data-stu-id="aad2d-120">String collection</span></span>| <span data-ttu-id="aad2d-121">ユーザー トークンは、サインイン用に送信される Url または Uri を OAuth 2.0 の認証コードとアクセス トークンに送信のリダイレクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="aad2d-121">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aad2d-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aad2d-122">JSON representation</span></span>
<span data-ttu-id="aad2d-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aad2d-123">Here is a JSON representation of the resource.</span></span>

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
