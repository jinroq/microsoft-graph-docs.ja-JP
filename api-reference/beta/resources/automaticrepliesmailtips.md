---
title: automaticRepliesMailTips リソースの種類
description: メールボックスに設定されている自動応答に関するメールヒント。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 74fda9db7de1a97ce2b7e44ca9d56020b87ab6f9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974250"
---
# <a name="automaticrepliesmailtips-resource-type"></a><span data-ttu-id="be64b-103">automaticRepliesMailTips リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be64b-103">automaticRepliesMailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be64b-104">メールボックスに設定されている自動応答に関する[メールヒント](../resources/mailtips.md)。</span><span class="sxs-lookup"><span data-stu-id="be64b-104">[MailTips](../resources/mailtips.md) about any automatic replies that have been set up on a mailbox.</span></span>

## <a name="properties"></a><span data-ttu-id="be64b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be64b-105">Properties</span></span>
| <span data-ttu-id="be64b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be64b-106">Property</span></span>     | <span data-ttu-id="be64b-107">型</span><span class="sxs-lookup"><span data-stu-id="be64b-107">Type</span></span>   |<span data-ttu-id="be64b-108">説明</span><span class="sxs-lookup"><span data-stu-id="be64b-108">Description</span></span>|
|:-----|:-----|:-----|
| <span data-ttu-id="be64b-109">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="be64b-109">message</span></span> | <span data-ttu-id="be64b-110">String</span><span class="sxs-lookup"><span data-stu-id="be64b-110">String</span></span> | <span data-ttu-id="be64b-111">自動応答メッセージ。</span><span class="sxs-lookup"><span data-stu-id="be64b-111">The automatic reply message.</span></span> |
| <span data-ttu-id="be64b-112">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="be64b-112">messageLanguage</span></span> | [<span data-ttu-id="be64b-113">localeInfo</span><span class="sxs-lookup"><span data-stu-id="be64b-113">localeInfo</span></span>](../resources/localeinfo.md) | <span data-ttu-id="be64b-114">自動応答メッセージが含まれる言語。</span><span class="sxs-lookup"><span data-stu-id="be64b-114">The language that the automatic reply message is in.</span></span> |
| <span data-ttu-id="be64b-115">scheduledEndTime</span><span class="sxs-lookup"><span data-stu-id="be64b-115">scheduledEndTime</span></span> | [<span data-ttu-id="be64b-116">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="be64b-116">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="be64b-117">自動応答を終了する日付と時刻を指定します。</span><span class="sxs-lookup"><span data-stu-id="be64b-117">The date and time that automatic replies are set to end.</span></span> |
| <span data-ttu-id="be64b-118">scheduledStartTime</span><span class="sxs-lookup"><span data-stu-id="be64b-118">scheduledStartTime</span></span> | [<span data-ttu-id="be64b-119">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="be64b-119">dateTimeTimeZone</span></span>](../resources/datetimetimezone.md) | <span data-ttu-id="be64b-120">自動応答が開始される日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="be64b-120">The date and time that automatic replies are set to begin.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="be64b-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be64b-121">JSON representation</span></span>

<span data-ttu-id="be64b-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be64b-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "automaticRepliesMailTips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
