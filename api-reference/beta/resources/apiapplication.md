---
title: api リソースの種類
description: Web API アプリケーションの設定を指定します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3bf5ffc21c13e0952efd0f5ea773f76dc3f7b46f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974340"
---
# <a name="api-resource-type"></a><span data-ttu-id="e661e-103">api リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e661e-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e661e-104">Web API アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="e661e-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="e661e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e661e-105">Properties</span></span>

| <span data-ttu-id="e661e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e661e-106">Property</span></span> | <span data-ttu-id="e661e-107">型</span><span class="sxs-lookup"><span data-stu-id="e661e-107">Type</span></span> | <span data-ttu-id="e661e-108">説明</span><span class="sxs-lookup"><span data-stu-id="e661e-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e661e-109">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="e661e-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="e661e-110">Int32</span><span class="sxs-lookup"><span data-stu-id="e661e-110">Int32</span></span>| <span data-ttu-id="e661e-111">現在の API リソースに対して承認されたアクセストークンのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="e661e-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="e661e-112">可能な値は1または2です。</span><span class="sxs-lookup"><span data-stu-id="e661e-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="e661e-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="e661e-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="e661e-114">[Permissionscope](permissionscope.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e661e-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="e661e-115">Web API (リソース) アプリケーションがクライアントアプリケーションに公開する OAuth 2.0 アクセス許可スコープのコレクション。</span><span class="sxs-lookup"><span data-stu-id="e661e-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="e661e-116">これらのアクセス許可スコープは、同意時にクライアントアプリケーションに付与されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e661e-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e661e-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e661e-117">JSON representation</span></span>
<span data-ttu-id="e661e-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e661e-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.apiApplication"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
