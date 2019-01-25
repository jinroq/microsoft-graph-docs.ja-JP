---
title: freeBusyError リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: f1ff7717034798830a610b35dbbff5c987cf7371
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529846"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="dedfa-104">freeBusyError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dedfa-104">freeBusyError resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="dedfa-105">ユーザー、配布リスト、またはリソースの可用性を取得しようとしていますからエラー情報を表します。</span><span class="sxs-lookup"><span data-stu-id="dedfa-105">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="dedfa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dedfa-106">Properties</span></span>
| <span data-ttu-id="dedfa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dedfa-107">Property</span></span>     | <span data-ttu-id="dedfa-108">型</span><span class="sxs-lookup"><span data-stu-id="dedfa-108">Type</span></span>   |<span data-ttu-id="dedfa-109">説明</span><span class="sxs-lookup"><span data-stu-id="dedfa-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dedfa-110">message</span><span class="sxs-lookup"><span data-stu-id="dedfa-110">message</span></span> |<span data-ttu-id="dedfa-111">String</span><span class="sxs-lookup"><span data-stu-id="dedfa-111">String</span></span> |<span data-ttu-id="dedfa-112">エラーをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="dedfa-112">Describes the error.</span></span> |
|<span data-ttu-id="dedfa-113">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dedfa-113">responseCode</span></span> |<span data-ttu-id="dedfa-114">String</span><span class="sxs-lookup"><span data-stu-id="dedfa-114">String</span></span> |<span data-ttu-id="dedfa-115">ユーザー、配布リスト、またはリソースの可用性のクエリからの応答コード。</span><span class="sxs-lookup"><span data-stu-id="dedfa-115">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="dedfa-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dedfa-116">JSON representation</span></span>

<span data-ttu-id="dedfa-117">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dedfa-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/freebusyerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
