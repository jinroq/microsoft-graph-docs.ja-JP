---
title: operationError リソースの種類
description: TeamsAsyncOperation で発生したエラーをについて説明します。
localization_priority: Normal
ms.openlocfilehash: 1f07fe064d7bbd255f2693071c86842a34fdffa0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526131"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="8c3d5-103">operationError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c3d5-103">operationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c3d5-104">[TeamsAsyncOperation](teamsasyncoperation.md)で発生したエラーをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8c3d5-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="8c3d5-105">operationError プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c3d5-105">operationError Properties</span></span>
| <span data-ttu-id="8c3d5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c3d5-106">Property</span></span>     | <span data-ttu-id="8c3d5-107">型</span><span class="sxs-lookup"><span data-stu-id="8c3d5-107">Type</span></span>   |<span data-ttu-id="8c3d5-108">説明</span><span class="sxs-lookup"><span data-stu-id="8c3d5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c3d5-109">code</span><span class="sxs-lookup"><span data-stu-id="8c3d5-109">code</span></span>|<span data-ttu-id="8c3d5-110">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="8c3d5-110">string (readonly)</span></span>|<span data-ttu-id="8c3d5-111">操作のエラー コードです。</span><span class="sxs-lookup"><span data-stu-id="8c3d5-111">Operation error code.</span></span>|
|<span data-ttu-id="8c3d5-112">message</span><span class="sxs-lookup"><span data-stu-id="8c3d5-112">message</span></span>|<span data-ttu-id="8c3d5-113">文字列 (読み取り専用)</span><span class="sxs-lookup"><span data-stu-id="8c3d5-113">string (readonly)</span></span>|<span data-ttu-id="8c3d5-114">エラー メッセージを操作します。</span><span class="sxs-lookup"><span data-stu-id="8c3d5-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c3d5-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c3d5-115">JSON representation</span></span>

<span data-ttu-id="8c3d5-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8c3d5-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/operationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
