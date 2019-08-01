---
title: timeZoneInformation リソースの種類
description: タイム ゾーンを表します。 サポートされる形式は、Windows、およびインターネットに割り当てられた電話番号 (IANA) タイムゾーン (Olson タイムゾーンとも呼ばれます)
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9a1efdb217b6f4970cf0925aa69ebb50f451e938
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033552"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="68ef3-104">timeZoneInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68ef3-104">timeZoneInformation resource type</span></span>


<span data-ttu-id="68ef3-105">タイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="68ef3-105">Represents a time zone.</span></span> <span data-ttu-id="68ef3-106">サポートされる形式は、Windows 形式です。現在既知の問題が解決されている場合は、[Internet Assigned Numbers Authority (IANA) タイム ゾーン](https://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式もサポートされます。</span><span class="sxs-lookup"><span data-stu-id="68ef3-106">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="68ef3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68ef3-107">Properties</span></span>
| <span data-ttu-id="68ef3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68ef3-108">Property</span></span>     | <span data-ttu-id="68ef3-109">型</span><span class="sxs-lookup"><span data-stu-id="68ef3-109">Type</span></span>   |<span data-ttu-id="68ef3-110">説明</span><span class="sxs-lookup"><span data-stu-id="68ef3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68ef3-111">エイリアス</span><span class="sxs-lookup"><span data-stu-id="68ef3-111">alias</span></span>|<span data-ttu-id="68ef3-112">string</span><span class="sxs-lookup"><span data-stu-id="68ef3-112">string</span></span>|<span data-ttu-id="68ef3-113">タイム ゾーンの識別子。</span><span class="sxs-lookup"><span data-stu-id="68ef3-113">An identifier for the time zone.</span></span>|
|<span data-ttu-id="68ef3-114">displayName</span><span class="sxs-lookup"><span data-stu-id="68ef3-114">displayName</span></span>|<span data-ttu-id="68ef3-115">string</span><span class="sxs-lookup"><span data-stu-id="68ef3-115">string</span></span>|<span data-ttu-id="68ef3-116">タイム ゾーンを表す表示文字列。</span><span class="sxs-lookup"><span data-stu-id="68ef3-116">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="68ef3-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68ef3-117">JSON representation</span></span>

<span data-ttu-id="68ef3-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68ef3-118">Here is a JSON representation of the resource.</span></span>

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
