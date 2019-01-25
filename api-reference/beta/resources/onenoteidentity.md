---
title: oneNoteIdentity リソースの種類
description: '**準備中のサポート**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f1b03ad907a0b8f6f3cf2674d74f1ee8722357ea
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513943"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="54466-103">oneNoteIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="54466-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54466-104">**準備中のサポート**</span><span class="sxs-lookup"><span data-stu-id="54466-104">**Support coming soon**</span></span>

<span data-ttu-id="54466-105">OneNoteIdentity 型は、_ユーザー_の id を表します。</span><span class="sxs-lookup"><span data-stu-id="54466-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="54466-106">[Id](identity.md)を使用してこの型をマージする将来的には、</span><span class="sxs-lookup"><span data-stu-id="54466-106">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="54466-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="54466-107">JSON representation</span></span>

<span data-ttu-id="54466-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="54466-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteidentity"
}-->

```json
{
  "displayName": "string",
  "id": "string"
}

```
## <a name="properties"></a><span data-ttu-id="54466-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54466-109">Properties</span></span>
| <span data-ttu-id="54466-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54466-110">Property</span></span>     | <span data-ttu-id="54466-111">型</span><span class="sxs-lookup"><span data-stu-id="54466-111">Type</span></span>   |<span data-ttu-id="54466-112">説明</span><span class="sxs-lookup"><span data-stu-id="54466-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54466-113">displayName</span><span class="sxs-lookup"><span data-stu-id="54466-113">displayName</span></span>|<span data-ttu-id="54466-114">string</span><span class="sxs-lookup"><span data-stu-id="54466-114">string</span></span>|<span data-ttu-id="54466-115">Id の表示名です。</span><span class="sxs-lookup"><span data-stu-id="54466-115">The identity's display name.</span></span>|
|<span data-ttu-id="54466-116">id</span><span class="sxs-lookup"><span data-stu-id="54466-116">id</span></span>|<span data-ttu-id="54466-117">文字列</span><span class="sxs-lookup"><span data-stu-id="54466-117">string</span></span>|<span data-ttu-id="54466-118">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="54466-118">Unique identifier for the identity.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oneNoteIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteidentity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
