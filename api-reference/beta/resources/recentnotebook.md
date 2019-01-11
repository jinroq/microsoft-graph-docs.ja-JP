---
title: recentNotebook リソース型
description: 最近アクセスした OneNote ノートブック。 **recentNotebook** は、notebook と類似していますが、より少ないプロパティを持ちます。
localization_priority: Normal
ms.openlocfilehash: f2dd1ca642203cde36bb636b9cb2eb7c79344e3e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833832"
---
# <a name="recentnotebook-resource-type"></a><span data-ttu-id="77c67-104">recentNotebook リソース型</span><span class="sxs-lookup"><span data-stu-id="77c67-104">recentNotebook resource type</span></span>

> <span data-ttu-id="77c67-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="77c67-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77c67-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77c67-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="77c67-107">最近アクセスした OneNote ノートブック。</span><span class="sxs-lookup"><span data-stu-id="77c67-107">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="77c67-108">**recentNotebook** は、[notebook](notebook.md) と類似していますが、より少ないプロパティを持ちます。</span><span class="sxs-lookup"><span data-stu-id="77c67-108">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="77c67-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77c67-109">Properties</span></span>
| <span data-ttu-id="77c67-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77c67-110">Property</span></span>     | <span data-ttu-id="77c67-111">種類</span><span class="sxs-lookup"><span data-stu-id="77c67-111">Type</span></span>   |<span data-ttu-id="77c67-112">説明</span><span class="sxs-lookup"><span data-stu-id="77c67-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77c67-113">名前</span><span class="sxs-lookup"><span data-stu-id="77c67-113">name</span></span>|<span data-ttu-id="77c67-114">String</span><span class="sxs-lookup"><span data-stu-id="77c67-114">String</span></span>|<span data-ttu-id="77c67-115">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="77c67-115">The name of the notebook.</span></span>|
|<span data-ttu-id="77c67-116">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="77c67-116">lastAccessedTime</span></span>|<span data-ttu-id="77c67-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77c67-117">DateTimeOffset</span></span>|<span data-ttu-id="77c67-p104">ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="77c67-p104">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="77c67-122">リンク</span><span class="sxs-lookup"><span data-stu-id="77c67-122">links</span></span>|[<span data-ttu-id="77c67-123">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="77c67-123">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="77c67-124">ノートブックを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="77c67-124">Links for opening the notebook.</span></span> <span data-ttu-id="77c67-125">`oneNoteClientURL` リンクは、OneNote クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="77c67-125">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="77c67-126">`oneNoteWebURL` リンクは、OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="77c67-126">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="77c67-127">sourceService</span><span class="sxs-lookup"><span data-stu-id="77c67-127">sourceService</span></span>|<span data-ttu-id="77c67-128">String</span><span class="sxs-lookup"><span data-stu-id="77c67-128">String</span></span>|<span data-ttu-id="77c67-129">ノートブックが存在するバックエンド ストア (`OneDriveForBusiness` または `OneDrive` のいずれか)。</span><span class="sxs-lookup"><span data-stu-id="77c67-129">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="77c67-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="77c67-130">JSON representation</span></span>

<span data-ttu-id="77c67-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="77c67-131">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="77c67-132">メソッド</span><span class="sxs-lookup"><span data-stu-id="77c67-132">Methods</span></span>

| <span data-ttu-id="77c67-133">メソッド</span><span class="sxs-lookup"><span data-stu-id="77c67-133">Method</span></span>           | <span data-ttu-id="77c67-134">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="77c67-134">Return Type</span></span>    |<span data-ttu-id="77c67-135">説明</span><span class="sxs-lookup"><span data-stu-id="77c67-135">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77c67-136">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="77c67-136">getRecentNotebooks</span></span>](../api/notebook-getrecentnotebooks.md) | <span data-ttu-id="77c67-137">[ノートブック](notebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="77c67-137">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="77c67-138">ユーザーの最近アクセスしたノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="77c67-138">Get a collection of the most recently accessed notebooks for the user.</span></span> |
