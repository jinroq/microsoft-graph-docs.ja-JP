---
title: timeZoneInformation リソースの種類
description: タイム ゾーンを表します。 サポートされている形式は、Windows、およびインターネット割り当て番号機関 (IANA) はタイム ゾーン (Olson タイム ・ ゾーンとも呼ばれます)
localization_priority: Normal
ms.openlocfilehash: dc53cca34ef9c6a53a39394cbba8be4e1baca662
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839740"
---
# <a name="timezoneinformation-resource-type"></a><span data-ttu-id="81af3-104">timeZoneInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81af3-104">timeZoneInformation resource type</span></span>

> <span data-ttu-id="81af3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81af3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81af3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81af3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81af3-107">タイム ゾーンを表します。</span><span class="sxs-lookup"><span data-stu-id="81af3-107">Represents a time zone.</span></span> <span data-ttu-id="81af3-108">サポートされる形式は、Windows 形式です。現在既知の問題が解決されている場合は、[Internet Assigned Numbers Authority (IANA) タイム ゾーン](https://www.iana.org/time-zones) (Olson タイム ゾーンとも呼ばれる) 形式もサポートされます。</span><span class="sxs-lookup"><span data-stu-id="81af3-108">The supported format is Windows, and [Internet Assigned Numbers Authority (IANA) time zone](https://www.iana.org/time-zones) (also known as Olson time zone) format as well when the current known problem is fixed.</span></span>

## <a name="properties"></a><span data-ttu-id="81af3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81af3-109">Properties</span></span>
| <span data-ttu-id="81af3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81af3-110">Property</span></span>     | <span data-ttu-id="81af3-111">種類</span><span class="sxs-lookup"><span data-stu-id="81af3-111">Type</span></span>   |<span data-ttu-id="81af3-112">説明</span><span class="sxs-lookup"><span data-stu-id="81af3-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81af3-113">alias</span><span class="sxs-lookup"><span data-stu-id="81af3-113">alias</span></span>|<span data-ttu-id="81af3-114">文字列</span><span class="sxs-lookup"><span data-stu-id="81af3-114">string</span></span>|<span data-ttu-id="81af3-115">タイム ゾーンの識別子。</span><span class="sxs-lookup"><span data-stu-id="81af3-115">An identifier for the time zone.</span></span>|
|<span data-ttu-id="81af3-116">displayName</span><span class="sxs-lookup"><span data-stu-id="81af3-116">displayName</span></span>|<span data-ttu-id="81af3-117">string</span><span class="sxs-lookup"><span data-stu-id="81af3-117">string</span></span>|<span data-ttu-id="81af3-118">タイム ゾーンを表す表示文字列。</span><span class="sxs-lookup"><span data-stu-id="81af3-118">A display string that represents the time zone.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="81af3-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81af3-119">JSON representation</span></span>

<span data-ttu-id="81af3-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="81af3-120">Here is a JSON representation of the resource.</span></span>

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
