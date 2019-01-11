---
title: 参加者リソースの種類
description: イベントの参加者です。 これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。
localization_priority: Normal
ms.openlocfilehash: 95881d0e2f3dfe51b975e60ba6f8d32cda5e222c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859326"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="57f21-104">参加者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="57f21-104">attendee resource type</span></span>

> <span data-ttu-id="57f21-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57f21-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57f21-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57f21-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="57f21-107">イベントの参加者です。</span><span class="sxs-lookup"><span data-stu-id="57f21-107">An event attendee.</span></span> <span data-ttu-id="57f21-108">これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。</span><span class="sxs-lookup"><span data-stu-id="57f21-108">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="57f21-109">[attendeeBase](attendeebase.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="57f21-109">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="57f21-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57f21-110">Properties</span></span>
| <span data-ttu-id="57f21-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57f21-111">Property</span></span>     | <span data-ttu-id="57f21-112">種類</span><span class="sxs-lookup"><span data-stu-id="57f21-112">Type</span></span>   |<span data-ttu-id="57f21-113">説明</span><span class="sxs-lookup"><span data-stu-id="57f21-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57f21-114">status</span><span class="sxs-lookup"><span data-stu-id="57f21-114">status</span></span>|[<span data-ttu-id="57f21-115">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="57f21-115">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="57f21-116">イベントに対する参加者からの応答 (なし、承諾、辞退など) と応答が送信された日時。</span><span class="sxs-lookup"><span data-stu-id="57f21-116">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="57f21-117">type</span><span class="sxs-lookup"><span data-stu-id="57f21-117">type</span></span>|<span data-ttu-id="57f21-118">String</span><span class="sxs-lookup"><span data-stu-id="57f21-118">String</span></span>|<span data-ttu-id="57f21-119">参加者のタイプは、`required`、`optional`、`resource` です。</span><span class="sxs-lookup"><span data-stu-id="57f21-119">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="57f21-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="57f21-120">emailAddress</span></span>|[<span data-ttu-id="57f21-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="57f21-121">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="57f21-122">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="57f21-122">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57f21-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="57f21-123">JSON representation</span></span>

<span data-ttu-id="57f21-124">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="57f21-124">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attendee resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
