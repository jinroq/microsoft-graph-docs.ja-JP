---
title: publicClient リソースの種類
description: 以外の Web アプリケーションまたは Web Api の設定を指定します。 (モバイルやデスクトップ デバイスで実行されているインストール済みのアプリケーションなどの他のパブリック クライアント)
localization_priority: Normal
ms.openlocfilehash: c466c91f90ac8adc2bf3806fa212e0b01e6d2507
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864198"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="7e429-104">publicClient リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e429-104">publicClient resource type</span></span>

> <span data-ttu-id="7e429-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7e429-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e429-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e429-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7e429-107">以外の Web アプリケーションまたは Web Api の設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e429-107">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="7e429-108">(モバイルやデスクトップ デバイスで実行されているインストール済みのアプリケーションなどの他のパブリック クライアント)</span><span class="sxs-lookup"><span data-stu-id="7e429-108">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="7e429-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e429-109">Properties</span></span>

| <span data-ttu-id="7e429-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e429-110">Property</span></span> | <span data-ttu-id="7e429-111">種類</span><span class="sxs-lookup"><span data-stu-id="7e429-111">Type</span></span> | <span data-ttu-id="7e429-112">説明</span><span class="sxs-lookup"><span data-stu-id="7e429-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7e429-113">redirectUris</span><span class="sxs-lookup"><span data-stu-id="7e429-113">redirectUris</span></span>|<span data-ttu-id="7e429-114">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7e429-114">String collection</span></span>| <span data-ttu-id="7e429-115">ユーザー トークンは、サインイン用に送信される Url または Uri を OAuth 2.0 の認証コードとアクセス トークンに送信のリダイレクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e429-115">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7e429-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e429-116">JSON representation</span></span>
<span data-ttu-id="7e429-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e429-117">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
