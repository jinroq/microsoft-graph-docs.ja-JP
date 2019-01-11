---
title: automaticRepliesMailTips リソースの種類
description: メールボックスに設定されているすべての自動返信のメール ヒントです。
localization_priority: Normal
ms.openlocfilehash: bb477979b975996f70e4b8ac624befab7f254f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816276"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="e5737-103">automaticRepliesMailTips リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5737-103">automaticRepliesMailTips resource type</span></span>


<span data-ttu-id="e5737-104">メールボックスに設定されているすべての自動返信の[メール ヒント](../resources/mailtips.md)にします。</span><span class="sxs-lookup"><span data-stu-id="e5737-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="e5737-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5737-105">Properties</span></span>
| <span data-ttu-id="e5737-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5737-106">Property</span></span>     | <span data-ttu-id="e5737-107">種類</span><span class="sxs-lookup"><span data-stu-id="e5737-107">Type</span></span>   |<span data-ttu-id="e5737-108">説明</span><span class="sxs-lookup"><span data-stu-id="e5737-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="e5737-109">message</span><span class="sxs-lookup"><span data-stu-id="e5737-109">message</span></span> | <span data-ttu-id="e5737-110">String</span><span class="sxs-lookup"><span data-stu-id="e5737-110">String</span></span> | <span data-ttu-id="e5737-111">自動応答メッセージ。</span><span class="sxs-lookup"><span data-stu-id="e5737-111">The automatic reply message.</span></span> |
| <span data-ttu-id="e5737-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="e5737-112">messageLanguage</span></span> | [<span data-ttu-id="e5737-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="e5737-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="e5737-114">自動応答メッセージの言語。</span><span class="sxs-lookup"><span data-stu-id="e5737-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="e5737-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="e5737-115">scheduledEndTime</span></span> | [<span data-ttu-id="e5737-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e5737-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="e5737-117">自動応答を終了する日時。</span><span class="sxs-lookup"><span data-stu-id="e5737-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="e5737-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="e5737-118">scheduledStartTime</span></span> | [<span data-ttu-id="e5737-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="e5737-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="e5737-120">自動応答を開始する日時。</span><span class="sxs-lookup"><span data-stu-id="e5737-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e5737-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5737-121">JSON representation</span></span>

<span data-ttu-id="e5737-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5737-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "messageLanguage",
    "scheduledEndTime",
    "scheduledStartTime"
  ],
  "@odata.type": "microsoft.graph.automaticRepliesMailTips"
}-->

```json
{
  "message": "string",
  "messageLanguage": {"@odata.type": "microsoft.graph.localeInfo"},
  "scheduledEndTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "scheduledStartTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
