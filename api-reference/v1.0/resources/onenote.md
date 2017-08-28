# <a name="onenote-resource-type"></a><span data-ttu-id="4fd4b-101">OneNote リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4fd4b-101">onenote resource type</span></span>

<span data-ttu-id="4fd4b-102">OneNote リソースのエントリ ポイントです。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-102">The entry point for OneNote resources.</span></span>

<span data-ttu-id="4fd4b-103">Microsoft Graph API を介しての OneNote サービスに対する呼び出しすべては、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-103">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="4fd4b-104">Office 365 またはコンシューマー OneDrive のユーザー ノートブック、Office 365 のグループ ノートブック、または SharePoint サイトでホストされているチームのノートブックを場所として指定できます。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-104">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="4fd4b-105">**ユーザー ノートブック** コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-105">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="4fd4b-106">**グループ ノートブック** グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-106">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="4fd4b-107">**SharePoint サイト ノートブック** SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-107">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="4fd4b-108">承認</span><span class="sxs-lookup"><span data-stu-id="4fd4b-108">Authorization</span></span>

<span data-ttu-id="4fd4b-109">OneNote API で動作するために必要なアクセス許可については、「[メモのアクセス許可](../../../concepts/permissions_reference.md#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-109">For information about the permissions required to work with OneNote APIs, see [Notes permissions](../../../concepts/permissions_reference.md#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="4fd4b-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fd4b-110">Relationships</span></span>
| <span data-ttu-id="4fd4b-111">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4fd4b-111">Relationship</span></span> | <span data-ttu-id="4fd4b-112">型</span><span class="sxs-lookup"><span data-stu-id="4fd4b-112">Type</span></span>   |<span data-ttu-id="4fd4b-113">説明</span><span class="sxs-lookup"><span data-stu-id="4fd4b-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4fd4b-114">notebooks</span><span class="sxs-lookup"><span data-stu-id="4fd4b-114">notebooks</span></span>|<span data-ttu-id="4fd4b-115">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-115">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="4fd4b-p101">ユーザーまたはグループが所有している OneNote ノートブックのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="4fd4b-119">operations</span><span class="sxs-lookup"><span data-stu-id="4fd4b-119">operations</span></span>|<span data-ttu-id="4fd4b-120">[Operation](onenoteoperation.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-120">[Operation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="4fd4b-p102">OneNote の操作の状態です。操作のコレクションを取得することはサポートされていませんが、応答で `Operation-Location` ヘッダーが返される場合には長時間実行処理の状態を取得できます。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="4fd4b-125">pages</span><span class="sxs-lookup"><span data-stu-id="4fd4b-125">pages</span></span>|<span data-ttu-id="4fd4b-126">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-126">[Page](page.md) collection</span></span>|<span data-ttu-id="4fd4b-p103">ユーザーまたはグループが所有しているすべての OneNote ノートブックのページです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="4fd4b-130">リソース</span><span class="sxs-lookup"><span data-stu-id="4fd4b-130">resources</span></span>|<span data-ttu-id="4fd4b-131">[Resource](resource.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-131">[Resource](resource.md) collection</span></span> |<span data-ttu-id="4fd4b-p104">OneNote ページの画像リソースおよび他のファイル リソースです。リソース コレクションを取得することはサポートされていませんが、[特定のリソースのバイナリ コンテンツを取得](resource.md)できます。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="4fd4b-136">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="4fd4b-136">sectionGroups</span></span>|<span data-ttu-id="4fd4b-137">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-137">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="4fd4b-p105">ユーザーまたはグループが所有しているすべての OneNote ノートブックのセクション グループです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="4fd4b-141">セクション</span><span class="sxs-lookup"><span data-stu-id="4fd4b-141">sections</span></span>|<span data-ttu-id="4fd4b-142">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-142">[Section](section.md) collection</span></span>|<span data-ttu-id="4fd4b-p106">ユーザーまたはグループが所有しているすべての OneNote ノートブック内のセクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="4fd4b-146">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fd4b-146">Methods</span></span>

| <span data-ttu-id="4fd4b-147">メソッド</span><span class="sxs-lookup"><span data-stu-id="4fd4b-147">Method</span></span>           | <span data-ttu-id="4fd4b-148">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4fd4b-148">Return Type</span></span>    |<span data-ttu-id="4fd4b-149">説明</span><span class="sxs-lookup"><span data-stu-id="4fd4b-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4fd4b-150">Create notebook</span><span class="sxs-lookup"><span data-stu-id="4fd4b-150">Create notebook</span></span>](../api/onenote_post_notebooks.md) |[<span data-ttu-id="4fd4b-151">Notebook</span><span class="sxs-lookup"><span data-stu-id="4fd4b-151">Notebook</span></span>](notebook.md)| <span data-ttu-id="4fd4b-152">ノートブックのコレクションに投稿してノートブックを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-152">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="4fd4b-153">List notebooks</span><span class="sxs-lookup"><span data-stu-id="4fd4b-153">List notebooks</span></span>](../api/onenote_list_notebooks.md) |<span data-ttu-id="4fd4b-154">[Notebook](notebook.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-154">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="4fd4b-155">ノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-155">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="4fd4b-156">Create page</span><span class="sxs-lookup"><span data-stu-id="4fd4b-156">Create page</span></span>](../api/onenote_post_pages.md) |[<span data-ttu-id="4fd4b-157">Page</span><span class="sxs-lookup"><span data-stu-id="4fd4b-157">Page</span></span>](page.md)| <span data-ttu-id="4fd4b-158">ページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-158">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="4fd4b-159">List pages</span><span class="sxs-lookup"><span data-stu-id="4fd4b-159">List pages</span></span>](../api/onenote_list_pages.md) |<span data-ttu-id="4fd4b-160">[Page](page.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-160">[Page](page.md) collection</span></span>| <span data-ttu-id="4fd4b-161">ページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-161">Get a collection of pages.</span></span>|
|[<span data-ttu-id="4fd4b-162">List section groups</span><span class="sxs-lookup"><span data-stu-id="4fd4b-162">List section groups</span></span>](../api/onenote_list_sectiongroups.md) |<span data-ttu-id="4fd4b-163">[SectionGroup](sectiongroup.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-163">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="4fd4b-164">セクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-164">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="4fd4b-165">List sections</span><span class="sxs-lookup"><span data-stu-id="4fd4b-165">List sections</span></span>](../api/onenote_list_sections.md) |<span data-ttu-id="4fd4b-166">[Section](section.md) collection</span><span class="sxs-lookup"><span data-stu-id="4fd4b-166">[Section](section.md) collection</span></span>| <span data-ttu-id="4fd4b-167">セクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="4fd4b-167">Get a collection of sections.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
