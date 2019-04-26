---
title: resourceaccess リソースの種類
description: アプリケーションに必要な OAuth 2.0 アクセス許可スコープまたはアプリの役割を指定します。 requiredresourceaccess 型の**resourceaccess**プロパティは、 **resourceaccess**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: bb77a12a207e274b27263029d96f4ef260cfe5cb
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343634"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="c9153-104">resourceaccess リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9153-104">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9153-105">アプリケーションに必要な OAuth 2.0 アクセス許可スコープまたはアプリの役割を指定します。</span><span class="sxs-lookup"><span data-stu-id="c9153-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="c9153-106">[requiredresourceaccess](requiredresourceaccess.md)型の**resourceaccess**プロパティは、 **resourceaccess**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c9153-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c9153-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9153-107">JSON representation</span></span>

<span data-ttu-id="c9153-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c9153-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="c9153-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9153-109">Properties</span></span>
| <span data-ttu-id="c9153-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9153-110">Property</span></span>     | <span data-ttu-id="c9153-111">型</span><span class="sxs-lookup"><span data-stu-id="c9153-111">Type</span></span>   |<span data-ttu-id="c9153-112">説明</span><span class="sxs-lookup"><span data-stu-id="c9153-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9153-113">id</span><span class="sxs-lookup"><span data-stu-id="c9153-113">id</span></span>|<span data-ttu-id="c9153-114">Guid</span><span class="sxs-lookup"><span data-stu-id="c9153-114">Guid</span></span>|<span data-ttu-id="c9153-115">リソースアプリケーションが公開する[oAuth2Permission](oauth2permission.md)または[approle](approle.md)インスタンスの1つの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c9153-115">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="c9153-116">type</span><span class="sxs-lookup"><span data-stu-id="c9153-116">type</span></span>|<span data-ttu-id="c9153-117">String</span><span class="sxs-lookup"><span data-stu-id="c9153-117">String</span></span>|<span data-ttu-id="c9153-118">**id**プロパティが[oAuth2Permission](oauth2permission.md)または[approle](approle.md)のどちらを参照するかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c9153-118">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="c9153-119">可能な値は、"scope" または "role" です。</span><span class="sxs-lookup"><span data-stu-id="c9153-119">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
