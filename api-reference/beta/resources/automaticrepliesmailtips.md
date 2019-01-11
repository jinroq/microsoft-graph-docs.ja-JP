---
title: automaticRepliesMailTips リソースの種類
description: メールボックスに設定されているすべての自動返信のメール ヒントです。
localization_priority: Normal
ms.openlocfilehash: 80ecaaa9fced0bcb00494b0414a86f0a11fd8996
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833230"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="3e733-103">automaticRepliesMailTips リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3e733-103">automaticRepliesMailTips resource type</span></span>

> <span data-ttu-id="3e733-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3e733-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e733-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e733-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3e733-106">メールボックスに設定されているすべての自動返信の[メール ヒント](../resources/mailtips.md)にします。</span><span class="sxs-lookup"><span data-stu-id="3e733-106">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="3e733-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e733-107">Properties</span></span>
| <span data-ttu-id="3e733-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e733-108">Property</span></span>     | <span data-ttu-id="3e733-109">種類</span><span class="sxs-lookup"><span data-stu-id="3e733-109">Type</span></span>   |<span data-ttu-id="3e733-110">説明</span><span class="sxs-lookup"><span data-stu-id="3e733-110">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="3e733-111">message</span><span class="sxs-lookup"><span data-stu-id="3e733-111">message</span></span> | <span data-ttu-id="3e733-112">String</span><span class="sxs-lookup"><span data-stu-id="3e733-112">String</span></span> | <span data-ttu-id="3e733-113">自動応答メッセージ。</span><span class="sxs-lookup"><span data-stu-id="3e733-113">The automatic reply message.</span></span> |
| <span data-ttu-id="3e733-114">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="3e733-114">messageLanguage</span></span> | [<span data-ttu-id="3e733-115">localeInfo</span><span class="sxs-lookup"><span data-stu-id="3e733-115">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="3e733-116">自動応答メッセージの言語。</span><span class="sxs-lookup"><span data-stu-id="3e733-116">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="3e733-117">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="3e733-117">scheduledEndTime</span></span> | [<span data-ttu-id="3e733-118">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e733-118">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="3e733-119">自動応答を終了する日時。</span><span class="sxs-lookup"><span data-stu-id="3e733-119">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="3e733-120">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="3e733-120">scheduledStartTime</span></span> | [<span data-ttu-id="3e733-121">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e733-121">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="3e733-122">自動応答を開始する日時。</span><span class="sxs-lookup"><span data-stu-id="3e733-122">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="3e733-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e733-123">JSON representation</span></span>

<span data-ttu-id="3e733-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3e733-124">Here is a JSON representation of the resource.</span></span>

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
