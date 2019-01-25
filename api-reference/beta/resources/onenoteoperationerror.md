---
title: onenoteOperationError リソースの種類
description: 失敗した OneNote 操作によるエラー。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 78e0ab763f27d17cf926795459b4e4a25cdf8e71
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522057"
---
# <a name="onenoteoperationerror-resource-type"></a><span data-ttu-id="18f6e-103">onenoteOperationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="18f6e-103">onenoteOperationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18f6e-104">失敗した OneNote 操作によるエラー。</span><span class="sxs-lookup"><span data-stu-id="18f6e-104">An error from a failed OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="18f6e-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="18f6e-105">JSON representation</span></span>

<span data-ttu-id="18f6e-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="18f6e-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteOperationError"
}-->

```json
{
  "code": "string",
  "message": "string"
}

```
## <a name="properties"></a><span data-ttu-id="18f6e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18f6e-107">Properties</span></span>
| <span data-ttu-id="18f6e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="18f6e-108">Property</span></span>     | <span data-ttu-id="18f6e-109">型</span><span class="sxs-lookup"><span data-stu-id="18f6e-109">Type</span></span>   |<span data-ttu-id="18f6e-110">説明</span><span class="sxs-lookup"><span data-stu-id="18f6e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18f6e-111">code</span><span class="sxs-lookup"><span data-stu-id="18f6e-111">code</span></span>|<span data-ttu-id="18f6e-112">文字列</span><span class="sxs-lookup"><span data-stu-id="18f6e-112">string</span></span>|<span data-ttu-id="18f6e-113">エラー コード。</span><span class="sxs-lookup"><span data-stu-id="18f6e-113">The error code.</span></span>|
|<span data-ttu-id="18f6e-114">message</span><span class="sxs-lookup"><span data-stu-id="18f6e-114">message</span></span>|<span data-ttu-id="18f6e-115">string</span><span class="sxs-lookup"><span data-stu-id="18f6e-115">string</span></span>|<span data-ttu-id="18f6e-116">エラー メッセージ。</span><span class="sxs-lookup"><span data-stu-id="18f6e-116">The error message.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenoteOperationError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenoteoperationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
