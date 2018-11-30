---
title: timeZoneBase リソースの種類
description: タイム ゾーンの基本的な表現です。
ms.openlocfilehash: 00e09b064a083aa72316838c213f9c84e1139a19
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073144"
---
# <a name="timezonebase-resource-type"></a><span data-ttu-id="ac264-103">timeZoneBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac264-103">timeZoneBase resource type</span></span>

> <span data-ttu-id="ac264-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ac264-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ac264-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac264-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ac264-106">タイム ゾーンの基本的な表現です。</span><span class="sxs-lookup"><span data-stu-id="ac264-106">The basic representation of a time zone.</span></span>


## <a name="properties"></a><span data-ttu-id="ac264-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac264-107">Properties</span></span>
| <span data-ttu-id="ac264-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac264-108">Property</span></span>     | <span data-ttu-id="ac264-109">型</span><span class="sxs-lookup"><span data-stu-id="ac264-109">Type</span></span>   |<span data-ttu-id="ac264-110">説明</span><span class="sxs-lookup"><span data-stu-id="ac264-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ac264-111">name</span><span class="sxs-lookup"><span data-stu-id="ac264-111">name</span></span> | <span data-ttu-id="ac264-112">文字列</span><span class="sxs-lookup"><span data-stu-id="ac264-112">string</span></span> | <span data-ttu-id="ac264-113">タイム ゾーンの名前。</span><span class="sxs-lookup"><span data-stu-id="ac264-113">The name of a time zone.</span></span> <span data-ttu-id="ac264-114">標準的なタイム ゾーンの名前 ("ハワイ アリューシャン標準時" など) を使用することも、カスタム タイム ゾーンとして "カスタム タイム ゾーン" という名前を指定することもできます。</span><span class="sxs-lookup"><span data-stu-id="ac264-114">It can be a standard time zone name such as "Hawaii-Aleutian Standard Time", or "Customized Time Zone" for a custom time zone.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="ac264-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac264-115">JSON representation</span></span>

<span data-ttu-id="ac264-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ac264-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeZoneBase"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeZoneBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->