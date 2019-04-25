---
title: oneNoteIdentity リソースの種類
description: '**まもなくサポートが提供される**'
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: f1b03ad907a0b8f6f3cf2674d74f1ee8722357ea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525027"
---
# <a name="onenoteidentity-resource-type"></a><span data-ttu-id="ed889-103">oneNoteIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ed889-103">oneNoteIdentity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed889-104">**まもなくサポートが提供される**</span><span class="sxs-lookup"><span data-stu-id="ed889-104">**Support coming soon**</span></span>

<span data-ttu-id="ed889-105">OneNoteIdentity 型は、_ユーザー_の id を表します。</span><span class="sxs-lookup"><span data-stu-id="ed889-105">The OneNoteIdentity type represents an identity of a _user_.</span></span>

<span data-ttu-id="ed889-106">今後、この型は[Identity](identity.md)とマージされます。</span><span class="sxs-lookup"><span data-stu-id="ed889-106">In future, this type will be merged with [Identity](identity.md)</span></span>


## <a name="json-representation"></a><span data-ttu-id="ed889-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ed889-107">JSON representation</span></span>

<span data-ttu-id="ed889-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ed889-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ed889-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed889-109">Properties</span></span>
| <span data-ttu-id="ed889-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed889-110">Property</span></span>     | <span data-ttu-id="ed889-111">型</span><span class="sxs-lookup"><span data-stu-id="ed889-111">Type</span></span>   |<span data-ttu-id="ed889-112">説明</span><span class="sxs-lookup"><span data-stu-id="ed889-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ed889-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ed889-113">displayName</span></span>|<span data-ttu-id="ed889-114">string</span><span class="sxs-lookup"><span data-stu-id="ed889-114">string</span></span>|<span data-ttu-id="ed889-115">id の表示名。</span><span class="sxs-lookup"><span data-stu-id="ed889-115">The identity's display name.</span></span>|
|<span data-ttu-id="ed889-116">id</span><span class="sxs-lookup"><span data-stu-id="ed889-116">id</span></span>|<span data-ttu-id="ed889-117">string</span><span class="sxs-lookup"><span data-stu-id="ed889-117">string</span></span>|<span data-ttu-id="ed889-118">ID の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ed889-118">Unique identifier for the identity.</span></span>|

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
