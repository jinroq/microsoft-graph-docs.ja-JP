---
title: office365GroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: c94e79f688e117960b3a8a0f2c9888a908634a82
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572333"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="fb31c-103">office365GroupsActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fb31c-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="fb31c-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb31c-104">Properties</span></span>

| <span data-ttu-id="fb31c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fb31c-105">Property</span></span>               | <span data-ttu-id="fb31c-106">型</span><span class="sxs-lookup"><span data-stu-id="fb31c-106">Type</span></span>   | <span data-ttu-id="fb31c-107">説明</span><span class="sxs-lookup"><span data-stu-id="fb31c-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="fb31c-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="fb31c-108">reportRefreshDate</span></span>      | <span data-ttu-id="fb31c-109">日付</span><span class="sxs-lookup"><span data-stu-id="fb31c-109">Date</span></span>   | <span data-ttu-id="fb31c-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="fb31c-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="fb31c-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="fb31c-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="fb31c-112">Int64</span><span class="sxs-lookup"><span data-stu-id="fb31c-112">Int64</span></span>  | <span data-ttu-id="fb31c-113">グループのメールボックスで受信したメールの数です。</span><span class="sxs-lookup"><span data-stu-id="fb31c-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="fb31c-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="fb31c-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="fb31c-115">Int64</span><span class="sxs-lookup"><span data-stu-id="fb31c-115">Int64</span></span>  | <span data-ttu-id="fb31c-116">Yammer のグループに投稿されたメッセージの数です。</span><span class="sxs-lookup"><span data-stu-id="fb31c-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="fb31c-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="fb31c-117">yammerMessagesRead</span></span>     | <span data-ttu-id="fb31c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="fb31c-118">Int64</span></span>  | <span data-ttu-id="fb31c-119">Yammer グループでメッセージの数を読み取る。</span><span class="sxs-lookup"><span data-stu-id="fb31c-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="fb31c-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="fb31c-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="fb31c-121">Int64</span><span class="sxs-lookup"><span data-stu-id="fb31c-121">Int64</span></span>  | <span data-ttu-id="fb31c-122">Yammer グループに賛同のメッセージの数です。</span><span class="sxs-lookup"><span data-stu-id="fb31c-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="fb31c-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="fb31c-123">reportDate</span></span>             | <span data-ttu-id="fb31c-124">日付</span><span class="sxs-lookup"><span data-stu-id="fb31c-124">Date</span></span>   | <span data-ttu-id="fb31c-125">メールの数は、グループのメールボックスに送信されたまたはメッセージの数が転記された日付、または、Yammer グループで気に入られました</span><span class="sxs-lookup"><span data-stu-id="fb31c-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="fb31c-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="fb31c-126">reportPeriod</span></span>           | <span data-ttu-id="fb31c-127">String</span><span class="sxs-lookup"><span data-stu-id="fb31c-127">String</span></span> | <span data-ttu-id="fb31c-128">レポートの対象日数です。</span><span class="sxs-lookup"><span data-stu-id="fb31c-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="fb31c-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fb31c-129">JSON representation</span></span>

<span data-ttu-id="fb31c-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fb31c-130">The following is a JSON representation of the resource.</span></span>

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
