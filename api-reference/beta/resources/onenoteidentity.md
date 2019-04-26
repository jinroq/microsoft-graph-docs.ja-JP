---
title: oneNoteIdentity リソースの種類
description: '**まもなくサポートが提供される**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: ee5eb0db40516e1069fe8e40a8711cf97ae18eaa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341499"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="5e671-103">oneNoteIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5e671-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e671-104">**まもなくサポートが提供される**</span><span class="sxs-lookup"><span data-stu-id="5e671-104">**Support coming soon**</span></span>

<span data-ttu-id="5e671-105">OneNoteIdentity 型は、_ユーザー_の id を表します。</span><span class="sxs-lookup"><span data-stu-id="5e671-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="5e671-106">今後、この型は[identity](identity.md)とマージされます。</span><span class="sxs-lookup"><span data-stu-id="5e671-106">In future, this type will be merged with [identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="5e671-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5e671-107">JSON representation</span></span>

<span data-ttu-id="5e671-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5e671-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="5e671-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e671-109">Properties</span></span>
| <span data-ttu-id="5e671-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e671-110">Property</span></span>     | <span data-ttu-id="5e671-111">型</span><span class="sxs-lookup"><span data-stu-id="5e671-111">Type</span></span>   |<span data-ttu-id="5e671-112">説明</span><span class="sxs-lookup"><span data-stu-id="5e671-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e671-113">displayName</span><span class="sxs-lookup"><span data-stu-id="5e671-113">displayName</span></span>|<span data-ttu-id="5e671-114">string</span><span class="sxs-lookup"><span data-stu-id="5e671-114">string</span></span>|<span data-ttu-id="5e671-115">id の表示名。</span><span class="sxs-lookup"><span data-stu-id="5e671-115">The identity's display name.</span></span>|
|<span data-ttu-id="5e671-116">id</span><span class="sxs-lookup"><span data-stu-id="5e671-116">id</span></span>|<span data-ttu-id="5e671-117">string</span><span class="sxs-lookup"><span data-stu-id="5e671-117">string</span></span>|<span data-ttu-id="5e671-118">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5e671-118">Unique identifier for the identity.</span></span>|

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
