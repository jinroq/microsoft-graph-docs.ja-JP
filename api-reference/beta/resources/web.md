---
title: web リソースの種類
description: Web アプリケーションの設定を指定します。
ms.openlocfilehash: c040de0c323e57f20e04dcf662ea088b1018c144
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072403"
---
# <a name="web-resource-type"></a><span data-ttu-id="8fcf6-103">web リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fcf6-103">web resource type</span></span>

> <span data-ttu-id="8fcf6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8fcf6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8fcf6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fcf6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8fcf6-106">Web アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="8fcf6-106">Specifies settings for a web application.</span></span>

## <a name="properties"></a><span data-ttu-id="8fcf6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fcf6-107">Properties</span></span>

| <span data-ttu-id="8fcf6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fcf6-108">Property</span></span> | <span data-ttu-id="8fcf6-109">型</span><span class="sxs-lookup"><span data-stu-id="8fcf6-109">Type</span></span> | <span data-ttu-id="8fcf6-110">説明</span><span class="sxs-lookup"><span data-stu-id="8fcf6-110">Description</span></span> |
|:---------|:-----|:------------|
|<span data-ttu-id="8fcf6-111">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="8fcf6-111">implicitGrantSettings</span></span>|[<span data-ttu-id="8fcf6-112">implicitGrantSettings</span><span class="sxs-lookup"><span data-stu-id="8fcf6-112">implicitGrantSettings</span></span>](implicitgrantsettings.md)| <span data-ttu-id="8fcf6-113">この web アプリケーションが、OAuth 2.0 の暗黙的なフローを使用してトークンを要求できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8fcf6-113">Specifies whether this web application can request tokens using the OAuth 2.0 implicit flow.</span></span>|
|<span data-ttu-id="8fcf6-114">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="8fcf6-114">logoutUrl</span></span>|<span data-ttu-id="8fcf6-115">String</span><span class="sxs-lookup"><span data-stu-id="8fcf6-115">String</span></span>| <span data-ttu-id="8fcf6-116">[前方チャンネル](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[背面チャネル](https://openid.net/specs/openid-connect-backchannel-1_0.html)または SAML ログアウトのプロトコルを使用してユーザーをログアウトするマイクロソフトの承認のサービスによって使用される URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="8fcf6-116">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="8fcf6-117">oauth2AllowImplicitFlow</span><span class="sxs-lookup"><span data-stu-id="8fcf6-117">oauth2AllowImplicitFlow</span></span>|<span data-ttu-id="8fcf6-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="8fcf6-118">Boolean</span></span>| <span data-ttu-id="8fcf6-119">現在は廃止されています。</span><span class="sxs-lookup"><span data-stu-id="8fcf6-119">Deprecated.</span></span> <span data-ttu-id="8fcf6-120">使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="8fcf6-120">Do not use.</span></span> | 
|<span data-ttu-id="8fcf6-121">redirectUris</span><span class="sxs-lookup"><span data-stu-id="8fcf6-121">redirectUris</span></span>|<span data-ttu-id="8fcf6-122">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8fcf6-122">String collection</span></span>| <span data-ttu-id="8fcf6-123">ユーザー トークンは、サインイン用に送信される Url または Uri を OAuth 2.0 の認証コードとアクセス トークンに送信のリダイレクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="8fcf6-123">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8fcf6-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fcf6-124">JSON representation</span></span>
<span data-ttu-id="8fcf6-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8fcf6-125">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
