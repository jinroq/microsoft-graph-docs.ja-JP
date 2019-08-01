---
title: OneNote リソースの種類
description: OneNote リソースのエントリ ポイントです。
author: jewan-microsoft
localization_priority: Priority
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 0311e514c7d15e8b5fafcc94beecaecdcc6d9d49
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035855"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="82187-103">OneNote リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82187-103">onenote resource type</span></span>

<span data-ttu-id="82187-104">OneNote リソースのエントリ ポイントです。</span><span class="sxs-lookup"><span data-stu-id="82187-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="82187-105">Microsoft Graph API を介しての OneNote サービスに対する呼び出しすべては、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="82187-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="82187-106">Office 365 またはコンシューマー OneDrive のユーザー ノートブック、Office 365 のグループ ノートブック、または SharePoint サイトでホストされているチームのノートブックを場所として指定できます。</span><span class="sxs-lookup"><span data-stu-id="82187-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="82187-107">**ユーザー ノートブック** コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="82187-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="82187-108">**グループ ノートブック** グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="82187-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="82187-109">**SharePoint サイト ノートブック** SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="82187-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="82187-110">承認</span><span class="sxs-lookup"><span data-stu-id="82187-110">Authorization</span></span>

<span data-ttu-id="82187-111">OneNote API で動作するために必要なアクセス許可については、「[メモのアクセス許可](/graph/permissions-reference#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82187-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="82187-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82187-112">Relationships</span></span>
| <span data-ttu-id="82187-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82187-113">Relationship</span></span> | <span data-ttu-id="82187-114">型</span><span class="sxs-lookup"><span data-stu-id="82187-114">Type</span></span>   |<span data-ttu-id="82187-115">説明</span><span class="sxs-lookup"><span data-stu-id="82187-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82187-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="82187-116">notebooks</span></span>|<span data-ttu-id="82187-117">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="82187-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="82187-118">ユーザーまたはグループが所有している OneNote ノートブックのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="82187-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="82187-119">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="82187-119">Read-only.</span></span> <span data-ttu-id="82187-120">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="82187-120">Nullable.</span></span>|
|<span data-ttu-id="82187-121">operations</span><span class="sxs-lookup"><span data-stu-id="82187-121">operations</span></span>|<span data-ttu-id="82187-122">[OnenoteOperation](onenoteoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="82187-122">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="82187-123">OneNote の操作の状態です。</span><span class="sxs-lookup"><span data-stu-id="82187-123">The status of OneNote operations.</span></span> <span data-ttu-id="82187-124">操作のコレクションを取得することはサポートされていませんが、応答で `Operation-Location` ヘッダーが返される場合には長時間実行処理の状態を取得できます。</span><span class="sxs-lookup"><span data-stu-id="82187-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="82187-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="82187-125">Read-only.</span></span> <span data-ttu-id="82187-126">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="82187-126">Nullable.</span></span>|
|<span data-ttu-id="82187-127">ページ</span><span class="sxs-lookup"><span data-stu-id="82187-127">pages</span></span>|<span data-ttu-id="82187-128">[OnenotePage](page.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="82187-128">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="82187-129">ユーザーまたはグループが所有しているすべての OneNote ノートブックのページです。</span><span class="sxs-lookup"><span data-stu-id="82187-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="82187-130">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="82187-130">Read-only.</span></span> <span data-ttu-id="82187-131">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="82187-131">Nullable.</span></span>|
|<span data-ttu-id="82187-132">リソース</span><span class="sxs-lookup"><span data-stu-id="82187-132">resources</span></span>|<span data-ttu-id="82187-133">[OnenoteResource](resource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="82187-133">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="82187-134">OneNote ページの画像リソースおよび他のファイル リソースです。</span><span class="sxs-lookup"><span data-stu-id="82187-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="82187-135">リソース コレクションを取得することはサポートされていませんが、[特定のリソースのバイナリ コンテンツを取得](resource.md)できます。</span><span class="sxs-lookup"><span data-stu-id="82187-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="82187-136">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="82187-136">Read-only.</span></span> <span data-ttu-id="82187-137">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="82187-137">Nullable.</span></span>|
|<span data-ttu-id="82187-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="82187-138">sectionGroups</span></span>|<span data-ttu-id="82187-139">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="82187-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="82187-140">ユーザーまたはグループが所有しているすべての OneNote ノートブックのセクション グループです。</span><span class="sxs-lookup"><span data-stu-id="82187-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="82187-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="82187-141">Read-only.</span></span> <span data-ttu-id="82187-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="82187-142">Nullable.</span></span>|
|<span data-ttu-id="82187-143">セクション</span><span class="sxs-lookup"><span data-stu-id="82187-143">sections</span></span>|<span data-ttu-id="82187-144">[OnenoteSection](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="82187-144">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="82187-145">ユーザーまたはグループが所有しているすべての OneNote ノートブック内のセクションです。</span><span class="sxs-lookup"><span data-stu-id="82187-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="82187-146">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="82187-146">Read-only.</span></span> <span data-ttu-id="82187-147">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="82187-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="82187-148">メソッド</span><span class="sxs-lookup"><span data-stu-id="82187-148">Methods</span></span>

| <span data-ttu-id="82187-149">メソッド</span><span class="sxs-lookup"><span data-stu-id="82187-149">Method</span></span>           | <span data-ttu-id="82187-150">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="82187-150">Return Type</span></span>    |<span data-ttu-id="82187-151">説明</span><span class="sxs-lookup"><span data-stu-id="82187-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82187-152">Create notebook</span><span class="sxs-lookup"><span data-stu-id="82187-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="82187-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="82187-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="82187-154">ノートブックのコレクションに投稿してノートブックを作成します。</span><span class="sxs-lookup"><span data-stu-id="82187-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="82187-155">List notebooks</span><span class="sxs-lookup"><span data-stu-id="82187-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="82187-156">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="82187-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="82187-157">ノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="82187-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="82187-158">Create page</span><span class="sxs-lookup"><span data-stu-id="82187-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="82187-159">Page</span><span class="sxs-lookup"><span data-stu-id="82187-159">Page</span></span>](page.md)| <span data-ttu-id="82187-160">ページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="82187-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="82187-161">List pages</span><span class="sxs-lookup"><span data-stu-id="82187-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="82187-162">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="82187-162">[Page](page.md) collection</span></span>| <span data-ttu-id="82187-163">ページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="82187-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="82187-164">List section groups</span><span class="sxs-lookup"><span data-stu-id="82187-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="82187-165">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="82187-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="82187-166">セクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="82187-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="82187-167">List sections</span><span class="sxs-lookup"><span data-stu-id="82187-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="82187-168">[OnenoteSection](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="82187-168">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="82187-169">セクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="82187-169">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="82187-170">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82187-170">JSON Representation</span></span>
<span data-ttu-id="82187-171">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82187-171">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
