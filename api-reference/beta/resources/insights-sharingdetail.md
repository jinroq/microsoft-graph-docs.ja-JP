---
title: sharingDetail リソースの種類
description: '共有アイテムのプロパティを格納する複合型。 '
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: add63a89a451b742778dda1d6d313d58f675a642
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918764"
---
# <a name="sharingdetail-resource-type"></a><span data-ttu-id="60817-103">sharingDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60817-103">sharingDetail resource type</span></span>

> <span data-ttu-id="60817-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="60817-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60817-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60817-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="60817-106">[共有](insights-shared.md)アイテムのプロパティを格納する複合型。</span><span class="sxs-lookup"><span data-stu-id="60817-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="60817-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60817-107">JSON representation</span></span>
<span data-ttu-id="60817-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="60817-108">Here is a JSON representation of the resource</span></span>

```json
{
  "sharedDateTime": "dateTimeOffset",
  "sharingSubject": "string",
  "sharingType": "string",
  "sharedBy": "insightIdentity",
  "resourceReference": "resourceReference"
}
```

## <a name="properties"></a><span data-ttu-id="60817-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60817-109">Properties</span></span>

| <span data-ttu-id="60817-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60817-110">Property</span></span>              | <span data-ttu-id="60817-111">種類</span><span class="sxs-lookup"><span data-stu-id="60817-111">Type</span></span>          | <span data-ttu-id="60817-112">説明</span><span class="sxs-lookup"><span data-stu-id="60817-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="60817-113">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="60817-113">sharedDateTime</span></span>        | <span data-ttu-id="60817-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60817-114">DateTimeOffset</span></span>| <span data-ttu-id="60817-115">日付と時刻、ファイルが最後に共有します。</span><span class="sxs-lookup"><span data-stu-id="60817-115">The date and time the file was last shared.</span></span> <span data-ttu-id="60817-116">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="60817-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="60817-117">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="60817-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="60817-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="60817-118">Read-only.</span></span>  |
| <span data-ttu-id="60817-119">sharingSubject</span><span class="sxs-lookup"><span data-stu-id="60817-119">sharingSubject</span></span>        | <span data-ttu-id="60817-120">String</span><span class="sxs-lookup"><span data-stu-id="60817-120">String</span></span>          | <span data-ttu-id="60817-121">ドキュメントを共有している情報カテゴリです。</span><span class="sxs-lookup"><span data-stu-id="60817-121">The subject with which the document was shared.</span></span> |
| <span data-ttu-id="60817-122">sharingType</span><span class="sxs-lookup"><span data-stu-id="60817-122">sharingType</span></span>             | <span data-ttu-id="60817-123">String</span><span class="sxs-lookup"><span data-stu-id="60817-123">String</span></span>        | <span data-ttu-id="60817-124">方法、ドキュメントが共有されていた、「リンク」、「添付ファイル」、「グループ」、「サイト」であることができますを決定します。</span><span class="sxs-lookup"><span data-stu-id="60817-124">Determines the way the document was shared, can be by a "Link", "Attachment", "Group", "Site".</span></span>     |
| <span data-ttu-id="60817-125">sharedBy</span><span class="sxs-lookup"><span data-stu-id="60817-125">sharedBy</span></span>                | [<span data-ttu-id="60817-126">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="60817-126">insightIdentity</span></span>](insights-insightidentity.md)      | <span data-ttu-id="60817-127">ドキュメントを共有するユーザーです。</span><span class="sxs-lookup"><span data-stu-id="60817-127">The user who shared the document.</span></span>  |
| <span data-ttu-id="60817-128">sharingReference</span><span class="sxs-lookup"><span data-stu-id="60817-128">sharingReference</span></span>        | [<span data-ttu-id="60817-129">resourceReference</span><span class="sxs-lookup"><span data-stu-id="60817-129">resourceReference</span></span>](insights-resourcereference.md)      |  |
