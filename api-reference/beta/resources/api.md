---
title: api リソースの種類
description: Web API アプリケーションの設定を指定します。
localization_priority: Normal
ms.openlocfilehash: 9d9259911464feb545b97a9eb8585723a9c3e20e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535692"
---
# <a name="api-resource-type"></a><span data-ttu-id="54347-103">api リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54347-103">api resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54347-104">Web API アプリケーションの設定を指定します。</span><span class="sxs-lookup"><span data-stu-id="54347-104">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="54347-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54347-105">Properties</span></span>

| <span data-ttu-id="54347-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54347-106">Property</span></span> | <span data-ttu-id="54347-107">型</span><span class="sxs-lookup"><span data-stu-id="54347-107">Type</span></span> | <span data-ttu-id="54347-108">説明</span><span class="sxs-lookup"><span data-stu-id="54347-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="54347-109">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="54347-109">requestedAccessTokenVersion</span></span>|<span data-ttu-id="54347-110">Int32</span><span class="sxs-lookup"><span data-stu-id="54347-110">Int32</span></span>| <span data-ttu-id="54347-111">現在の API リソースに対して承認されたアクセストークンのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="54347-111">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="54347-112">可能な値は1または2です。</span><span class="sxs-lookup"><span data-stu-id="54347-112">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="54347-113">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="54347-113">oauth2PermissionScopes</span></span>|<span data-ttu-id="54347-114">[permissionscope](permissionscope.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="54347-114">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="54347-115">web API (リソース) アプリケーションがクライアントアプリケーションに公開する OAuth 2.0 アクセス許可スコープのコレクション。</span><span class="sxs-lookup"><span data-stu-id="54347-115">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="54347-116">これらのアクセス許可スコープは、同意時にクライアントアプリケーションに付与されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54347-116">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="54347-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54347-117">JSON representation</span></span>
<span data-ttu-id="54347-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54347-118">Here is a JSON representation of the resource.</span></span>

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
