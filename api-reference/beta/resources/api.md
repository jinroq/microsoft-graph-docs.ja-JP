---
title: api リソースの種類
description: Web API アプリケーションの設定を指定します。
ms.openlocfilehash: b5b07ccb5a66027f9eb755754842f6e2e2ae708e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068798"
---
# <a name="api-resource-type"></a><span data-ttu-id="0c434-103">api リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c434-103">api resource type</span></span>

> <span data-ttu-id="0c434-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c434-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c434-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c434-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0c434-106">Web API アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c434-106">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="0c434-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c434-107">Properties</span></span>

| <span data-ttu-id="0c434-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c434-108">Property</span></span> | <span data-ttu-id="0c434-109">型</span><span class="sxs-lookup"><span data-stu-id="0c434-109">Type</span></span> | <span data-ttu-id="0c434-110">説明</span><span class="sxs-lookup"><span data-stu-id="0c434-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0c434-111">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="0c434-111">requestedAccessTokenVersion</span></span>|<span data-ttu-id="0c434-112">Int32</span><span class="sxs-lookup"><span data-stu-id="0c434-112">Int32</span></span>| <span data-ttu-id="0c434-113">API の現在のリソースに許可されたアクセス トークンのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="0c434-113">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="0c434-114">使用可能な値は、1 または 2 です。</span><span class="sxs-lookup"><span data-stu-id="0c434-114">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="0c434-115">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="0c434-115">oauth2PermissionScopes</span></span>|<span data-ttu-id="0c434-116">[permissionScope](permissionscope.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0c434-116">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="0c434-117">Web アプリケーションの API (リソース) をクライアント アプリケーションに公開する OAuth 2.0 のアクセス許可のスコープのコレクション。</span><span class="sxs-lookup"><span data-stu-id="0c434-117">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="0c434-118">同意の中には、クライアント アプリケーションにこれらのアクセス許可のスコープを付与する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0c434-118">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0c434-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c434-119">JSON representation</span></span>
<span data-ttu-id="0c434-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c434-120">Here is a JSON representation of the resource.</span></span>

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