---
title: office365GroupsActivityCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: c1e441b142ef27abbdde4ac613ef8d75848f5001
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966553"
---
# <a name="office365groupsactivitycounts-resource-type"></a><span data-ttu-id="267aa-103">office365GroupsActivityCounts リソースの種類</span><span class="sxs-lookup"><span data-stu-id="267aa-103">office365GroupsActivityCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="267aa-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="267aa-104">Properties</span></span>

| <span data-ttu-id="267aa-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="267aa-105">Property</span></span>               | <span data-ttu-id="267aa-106">型</span><span class="sxs-lookup"><span data-stu-id="267aa-106">Type</span></span>   | <span data-ttu-id="267aa-107">説明</span><span class="sxs-lookup"><span data-stu-id="267aa-107">Description</span></span>                              |
| :--------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="267aa-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="267aa-108">reportRefreshDate</span></span>      | <span data-ttu-id="267aa-109">日付</span><span class="sxs-lookup"><span data-stu-id="267aa-109">Date</span></span>   | <span data-ttu-id="267aa-110">コンテンツの最新の日付。</span><span class="sxs-lookup"><span data-stu-id="267aa-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="267aa-111">exchangeEmailsReceived</span><span class="sxs-lookup"><span data-stu-id="267aa-111">exchangeEmailsReceived</span></span> | <span data-ttu-id="267aa-112">Int64</span><span class="sxs-lookup"><span data-stu-id="267aa-112">Int64</span></span>  | <span data-ttu-id="267aa-113">グループメールボックスで受信したメールの数。</span><span class="sxs-lookup"><span data-stu-id="267aa-113">The number of emails received by Group mailboxes.</span></span> |
| <span data-ttu-id="267aa-114">yammerMessagesPosted</span><span class="sxs-lookup"><span data-stu-id="267aa-114">yammerMessagesPosted</span></span>   | <span data-ttu-id="267aa-115">Int64</span><span class="sxs-lookup"><span data-stu-id="267aa-115">Int64</span></span>  | <span data-ttu-id="267aa-116">Yammer グループに投稿されたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="267aa-116">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="267aa-117">yammerMessagesRead</span><span class="sxs-lookup"><span data-stu-id="267aa-117">yammerMessagesRead</span></span>     | <span data-ttu-id="267aa-118">Int64</span><span class="sxs-lookup"><span data-stu-id="267aa-118">Int64</span></span>  | <span data-ttu-id="267aa-119">Yammer グループで読み取られたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="267aa-119">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="267aa-120">yammerMessagesLiked</span><span class="sxs-lookup"><span data-stu-id="267aa-120">yammerMessagesLiked</span></span>    | <span data-ttu-id="267aa-121">Int64</span><span class="sxs-lookup"><span data-stu-id="267aa-121">Int64</span></span>  | <span data-ttu-id="267aa-122">Yammer グループに賛同されたメッセージの数。</span><span class="sxs-lookup"><span data-stu-id="267aa-122">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="267aa-123">reportDate</span><span class="sxs-lookup"><span data-stu-id="267aa-123">reportDate</span></span>             | <span data-ttu-id="267aa-124">日付</span><span class="sxs-lookup"><span data-stu-id="267aa-124">Date</span></span>   | <span data-ttu-id="267aa-125">グループメールボックスに送信されたメールの数またはメッセージ数が Yammer グループで投稿、読み取り、または賛同された日付</span><span class="sxs-lookup"><span data-stu-id="267aa-125">The date on which a number of emails were sent to a group mailbox or a number of messages were posted, read, or liked in a Yammer group</span></span> |
| <span data-ttu-id="267aa-126">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="267aa-126">reportPeriod</span></span>           | <span data-ttu-id="267aa-127">String</span><span class="sxs-lookup"><span data-stu-id="267aa-127">String</span></span> | <span data-ttu-id="267aa-128">レポートの対象となる日数を指定します。</span><span class="sxs-lookup"><span data-stu-id="267aa-128">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="267aa-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="267aa-129">JSON representation</span></span>

<span data-ttu-id="267aa-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="267aa-130">The following is a JSON representation of the resource.</span></span>

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
