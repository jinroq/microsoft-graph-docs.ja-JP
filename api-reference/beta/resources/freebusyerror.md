---
title: freeBusyError リソースの種類
description: ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたときに発生したエラー情報を表します。
localization_priority: Normal
ms.openlocfilehash: e2c755b51e72adf3ff4efa4de5c9438e70d701e1
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869338"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="01c3f-103">freeBusyError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="01c3f-103">freeBusyError resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
<span data-ttu-id="01c3f-104">ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたときに発生したエラー情報を表します。</span><span class="sxs-lookup"><span data-stu-id="01c3f-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="01c3f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01c3f-105">Properties</span></span>
| <span data-ttu-id="01c3f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01c3f-106">Property</span></span>     | <span data-ttu-id="01c3f-107">型</span><span class="sxs-lookup"><span data-stu-id="01c3f-107">Type</span></span>   |<span data-ttu-id="01c3f-108">説明</span><span class="sxs-lookup"><span data-stu-id="01c3f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01c3f-109">message</span><span class="sxs-lookup"><span data-stu-id="01c3f-109">message</span></span> |<span data-ttu-id="01c3f-110">String</span><span class="sxs-lookup"><span data-stu-id="01c3f-110">String</span></span> |<span data-ttu-id="01c3f-111">エラーについて説明します。</span><span class="sxs-lookup"><span data-stu-id="01c3f-111">Describes the error.</span></span> |
|<span data-ttu-id="01c3f-112">responseCode</span><span class="sxs-lookup"><span data-stu-id="01c3f-112">responseCode</span></span> |<span data-ttu-id="01c3f-113">String</span><span class="sxs-lookup"><span data-stu-id="01c3f-113">String</span></span> |<span data-ttu-id="01c3f-114">ユーザー、配布リスト、またはリソースの可用性を照会するための応答コード。</span><span class="sxs-lookup"><span data-stu-id="01c3f-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="01c3f-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="01c3f-115">JSON representation</span></span>

<span data-ttu-id="01c3f-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="01c3f-116">The following is a JSON representation of the resource.</span></span>

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
