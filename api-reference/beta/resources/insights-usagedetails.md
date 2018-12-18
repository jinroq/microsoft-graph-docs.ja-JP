---
title: usageDetails リソースの種類
description: 複合型を使用する項目のプロパティが含まれています。 リソースが最後にアクセスしたときに情報 (表示)、ユーザーが (編集) を変更します。
author: simonhult
ms.openlocfilehash: ef5efcfce439e9d08784637cb02657d7cd37adf7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349351"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="7d4e4-104">usageDetails リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7d4e4-104">usageDetails resource type</span></span>

> <span data-ttu-id="7d4e4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d4e4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d4e4-107">複合型が[使用されている](insights-used.md)アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-107">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="7d4e4-108">リソースが最後にアクセスしたときに情報 (表示)、ユーザーが (編集) を変更します。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-108">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d4e4-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7d4e4-109">JSON representation</span></span>

<span data-ttu-id="7d4e4-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7d4e4-110">Here is a JSON representation of the resource</span></span>

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="7d4e4-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d4e4-111">Properties</span></span>

| <span data-ttu-id="7d4e4-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d4e4-112">Property</span></span>              | <span data-ttu-id="7d4e4-113">種類</span><span class="sxs-lookup"><span data-stu-id="7d4e4-113">Type</span></span>          | <span data-ttu-id="7d4e4-114">説明</span><span class="sxs-lookup"><span data-stu-id="7d4e4-114">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="7d4e4-115">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d4e4-115">lastAccessedDateTime</span></span>                  | <span data-ttu-id="7d4e4-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d4e4-116">DateTimeOffset</span></span>        | <span data-ttu-id="7d4e4-117">日付と時刻、リソースは、ユーザーが最後にアクセスしました。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-117">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="7d4e4-118">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-118">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d4e4-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="7d4e4-119">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="7d4e4-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-120">Read-only.</span></span>                      |
| <span data-ttu-id="7d4e4-121">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d4e4-121">lastModifiedDateTime</span></span>              | <span data-ttu-id="7d4e4-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d4e4-122">DateTimeOffset</span></span>        | <span data-ttu-id="7d4e4-123">日付と時刻、ユーザーによってリソースが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-123">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="7d4e4-124">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-124">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7d4e4-125">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="7d4e4-125">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="7d4e4-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7d4e4-126">Read-only.</span></span>       |