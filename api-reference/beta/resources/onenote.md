---
title: OneNote リソースの種類
description: OneNote リソースのエントリ ポイントです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 2b6818ac5f9bd9bdc60d1c0d1e0cc8f80afc1f65
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970669"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="b68eb-103">OneNote リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b68eb-103">onenote resource type</span></span>

> <span data-ttu-id="b68eb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b68eb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b68eb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b68eb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b68eb-106">OneNote リソースのエントリ ポイントです。</span><span class="sxs-lookup"><span data-stu-id="b68eb-106">The entry point for OneNote resources.</span></span>

<span data-ttu-id="b68eb-107">Microsoft Graph API を介しての OneNote サービスに対する呼び出しすべては、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-107">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="b68eb-108">場所には、Office 365 またはコンシューマー OneDrive 上のユーザーのノートブック、ノートブックのグループ、または Office 365 で SharePoint サイトでホストされているチームのノートブックを指定できます。</span><span class="sxs-lookup"><span data-stu-id="b68eb-108">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="b68eb-109">**ユーザー ノートブック** コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-109">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="b68eb-110">**グループ ノートブック** グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-110">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="b68eb-111">**SharePoint サイト ノートブック** SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-111">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="b68eb-112">承認</span><span class="sxs-lookup"><span data-stu-id="b68eb-112">Authorization</span></span>

<span data-ttu-id="b68eb-113">OneNote API で動作するために必要なアクセス許可については、「[メモのアクセス許可](/graph/permissions-reference#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b68eb-113">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="b68eb-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b68eb-114">Relationships</span></span>
| <span data-ttu-id="b68eb-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b68eb-115">Relationship</span></span> | <span data-ttu-id="b68eb-116">型</span><span class="sxs-lookup"><span data-stu-id="b68eb-116">Type</span></span>   |<span data-ttu-id="b68eb-117">説明</span><span class="sxs-lookup"><span data-stu-id="b68eb-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b68eb-118">notebooks</span><span class="sxs-lookup"><span data-stu-id="b68eb-118">notebooks</span></span>|<span data-ttu-id="b68eb-119">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-119">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="b68eb-p102">ユーザーまたはグループが所有している OneNote ノートブックのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b68eb-p102">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b68eb-123">operations</span><span class="sxs-lookup"><span data-stu-id="b68eb-123">operations</span></span>|<span data-ttu-id="b68eb-124">[Operation](onenoteoperation.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-124">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="b68eb-p103">OneNote の操作の状態です。操作のコレクションを取得することはサポートされていませんが、応答で `Operation-Location` ヘッダーが返される場合には長時間実行処理の状態を取得できます。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b68eb-p103">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="b68eb-129">pages</span><span class="sxs-lookup"><span data-stu-id="b68eb-129">pages</span></span>|<span data-ttu-id="b68eb-130">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-130">[Page](page.md) collection</span></span>|<span data-ttu-id="b68eb-p104">ユーザーまたはグループが所有しているすべての OneNote ノートブックのページです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b68eb-p104">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="b68eb-134">resources</span><span class="sxs-lookup"><span data-stu-id="b68eb-134">resources</span></span>|<span data-ttu-id="b68eb-135">[Resource](resource.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-135">[Resource](resource.md) collection</span></span> |<span data-ttu-id="b68eb-p105">OneNote ページの画像リソースおよび他のファイル リソースです。リソース コレクションを取得することはサポートされていませんが、[特定のリソースのバイナリ コンテンツを取得](resource.md)できます。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b68eb-p105">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="b68eb-140">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="b68eb-140">sectionGroups</span></span>|<span data-ttu-id="b68eb-141">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-141">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="b68eb-p106">ユーザーまたはグループが所有しているすべての OneNote ノートブックのセクション グループです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b68eb-p106">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="b68eb-145">sections</span><span class="sxs-lookup"><span data-stu-id="b68eb-145">sections</span></span>|<span data-ttu-id="b68eb-146">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-146">[Section](section.md) collection</span></span>|<span data-ttu-id="b68eb-p107">ユーザーまたはグループが所有しているすべての OneNote ノートブック内のセクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b68eb-p107">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="b68eb-150">メソッド</span><span class="sxs-lookup"><span data-stu-id="b68eb-150">Methods</span></span>

| <span data-ttu-id="b68eb-151">メソッド</span><span class="sxs-lookup"><span data-stu-id="b68eb-151">Method</span></span>           | <span data-ttu-id="b68eb-152">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b68eb-152">Return Type</span></span>    |<span data-ttu-id="b68eb-153">説明</span><span class="sxs-lookup"><span data-stu-id="b68eb-153">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b68eb-154">Create notebook</span><span class="sxs-lookup"><span data-stu-id="b68eb-154">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="b68eb-155">Notebook</span><span class="sxs-lookup"><span data-stu-id="b68eb-155">Notebook</span></span>](notebook.md)| <span data-ttu-id="b68eb-156">ノートブックのコレクションに投稿してノートブックを作成します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-156">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="b68eb-157">List notebooks</span><span class="sxs-lookup"><span data-stu-id="b68eb-157">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="b68eb-158">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-158">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="b68eb-159">ノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-159">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="b68eb-160">Create page</span><span class="sxs-lookup"><span data-stu-id="b68eb-160">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="b68eb-161">Page</span><span class="sxs-lookup"><span data-stu-id="b68eb-161">Page</span></span>](page.md)| <span data-ttu-id="b68eb-162">ページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-162">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="b68eb-163">List pages</span><span class="sxs-lookup"><span data-stu-id="b68eb-163">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="b68eb-164">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-164">[Page](page.md) collection</span></span>| <span data-ttu-id="b68eb-165">ページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-165">Get a collection of pages.</span></span>|
|[<span data-ttu-id="b68eb-166">List section groups</span><span class="sxs-lookup"><span data-stu-id="b68eb-166">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="b68eb-167">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-167">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="b68eb-168">セクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-168">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="b68eb-169">List sections</span><span class="sxs-lookup"><span data-stu-id="b68eb-169">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="b68eb-170">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="b68eb-170">[Section](section.md) collection</span></span>| <span data-ttu-id="b68eb-171">セクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="b68eb-171">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
