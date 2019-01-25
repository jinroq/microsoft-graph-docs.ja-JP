---
title: resourceAccess リソースの種類
description: OAuth 2.0 のためのアクセス許可のスコープまたはアプリケーションを必要とするアプリケーションの役割を指定します。 RequiredResourceAccess 型の**resourceAccess**プロパティは、 **ResourceAccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519025"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="01968-104">resourceAccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="01968-104">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01968-105">OAuth 2.0 のためのアクセス許可のスコープまたはアプリケーションを必要とするアプリケーションの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="01968-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="01968-106">[RequiredResourceAccess](requiredresourceaccess.md)型の**resourceAccess**プロパティは、 **ResourceAccess**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="01968-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="01968-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="01968-107">JSON representation</span></span>

<span data-ttu-id="01968-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="01968-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="01968-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01968-109">Properties</span></span>
| <span data-ttu-id="01968-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01968-110">Property</span></span>     | <span data-ttu-id="01968-111">型</span><span class="sxs-lookup"><span data-stu-id="01968-111">Type</span></span>   |<span data-ttu-id="01968-112">説明</span><span class="sxs-lookup"><span data-stu-id="01968-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01968-113">ID</span><span class="sxs-lookup"><span data-stu-id="01968-113">id</span></span>|<span data-ttu-id="01968-114">Guid</span><span class="sxs-lookup"><span data-stu-id="01968-114">Guid</span></span>|<span data-ttu-id="01968-115">リソースのアプリケーションを公開する[oAuth2Permission](oauth2permission.md)または[エンティティ](approle.md)のインスタンスの 1 つの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="01968-115">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="01968-116">type</span><span class="sxs-lookup"><span data-stu-id="01968-116">type</span></span>|<span data-ttu-id="01968-117">String</span><span class="sxs-lookup"><span data-stu-id="01968-117">String</span></span>|<span data-ttu-id="01968-118">[OAuth2Permission](oauth2permission.md)または[エンティティ](approle.md)の**id**プロパティを参照するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="01968-118">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="01968-119">使用可能な値は、「スコープ」または「ロール」です。</span><span class="sxs-lookup"><span data-stu-id="01968-119">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
