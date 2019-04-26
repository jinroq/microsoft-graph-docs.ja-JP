---
title: OneNote リソースの種類
description: OneNote リソースのエントリ ポイントです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561657"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="92f8b-103">OneNote リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92f8b-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92f8b-104">OneNote リソースのエントリ ポイントです。</span><span class="sxs-lookup"><span data-stu-id="92f8b-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="92f8b-105">Microsoft Graph API を介しての OneNote サービスに対する呼び出しすべては、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="92f8b-106">この場所は、office 365 またはコンシューマー OneDrive、グループノートブック、または office 365 上の SharePoint サイトでホストされるチームノートブックのユーザーノートブックであることができます。</span><span class="sxs-lookup"><span data-stu-id="92f8b-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="92f8b-107">**ユーザー ノートブック** コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="92f8b-108">**グループ ノートブック** グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="92f8b-109">**SharePoint サイト ノートブック** SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="92f8b-110">承認</span><span class="sxs-lookup"><span data-stu-id="92f8b-110">Authorization</span></span>

<span data-ttu-id="92f8b-111">OneNote API で動作するために必要なアクセス許可については、「[メモのアクセス許可](/graph/permissions-reference#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92f8b-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="92f8b-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92f8b-112">Relationships</span></span>
| <span data-ttu-id="92f8b-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92f8b-113">Relationship</span></span> | <span data-ttu-id="92f8b-114">型</span><span class="sxs-lookup"><span data-stu-id="92f8b-114">Type</span></span>   |<span data-ttu-id="92f8b-115">説明</span><span class="sxs-lookup"><span data-stu-id="92f8b-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="92f8b-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="92f8b-116">notebooks</span></span>|<span data-ttu-id="92f8b-117">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="92f8b-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="92f8b-118">ユーザーまたはグループが所有している OneNote ノートブックのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="92f8b-118">The collection of OneNote notebooks that are owned by the user or group.</span></span> <span data-ttu-id="92f8b-119">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92f8b-119">Read-only.</span></span> <span data-ttu-id="92f8b-120">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92f8b-120">Nullable.</span></span>|
|<span data-ttu-id="92f8b-121">operations</span><span class="sxs-lookup"><span data-stu-id="92f8b-121">operations</span></span>|<span data-ttu-id="92f8b-122">[Operation](onenoteoperation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="92f8b-122">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="92f8b-123">OneNote の操作の状態です。</span><span class="sxs-lookup"><span data-stu-id="92f8b-123">The status of OneNote operations.</span></span> <span data-ttu-id="92f8b-124">操作のコレクションを取得することはサポートされていませんが、応答で `Operation-Location` ヘッダーが返される場合には長時間実行処理の状態を取得できます。</span><span class="sxs-lookup"><span data-stu-id="92f8b-124">Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response.</span></span> <span data-ttu-id="92f8b-125">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92f8b-125">Read-only.</span></span> <span data-ttu-id="92f8b-126">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92f8b-126">Nullable.</span></span>|
|<span data-ttu-id="92f8b-127">ページ</span><span class="sxs-lookup"><span data-stu-id="92f8b-127">pages</span></span>|<span data-ttu-id="92f8b-128">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="92f8b-128">[Page](page.md) collection</span></span>|<span data-ttu-id="92f8b-129">ユーザーまたはグループが所有しているすべての OneNote ノートブックのページです。</span><span class="sxs-lookup"><span data-stu-id="92f8b-129">The pages in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="92f8b-130">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92f8b-130">Read-only.</span></span> <span data-ttu-id="92f8b-131">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92f8b-131">Nullable.</span></span>|
|<span data-ttu-id="92f8b-132">リソース</span><span class="sxs-lookup"><span data-stu-id="92f8b-132">resources</span></span>|<span data-ttu-id="92f8b-133">[リソース](resource.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="92f8b-133">[Resource](resource.md) collection</span></span> |<span data-ttu-id="92f8b-134">OneNote ページの画像リソースおよび他のファイル リソースです。</span><span class="sxs-lookup"><span data-stu-id="92f8b-134">The image and other file resources in OneNote pages.</span></span> <span data-ttu-id="92f8b-135">リソース コレクションを取得することはサポートされていませんが、[特定のリソースのバイナリ コンテンツを取得](resource.md)できます。</span><span class="sxs-lookup"><span data-stu-id="92f8b-135">Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md).</span></span> <span data-ttu-id="92f8b-136">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92f8b-136">Read-only.</span></span> <span data-ttu-id="92f8b-137">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92f8b-137">Nullable.</span></span>|
|<span data-ttu-id="92f8b-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="92f8b-138">sectionGroups</span></span>|<span data-ttu-id="92f8b-139">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="92f8b-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="92f8b-140">ユーザーまたはグループが所有しているすべての OneNote ノートブックのセクション グループです。</span><span class="sxs-lookup"><span data-stu-id="92f8b-140">The section groups in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="92f8b-141">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92f8b-141">Read-only.</span></span> <span data-ttu-id="92f8b-142">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92f8b-142">Nullable.</span></span>|
|<span data-ttu-id="92f8b-143">セクション</span><span class="sxs-lookup"><span data-stu-id="92f8b-143">sections</span></span>|<span data-ttu-id="92f8b-144">[Section](section.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="92f8b-144">[Section](section.md) collection</span></span>|<span data-ttu-id="92f8b-145">ユーザーまたはグループが所有しているすべての OneNote ノートブック内のセクションです。</span><span class="sxs-lookup"><span data-stu-id="92f8b-145">The sections in all OneNote notebooks that are owned by the user or group.</span></span>  <span data-ttu-id="92f8b-146">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="92f8b-146">Read-only.</span></span> <span data-ttu-id="92f8b-147">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="92f8b-147">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="92f8b-148">メソッド</span><span class="sxs-lookup"><span data-stu-id="92f8b-148">Methods</span></span>

| <span data-ttu-id="92f8b-149">メソッド</span><span class="sxs-lookup"><span data-stu-id="92f8b-149">Method</span></span>           | <span data-ttu-id="92f8b-150">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="92f8b-150">Return Type</span></span>    |<span data-ttu-id="92f8b-151">説明</span><span class="sxs-lookup"><span data-stu-id="92f8b-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="92f8b-152">Create notebook</span><span class="sxs-lookup"><span data-stu-id="92f8b-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="92f8b-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="92f8b-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="92f8b-154">ノートブックのコレクションに投稿してノートブックを作成します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="92f8b-155">List notebooks</span><span class="sxs-lookup"><span data-stu-id="92f8b-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="92f8b-156">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="92f8b-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="92f8b-157">ノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="92f8b-158">Create page</span><span class="sxs-lookup"><span data-stu-id="92f8b-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="92f8b-159">Page</span><span class="sxs-lookup"><span data-stu-id="92f8b-159">Page</span></span>](page.md)| <span data-ttu-id="92f8b-160">ページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="92f8b-161">List pages</span><span class="sxs-lookup"><span data-stu-id="92f8b-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="92f8b-162">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="92f8b-162">[Page](page.md) collection</span></span>| <span data-ttu-id="92f8b-163">ページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="92f8b-164">List section groups</span><span class="sxs-lookup"><span data-stu-id="92f8b-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="92f8b-165">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="92f8b-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="92f8b-166">セクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="92f8b-167">List sections</span><span class="sxs-lookup"><span data-stu-id="92f8b-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="92f8b-168">[Section](section.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="92f8b-168">[Section](section.md) collection</span></span>| <span data-ttu-id="92f8b-169">セクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="92f8b-169">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
