---
title: office365GroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 7e9f983d131d3b213689a48e10d8d23d3f99085b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968289"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="74f69-103">office365GroupsActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="74f69-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="74f69-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74f69-104">Properties</span></span>

| <span data-ttu-id="74f69-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74f69-105">Property</span></span>               | <span data-ttu-id="74f69-106">種類</span><span class="sxs-lookup"><span data-stu-id="74f69-106">Type</span></span>   | <span data-ttu-id="74f69-107">説明</span><span class="sxs-lookup"><span data-stu-id="74f69-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="74f69-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="74f69-108">reportRefreshDate</span></span>      | <span data-ttu-id="74f69-109">日付</span><span class="sxs-lookup"><span data-stu-id="74f69-109">Date</span></span>   | <span data-ttu-id="74f69-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="74f69-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="74f69-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="74f69-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="74f69-112">Int64</span><span class="sxs-lookup"><span data-stu-id="74f69-112">Int64</span></span>  | <span data-ttu-id="74f69-113">グループのメールボックスで受信したメールの数です。</span><span class="sxs-lookup"><span data-stu-id="74f69-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="74f69-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="74f69-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="74f69-115">Int64</span><span class="sxs-lookup"><span data-stu-id="74f69-115">Int64</span></span>  | <span data-ttu-id="74f69-116">Yammer のグループに投稿されたメッセージの数です。</span><span class="sxs-lookup"><span data-stu-id="74f69-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="74f69-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="74f69-117">yammerMessagesRead</span></span>     | <span data-ttu-id="74f69-118">Int64</span><span class="sxs-lookup"><span data-stu-id="74f69-118">Int64</span></span>  | <span data-ttu-id="74f69-119">Yammer グループでメッセージの数を読み取る。</span><span class="sxs-lookup"><span data-stu-id="74f69-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="74f69-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="74f69-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="74f69-121">Int64</span><span class="sxs-lookup"><span data-stu-id="74f69-121">Int64</span></span>  | <span data-ttu-id="74f69-122">Yammer グループに賛同のメッセージの数です。</span><span class="sxs-lookup"><span data-stu-id="74f69-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="74f69-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="74f69-123">reportDate</span></span>             | <span data-ttu-id="74f69-124">日付</span><span class="sxs-lookup"><span data-stu-id="74f69-124">Date</span></span>   | <span data-ttu-id="74f69-125">メールの数は、グループのメールボックスに送信されたまたはメッセージの数が転記された日付、または、Yammer グループで気に入られました</span><span class="sxs-lookup"><span data-stu-id="74f69-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="74f69-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="74f69-126">reportPeriod</span></span>           | <span data-ttu-id="74f69-127">String</span><span class="sxs-lookup"><span data-stu-id="74f69-127">String</span></span> | <span data-ttu-id="74f69-128">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="74f69-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="74f69-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="74f69-129">JSON representation</span></span>

<span data-ttu-id="74f69-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74f69-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeEmailsReceived": 1024, 
  "yammerMessagesPosted": 1024, 
  "yammerMessagesRead": 1024, 
  "yammerMessagesLiked": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
