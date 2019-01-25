---
title: api リソースの種類
description: Web API アプリケーションの設定を指定します。
localization_priority: Normal
ms.openlocfilehash: 9d9259911464feb545b97a9eb8585723a9c3e20e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521447"
---
# <a name="api-resource-type"></a><span data-ttu-id="70bba-103">api リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70bba-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70bba-104">Web API アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="70bba-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="70bba-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70bba-105">Properties</span></span>

| <span data-ttu-id="70bba-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70bba-106">Property</span></span> | <span data-ttu-id="70bba-107">型</span><span class="sxs-lookup"><span data-stu-id="70bba-107">Type</span></span> | <span data-ttu-id="70bba-108">説明</span><span class="sxs-lookup"><span data-stu-id="70bba-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="70bba-109">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="70bba-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="70bba-110">Int32</span><span class="sxs-lookup"><span data-stu-id="70bba-110">Int32</span></span>| <span data-ttu-id="70bba-111">API の現在のリソースに許可されたアクセス トークンのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="70bba-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="70bba-112">使用可能な値は、1 または 2 です。</span><span class="sxs-lookup"><span data-stu-id="70bba-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="70bba-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="70bba-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="70bba-114">[permissionScope](permissionscope.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="70bba-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="70bba-115">Web アプリケーションの API (リソース) をクライアント アプリケーションに公開する OAuth 2.0 のアクセス許可のスコープのコレクション。</span><span class="sxs-lookup"><span data-stu-id="70bba-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="70bba-116">同意の中には、クライアント アプリケーションにこれらのアクセス許可のスコープを付与する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="70bba-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="70bba-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70bba-117">JSON representation</span></span>
<span data-ttu-id="70bba-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="70bba-118">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/api.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
