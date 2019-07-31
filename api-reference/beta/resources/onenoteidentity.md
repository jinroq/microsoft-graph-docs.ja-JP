---
title: oneNoteIdentity リソースの種類
description: '**まもなくサポートが提供される**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 0a7df80dd3dcd4f4b93edb4e708e65de3f74d775
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966448"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="5ca71-103">oneNoteIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5ca71-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ca71-104">**まもなくサポートが提供される**</span><span class="sxs-lookup"><span data-stu-id="5ca71-104">**Support coming soon**</span></span>

<span data-ttu-id="5ca71-105">OneNoteIdentity 型は、_ユーザー_の id を表します。</span><span class="sxs-lookup"><span data-stu-id="5ca71-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="5ca71-106">今後、この型は[identity](identity.md)とマージされます。</span><span class="sxs-lookup"><span data-stu-id="5ca71-106">In future, this type will be merged with [identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="5ca71-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5ca71-107">JSON representation</span></span>

<span data-ttu-id="5ca71-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5ca71-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteIdentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="5ca71-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ca71-109">Properties</span></span>
| <span data-ttu-id="5ca71-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ca71-110">Property</span></span>     | <span data-ttu-id="5ca71-111">型</span><span class="sxs-lookup"><span data-stu-id="5ca71-111">Type</span></span>   |<span data-ttu-id="5ca71-112">説明</span><span class="sxs-lookup"><span data-stu-id="5ca71-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ca71-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5ca71-113">displayName</span></span>|<span data-ttu-id="5ca71-114">string</span><span class="sxs-lookup"><span data-stu-id="5ca71-114">string</span></span>|<span data-ttu-id="5ca71-115">Id の表示名。</span><span class="sxs-lookup"><span data-stu-id="5ca71-115">The identity's display name.</span></span>|
|<span data-ttu-id="5ca71-116">id</span><span class="sxs-lookup"><span data-stu-id="5ca71-116">id</span></span>|<span data-ttu-id="5ca71-117">string</span><span class="sxs-lookup"><span data-stu-id="5ca71-117">string</span></span>|<span data-ttu-id="5ca71-118">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5ca71-118">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
