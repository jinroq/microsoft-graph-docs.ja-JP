---
title: recentNotebook リソース型
description: 最近アクセスした OneNote ノートブック。 **recentNotebook** は、notebook と類似していますが、より少ないプロパティを持ちます。
ms.openlocfilehash: c3b717fcebdc229864aefe13c6452ce5eb95fc53
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070218"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="8a2ad-104">recentNotebook リソース型</span><span class="sxs-lookup"><span data-stu-id="8a2ad-104">recentNotebook resource type</span></span>

> <span data-ttu-id="8a2ad-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8a2ad-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8a2ad-107">最近アクセスした OneNote ノートブック。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-107">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="8a2ad-108">**recentNotebook** は、[notebook](notebook.md) と類似していますが、より少ないプロパティを持ちます。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-108">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="8a2ad-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a2ad-109">Properties</span></span>
| <span data-ttu-id="8a2ad-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8a2ad-110">Property</span></span>     | <span data-ttu-id="8a2ad-111">型</span><span class="sxs-lookup"><span data-stu-id="8a2ad-111">Type</span></span>   |<span data-ttu-id="8a2ad-112">説明</span><span class="sxs-lookup"><span data-stu-id="8a2ad-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a2ad-113">名前</span><span class="sxs-lookup"><span data-stu-id="8a2ad-113">name</span></span>|<span data-ttu-id="8a2ad-114">String</span><span class="sxs-lookup"><span data-stu-id="8a2ad-114">String</span></span>|<span data-ttu-id="8a2ad-115">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-115">The name of the notebook.</span></span>|
|<span data-ttu-id="8a2ad-116">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="8a2ad-116">lastAccessedTime</span></span>|<span data-ttu-id="8a2ad-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a2ad-117">DateTimeOffset</span></span>|<span data-ttu-id="8a2ad-p104">ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-p104">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="8a2ad-122">リンク</span><span class="sxs-lookup"><span data-stu-id="8a2ad-122">links</span></span>|[<span data-ttu-id="8a2ad-123">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="8a2ad-123">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="8a2ad-124">ノートブックを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-124">Links for opening the notebook.</span></span> <span data-ttu-id="8a2ad-125">`oneNoteClientURL` リンクは、OneNote クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-125">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="8a2ad-126">`oneNoteWebURL` リンクは、OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-126">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="8a2ad-127">sourceService</span><span class="sxs-lookup"><span data-stu-id="8a2ad-127">sourceService</span></span>|<span data-ttu-id="8a2ad-128">String</span><span class="sxs-lookup"><span data-stu-id="8a2ad-128">String</span></span>|<span data-ttu-id="8a2ad-129">ノートブックが存在するバックエンド ストア (`OneDriveForBusiness` または `OneDrive` のいずれか)。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-129">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a2ad-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8a2ad-130">JSON representation</span></span>

<span data-ttu-id="8a2ad-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="8a2ad-132">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a2ad-132">Methods</span></span>

| <span data-ttu-id="8a2ad-133">メソッド</span><span class="sxs-lookup"><span data-stu-id="8a2ad-133">Method</span></span>           | <span data-ttu-id="8a2ad-134">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8a2ad-134">Return Type</span></span>    |<span data-ttu-id="8a2ad-135">説明</span><span class="sxs-lookup"><span data-stu-id="8a2ad-135">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a2ad-136">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="8a2ad-136">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="8a2ad-137">[ノートブック](notebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8a2ad-137">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="8a2ad-138">ユーザーの最近アクセスしたノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8a2ad-138">Get a collection of the most recently accessed notebooks for the user.</span></span> |
