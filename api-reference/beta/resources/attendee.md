---
title: 参加者リソースの種類
description: イベントの参加者です。 これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。
localization_priority: Normal
ms.openlocfilehash: 12512ea274e549cacba364fb394a3346e6bfee56
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328622"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="fa057-104">参加者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fa057-104">attendee resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa057-105">イベントの参加者です。</span><span class="sxs-lookup"><span data-stu-id="fa057-105">An event attendee.</span></span> <span data-ttu-id="fa057-106">これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。</span><span class="sxs-lookup"><span data-stu-id="fa057-106">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="fa057-107">[attendeeBase](attendeebase.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="fa057-107">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fa057-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa057-108">Properties</span></span>
| <span data-ttu-id="fa057-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fa057-109">Property</span></span>     | <span data-ttu-id="fa057-110">型</span><span class="sxs-lookup"><span data-stu-id="fa057-110">Type</span></span>   |<span data-ttu-id="fa057-111">説明</span><span class="sxs-lookup"><span data-stu-id="fa057-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa057-112">status</span><span class="sxs-lookup"><span data-stu-id="fa057-112">status</span></span>|[<span data-ttu-id="fa057-113">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="fa057-113">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="fa057-114">イベントに対する参加者からの応答 (なし、承諾、辞退など) と応答が送信された日時。</span><span class="sxs-lookup"><span data-stu-id="fa057-114">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="fa057-115">type</span><span class="sxs-lookup"><span data-stu-id="fa057-115">type</span></span>|<span data-ttu-id="fa057-116">String</span><span class="sxs-lookup"><span data-stu-id="fa057-116">String</span></span>|<span data-ttu-id="fa057-117">参加者のタイプは、`required`、`optional`、`resource` です。</span><span class="sxs-lookup"><span data-stu-id="fa057-117">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="fa057-118">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fa057-118">emailAddress</span></span>|[<span data-ttu-id="fa057-119">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fa057-119">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="fa057-120">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="fa057-120">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa057-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fa057-121">JSON representation</span></span>

<span data-ttu-id="fa057-122">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="fa057-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendee"
}-->

```json
{
  "status": {"@odata.type": "microsoft.graph.responseStatus"},
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
