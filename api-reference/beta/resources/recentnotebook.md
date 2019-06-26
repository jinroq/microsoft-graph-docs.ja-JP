---
title: recentNotebook リソース型
description: 最近アクセスした OneNote ノートブック。 **recentNotebook** は、notebook と類似していますが、より少ないプロパティを持ちます。
localization_priority: Normal
ms.openlocfilehash: 599bee8d2f87cdc3809016909a73f21bd18651e1
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236567"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="f2af5-104">recentNotebook リソース型</span><span class="sxs-lookup"><span data-stu-id="f2af5-104">recentNotebook resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2af5-105">最近アクセスした OneNote ノートブック。</span><span class="sxs-lookup"><span data-stu-id="f2af5-105">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="f2af5-106">**recentNotebook** は、[notebook](notebook.md) と類似していますが、より少ないプロパティを持ちます。</span><span class="sxs-lookup"><span data-stu-id="f2af5-106">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="f2af5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2af5-107">Properties</span></span>
| <span data-ttu-id="f2af5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2af5-108">Property</span></span>     | <span data-ttu-id="f2af5-109">型</span><span class="sxs-lookup"><span data-stu-id="f2af5-109">Type</span></span>   |<span data-ttu-id="f2af5-110">説明</span><span class="sxs-lookup"><span data-stu-id="f2af5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2af5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f2af5-111">displayName</span></span>|<span data-ttu-id="f2af5-112">String</span><span class="sxs-lookup"><span data-stu-id="f2af5-112">String</span></span>|<span data-ttu-id="f2af5-113">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="f2af5-113">The name of the notebook.</span></span>|
|<span data-ttu-id="f2af5-114">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="f2af5-114">lastAccessedTime</span></span>|<span data-ttu-id="f2af5-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2af5-115">DateTimeOffset</span></span>|<span data-ttu-id="f2af5-116">ノートブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f2af5-116">The date and time when the notebook was last modified.</span></span> <span data-ttu-id="f2af5-117">Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f2af5-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f2af5-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f2af5-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f2af5-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f2af5-119">Read-only.</span></span>|
|<span data-ttu-id="f2af5-120">リンク</span><span class="sxs-lookup"><span data-stu-id="f2af5-120">links</span></span>|[<span data-ttu-id="f2af5-121">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="f2af5-121">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="f2af5-122">ノートブックを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="f2af5-122">Links for opening the notebook.</span></span> <span data-ttu-id="f2af5-123">`oneNoteClientURL` リンクは、OneNote クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="f2af5-123">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="f2af5-124">リンク`oneNoteWebURL`は、OneNote で web 上のノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="f2af5-124">The `oneNoteWebURL` link opens the notebook in OneNote on the web.</span></span>|
|<span data-ttu-id="f2af5-125">sourceService</span><span class="sxs-lookup"><span data-stu-id="f2af5-125">sourceService</span></span>|<span data-ttu-id="f2af5-126">String</span><span class="sxs-lookup"><span data-stu-id="f2af5-126">String</span></span>|<span data-ttu-id="f2af5-127">ノートブックが存在するバックエンド ストア (`OneDriveForBusiness` または `OneDrive` のいずれか)。</span><span class="sxs-lookup"><span data-stu-id="f2af5-127">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2af5-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2af5-128">JSON representation</span></span>

<span data-ttu-id="f2af5-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f2af5-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebook"
}-->

```json
{
  "displayName": "String",
  "lastAccessedTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.recentNotebookLinks"},
  "sourceService": "String"
}

```

## <a name="methods"></a><span data-ttu-id="f2af5-130">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2af5-130">Methods</span></span>

| <span data-ttu-id="f2af5-131">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2af5-131">Method</span></span>           | <span data-ttu-id="f2af5-132">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f2af5-132">Return Type</span></span>    |<span data-ttu-id="f2af5-133">説明</span><span class="sxs-lookup"><span data-stu-id="f2af5-133">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f2af5-134">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="f2af5-134">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="f2af5-135">[ノートブック](notebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f2af5-135">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="f2af5-136">ユーザーの最近アクセスしたノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f2af5-136">Get a collection of the most recently accessed notebooks for the user.</span></span> |
