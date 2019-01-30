---
title: OneNote リソースの種類
description: OneNote リソースのエントリ ポイントです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640099"
---
# <a name="onenote-resource-type"></a><span data-ttu-id="73389-103">OneNote リソースの種類</span><span class="sxs-lookup"><span data-stu-id="73389-103">onenote resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73389-104">OneNote リソースのエントリ ポイントです。</span><span class="sxs-lookup"><span data-stu-id="73389-104">The entry point for OneNote resources.</span></span>

<span data-ttu-id="73389-105">Microsoft Graph API を介しての OneNote サービスに対する呼び出しすべては、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="73389-105">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="73389-106">場所には、Office 365 またはコンシューマー OneDrive 上のユーザーのノートブック、ノートブックのグループ、または Office 365 で SharePoint サイトでホストされているチームのノートブックを指定できます。</span><span class="sxs-lookup"><span data-stu-id="73389-106">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks, or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="73389-107">**ユーザー ノートブック** コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="73389-107">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="73389-108">**グループ ノートブック** グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="73389-108">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="73389-109">**SharePoint サイト ノートブック** SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="73389-109">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a><span data-ttu-id="73389-110">承認</span><span class="sxs-lookup"><span data-stu-id="73389-110">Authorization</span></span>

<span data-ttu-id="73389-111">OneNote API で動作するために必要なアクセス許可については、「[メモのアクセス許可](/graph/permissions-reference#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73389-111">For information about the permissions required to work with OneNote APIs, see [Notes permissions](/graph/permissions-reference#notes-permissions).</span></span>

## <a name="relationships"></a><span data-ttu-id="73389-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="73389-112">Relationships</span></span>
| <span data-ttu-id="73389-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="73389-113">Relationship</span></span> | <span data-ttu-id="73389-114">型</span><span class="sxs-lookup"><span data-stu-id="73389-114">Type</span></span>   |<span data-ttu-id="73389-115">説明</span><span class="sxs-lookup"><span data-stu-id="73389-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73389-116">notebooks</span><span class="sxs-lookup"><span data-stu-id="73389-116">notebooks</span></span>|<span data-ttu-id="73389-117">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-117">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="73389-p101">ユーザーまたはグループが所有している OneNote ノートブックのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="73389-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="73389-121">operations</span><span class="sxs-lookup"><span data-stu-id="73389-121">operations</span></span>|<span data-ttu-id="73389-122">[Operation](onenoteoperation.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-122">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="73389-p102">OneNote の操作の状態です。操作のコレクションを取得することはサポートされていませんが、応答で `Operation-Location` ヘッダーが返される場合には長時間実行処理の状態を取得できます。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="73389-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="73389-127">pages</span><span class="sxs-lookup"><span data-stu-id="73389-127">pages</span></span>|<span data-ttu-id="73389-128">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-128">[Page](page.md) collection</span></span>|<span data-ttu-id="73389-p103">ユーザーまたはグループが所有しているすべての OneNote ノートブックのページです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="73389-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="73389-132">resources</span><span class="sxs-lookup"><span data-stu-id="73389-132">resources</span></span>|<span data-ttu-id="73389-133">[Resource](resource.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-133">[Resource](resource.md) collection</span></span> |<span data-ttu-id="73389-p104">OneNote ページの画像リソースおよび他のファイル リソースです。リソース コレクションを取得することはサポートされていませんが、[特定のリソースのバイナリ コンテンツを取得](resource.md)できます。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="73389-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="73389-138">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="73389-138">sectionGroups</span></span>|<span data-ttu-id="73389-139">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-139">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="73389-p105">ユーザーまたはグループが所有しているすべての OneNote ノートブックのセクション グループです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="73389-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="73389-143">sections</span><span class="sxs-lookup"><span data-stu-id="73389-143">sections</span></span>|<span data-ttu-id="73389-144">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-144">[Section](section.md) collection</span></span>|<span data-ttu-id="73389-p106">ユーザーまたはグループが所有しているすべての OneNote ノートブック内のセクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="73389-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="73389-148">メソッド</span><span class="sxs-lookup"><span data-stu-id="73389-148">Methods</span></span>

| <span data-ttu-id="73389-149">メソッド</span><span class="sxs-lookup"><span data-stu-id="73389-149">Method</span></span>           | <span data-ttu-id="73389-150">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="73389-150">Return Type</span></span>    |<span data-ttu-id="73389-151">説明</span><span class="sxs-lookup"><span data-stu-id="73389-151">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="73389-152">Create notebook</span><span class="sxs-lookup"><span data-stu-id="73389-152">Create notebook</span></span>](../api/onenote-post-notebooks.md) |[<span data-ttu-id="73389-153">Notebook</span><span class="sxs-lookup"><span data-stu-id="73389-153">Notebook</span></span>](notebook.md)| <span data-ttu-id="73389-154">ノートブックのコレクションに投稿してノートブックを作成します。</span><span class="sxs-lookup"><span data-stu-id="73389-154">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="73389-155">List notebooks</span><span class="sxs-lookup"><span data-stu-id="73389-155">List notebooks</span></span>](../api/onenote-list-notebooks.md) |<span data-ttu-id="73389-156">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-156">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="73389-157">ノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="73389-157">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="73389-158">Create page</span><span class="sxs-lookup"><span data-stu-id="73389-158">Create page</span></span>](../api/onenote-post-pages.md) |[<span data-ttu-id="73389-159">Page</span><span class="sxs-lookup"><span data-stu-id="73389-159">Page</span></span>](page.md)| <span data-ttu-id="73389-160">ページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="73389-160">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="73389-161">List pages</span><span class="sxs-lookup"><span data-stu-id="73389-161">List pages</span></span>](../api/onenote-list-pages.md) |<span data-ttu-id="73389-162">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-162">[Page](page.md) collection</span></span>| <span data-ttu-id="73389-163">ページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="73389-163">Get a collection of pages.</span></span>|
|[<span data-ttu-id="73389-164">List section groups</span><span class="sxs-lookup"><span data-stu-id="73389-164">List section groups</span></span>](../api/onenote-list-sectiongroups.md) |<span data-ttu-id="73389-165">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-165">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="73389-166">セクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="73389-166">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="73389-167">List sections</span><span class="sxs-lookup"><span data-stu-id="73389-167">List sections</span></span>](../api/onenote-list-sections.md) |<span data-ttu-id="73389-168">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="73389-168">[Section](section.md) collection</span></span>| <span data-ttu-id="73389-169">セクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="73389-169">Get a collection of sections.</span></span>|

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
