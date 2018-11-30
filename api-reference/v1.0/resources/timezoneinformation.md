---
title: timeZoneInformation リソースの種類
description: タイム ゾーンを表します。 サポートされている形式は、Windows、およびインターネット割り当て番号機関 (IANA) はタイム ゾーン (Olson タイム ・ ゾーンとも呼ばれます)
ms.openlocfilehash: de80ed293af834d299be5f9543c5c3bedde7a540
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020302"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="96835-104">timeZoneInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96835-104">timeZoneInformation resource type</span></span>


<span data-ttu-id="96835-105">タイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="96835-105">Represents a time zone.</span></span> <span data-ttu-id="96835-106">サポートされる形式は、Windows 形式です。現在既知の問題が解決されている場合は、[Internet Assigned Numbers Authority (IANA) タイム ゾーン](https://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式もサポートされます。</span><span class="sxs-lookup"><span data-stu-id="96835-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="96835-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96835-107">Properties</span></span>
| <span data-ttu-id="96835-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96835-108">Property</span></span>     | <span data-ttu-id="96835-109">型</span><span class="sxs-lookup"><span data-stu-id="96835-109">Type</span></span>   |<span data-ttu-id="96835-110">説明</span><span class="sxs-lookup"><span data-stu-id="96835-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96835-111">alias</span><span class="sxs-lookup"><span data-stu-id="96835-111">alias</span></span>|<span data-ttu-id="96835-112">文字列</span><span class="sxs-lookup"><span data-stu-id="96835-112">string</span></span>|<span data-ttu-id="96835-113">タイム ゾーンの識別子。</span><span class="sxs-lookup"><span data-stu-id="96835-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="96835-114">displayName</span><span class="sxs-lookup"><span data-stu-id="96835-114">displayName</span></span>|<span data-ttu-id="96835-115">string</span><span class="sxs-lookup"><span data-stu-id="96835-115">string</span></span>|<span data-ttu-id="96835-116">タイム ゾーンを表す表示文字列。</span><span class="sxs-lookup"><span data-stu-id="96835-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96835-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96835-117">JSON representation</span></span>

<span data-ttu-id="96835-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="96835-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneInformation"
}-->

```json
{
  "alias": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->