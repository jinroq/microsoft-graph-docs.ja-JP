---
title: api リソースの種類
description: Web API アプリケーションの設定を指定します。
localization_priority: Normal
ms.openlocfilehash: 50c21c31fec7434514408e1a214c6edf2b838c98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845208"
---
# <a name="api-resource-type"></a><span data-ttu-id="4582a-103">api リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4582a-103">api resource type</span></span>

> <span data-ttu-id="4582a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4582a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4582a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4582a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4582a-106">Web API アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="4582a-106">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="4582a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4582a-107">Properties</span></span>

| <span data-ttu-id="4582a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4582a-108">Property</span></span> | <span data-ttu-id="4582a-109">種類</span><span class="sxs-lookup"><span data-stu-id="4582a-109">Type</span></span> | <span data-ttu-id="4582a-110">説明</span><span class="sxs-lookup"><span data-stu-id="4582a-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4582a-111">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="4582a-111">requestedAccessTokenVersion</span></span>|<span data-ttu-id="4582a-112">Int32</span><span class="sxs-lookup"><span data-stu-id="4582a-112">Int32</span></span>| <span data-ttu-id="4582a-113">API の現在のリソースに許可されたアクセス トークンのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="4582a-113">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="4582a-114">使用可能な値は、1 または 2 です。</span><span class="sxs-lookup"><span data-stu-id="4582a-114">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="4582a-115">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="4582a-115">oauth2PermissionScopes</span></span>|<span data-ttu-id="4582a-116">[permissionScope](permissionscope.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4582a-116">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="4582a-117">Web アプリケーションの API (リソース) をクライアント アプリケーションに公開する OAuth 2.0 のアクセス許可のスコープのコレクション。</span><span class="sxs-lookup"><span data-stu-id="4582a-117">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="4582a-118">同意の中には、クライアント アプリケーションにこれらのアクセス許可のスコープを付与する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4582a-118">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4582a-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4582a-119">JSON representation</span></span>
<span data-ttu-id="4582a-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4582a-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
