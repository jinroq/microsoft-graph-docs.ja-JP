---
title: 参加者リソースの種類
description: イベントの参加者です。 これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。
ms.openlocfilehash: 7c1a4d5fb483dc722768c9b95885837bdaf6087e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071206"
---
# <a name="attendee-resource-type"></a><span data-ttu-id="7436b-104">参加者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7436b-104">attendee resource type</span></span>

> <span data-ttu-id="7436b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7436b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7436b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7436b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7436b-107">イベントの参加者です。</span><span class="sxs-lookup"><span data-stu-id="7436b-107">An event attendee.</span></span> <span data-ttu-id="7436b-108">これはユーザー、またはテナントの Exchange Server 上でリソースとしてセットアップされている会議室や備品などのリソースとなります。</span><span class="sxs-lookup"><span data-stu-id="7436b-108">This can be a person or resource such as a meeting room or equipment, that has been set up as a resource on the Exchange server for the tenant.</span></span>

<span data-ttu-id="7436b-109">[attendeeBase](attendeebase.md) から派生します。</span><span class="sxs-lookup"><span data-stu-id="7436b-109">Derived from [attendeeBase](attendeebase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7436b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7436b-110">Properties</span></span>
| <span data-ttu-id="7436b-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7436b-111">Property</span></span>     | <span data-ttu-id="7436b-112">型</span><span class="sxs-lookup"><span data-stu-id="7436b-112">Type</span></span>   |<span data-ttu-id="7436b-113">説明</span><span class="sxs-lookup"><span data-stu-id="7436b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7436b-114">status</span><span class="sxs-lookup"><span data-stu-id="7436b-114">status</span></span>|[<span data-ttu-id="7436b-115">ResponseStatus</span><span class="sxs-lookup"><span data-stu-id="7436b-115">ResponseStatus</span></span>](responsestatus.md)|<span data-ttu-id="7436b-116">イベントに対する参加者からの応答 (なし、承諾、辞退など) と応答が送信された日時。</span><span class="sxs-lookup"><span data-stu-id="7436b-116">The attendee's response (none, accepted, declined, etc.) for the event and date-time that the response was sent.</span></span>|
|<span data-ttu-id="7436b-117">type</span><span class="sxs-lookup"><span data-stu-id="7436b-117">type</span></span>|<span data-ttu-id="7436b-118">String</span><span class="sxs-lookup"><span data-stu-id="7436b-118">String</span></span>|<span data-ttu-id="7436b-119">参加者のタイプは、`required`、`optional`、`resource` です。</span><span class="sxs-lookup"><span data-stu-id="7436b-119">The attendee type: `required`, `optional`, `resource`.</span></span>|
|<span data-ttu-id="7436b-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7436b-120">emailAddress</span></span>|[<span data-ttu-id="7436b-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7436b-121">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="7436b-122">参加者の名前と SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="7436b-122">Includes the name and SMTP address of the attendee.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7436b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7436b-123">JSON representation</span></span>

<span data-ttu-id="7436b-124">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7436b-124">Here is a JSON representation of the resource</span></span>

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