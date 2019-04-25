---
title: 診断リソースの種類
description: OneNote の操作に関するエラーまたは警告に関する情報。
localization_priority: Normal
ms.openlocfilehash: ef495374f84e0df887198b38a5c8488987a59343
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535215"
---
# <a name="diagnostic-resource-type"></a><span data-ttu-id="a2f59-103">診断リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2f59-103">diagnostic resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2f59-104">OneNote の操作に関するエラーまたは警告に関する情報。</span><span class="sxs-lookup"><span data-stu-id="a2f59-104">Information about an error or warning for a OneNote operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2f59-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2f59-105">JSON representation</span></span>

<span data-ttu-id="a2f59-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a2f59-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.diagnostic"
}-->

```json
{
  "message": "string",
  "url": "string"
}

```
## <a name="properties"></a><span data-ttu-id="a2f59-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2f59-107">Properties</span></span>
| <span data-ttu-id="a2f59-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2f59-108">Property</span></span>     | <span data-ttu-id="a2f59-109">型</span><span class="sxs-lookup"><span data-stu-id="a2f59-109">Type</span></span>   |<span data-ttu-id="a2f59-110">説明</span><span class="sxs-lookup"><span data-stu-id="a2f59-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2f59-111">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="a2f59-111">message</span></span>|<span data-ttu-id="a2f59-112">String</span><span class="sxs-lookup"><span data-stu-id="a2f59-112">String</span></span>|<span data-ttu-id="a2f59-113">エラーまたは警告を発生させた条件を説明するメッセージ。</span><span class="sxs-lookup"><span data-stu-id="a2f59-113">The message describing the condition that triggered the error or warning.</span></span>|
|<span data-ttu-id="a2f59-114">url</span><span class="sxs-lookup"><span data-stu-id="a2f59-114">url</span></span>|<span data-ttu-id="a2f59-115">String</span><span class="sxs-lookup"><span data-stu-id="a2f59-115">String</span></span>|<span data-ttu-id="a2f59-116">この問題に関するドキュメントへのリンク。</span><span class="sxs-lookup"><span data-stu-id="a2f59-116">The link to the documentation for this issue.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "diagnostic resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/diagnostic.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
