# <a name="onenote-resource-type"></a><span data-ttu-id="e6608-101">OneNote リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e6608-101">onenote resource type</span></span>

<span data-ttu-id="e6608-102">OneNote リソースのエントリ ポイントです。</span><span class="sxs-lookup"><span data-stu-id="e6608-102">The entry point for OneNote resources.</span></span>

<span data-ttu-id="e6608-103">Microsoft Graph API を介しての OneNote サービスに対する呼び出しすべては、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="e6608-103">All calls to the OneNote service through the Microsoft Graph API use this service root URL:</span></span>

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

<span data-ttu-id="e6608-104">Office 365 またはコンシューマー OneDrive のユーザー ノートブック、Office 365 のグループ ノートブック、または SharePoint サイトでホストされているチームのノートブックを場所として指定できます。</span><span class="sxs-lookup"><span data-stu-id="e6608-104">The location can be user notebooks on Office 365 or consumer OneDrive, group notebooks or SharePoint site-hosted team notebooks on Office 365.</span></span> 

<span data-ttu-id="e6608-105">**ユーザー ノートブック** コンシューマー OneDrive または OneDrive for Business の個人用ノートブックにアクセスするには、次の URL のいずれかを使用します。</span><span class="sxs-lookup"><span data-stu-id="e6608-105">**User notebooks** To access personal notebooks on consumer OneDrive or OneDrive for Business, use one of the following URLs:</span></span>

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

<span data-ttu-id="e6608-106">**グループ ノートブック** グループによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="e6608-106">**Group notebooks** To access notebooks that are owned by a group, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
<span data-ttu-id="e6608-107">**SharePoint サイト ノートブック** SharePoint チーム サイトによって所有されているノートブックにアクセスするには、次のサービス ルート URL を使用します。</span><span class="sxs-lookup"><span data-stu-id="e6608-107">**SharePoint site notebooks** To access notebooks that are owned by a SharePoint team site, use the following service root URL:</span></span>

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a><span data-ttu-id="e6608-108">承認</span><span class="sxs-lookup"><span data-stu-id="e6608-108">Authorization</span></span>

<span data-ttu-id="e6608-109">OneNote API で動作するために必要なアクセス許可については、「[メモのアクセス許可](../../../concepts/permissions_reference.md#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6608-109">For information about the permissions required to work with OneNote APIs, see [Notes permissions](../../../concepts/permissions_reference.md#notes-permissions).</span></span>


## <a name="relationships"></a><span data-ttu-id="e6608-110">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6608-110">Relationships</span></span>
| <span data-ttu-id="e6608-111">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e6608-111">Relationship</span></span> | <span data-ttu-id="e6608-112">型</span><span class="sxs-lookup"><span data-stu-id="e6608-112">Type</span></span>   |<span data-ttu-id="e6608-113">説明</span><span class="sxs-lookup"><span data-stu-id="e6608-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6608-114">ノートブック</span><span class="sxs-lookup"><span data-stu-id="e6608-114">notebooks</span></span>|<span data-ttu-id="e6608-115">[ノートブック](notebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-115">[Notebook](notebook.md) collection</span></span>|<span data-ttu-id="e6608-p101">ユーザーまたはグループが所有している OneNote ノートブックのコレクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e6608-p101">The collection of OneNote notebooks that are owned by the user or group. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e6608-119">操作</span><span class="sxs-lookup"><span data-stu-id="e6608-119">operations</span></span>|<span data-ttu-id="e6608-120">[OnenoteOperation](onenoteoperation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-120">[OnenoteOperation](onenoteoperation.md) collection</span></span> |<span data-ttu-id="e6608-p102">OneNote の操作の状態です。操作のコレクションを取得することはサポートされていませんが、応答で `Operation-Location` ヘッダーが返される場合には長時間実行処理の状態を取得できます。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e6608-p102">The status of OneNote operations. Getting an operations collection is not supported, but you can get the status of long-running operations if the `Operation-Location` header is returned in the response. Read-only. Nullable.</span></span>|
|<span data-ttu-id="e6608-125">ページ</span><span class="sxs-lookup"><span data-stu-id="e6608-125">pages</span></span>|<span data-ttu-id="e6608-126">[OnenotePage](page.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-126">[OnenotePage](page.md) collection</span></span>|<span data-ttu-id="e6608-p103">ユーザーまたはグループが所有しているすべての OneNote ノートブックのページです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e6608-p103">The pages in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="e6608-130">リソース</span><span class="sxs-lookup"><span data-stu-id="e6608-130">resources</span></span>|<span data-ttu-id="e6608-131">[OnenoteResource](resource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-131">[OnenoteResource](resource.md) collection</span></span> |<span data-ttu-id="e6608-p104">OneNote ページの画像リソースおよび他のファイル リソースです。リソース コレクションを取得することはサポートされていませんが、[特定のリソースのバイナリ コンテンツを取得](resource.md)できます。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e6608-p104">The image and other file resources in OneNote pages. Getting a resources collection is not supported, but you can [get the binary content of a specific resource](resource.md). Read-only. Nullable.</span></span>|
|<span data-ttu-id="e6608-136">sectionGroups</span><span class="sxs-lookup"><span data-stu-id="e6608-136">sectionGroups</span></span>|<span data-ttu-id="e6608-137">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-137">[SectionGroup](sectiongroup.md) collection</span></span>|<span data-ttu-id="e6608-p105">ユーザーまたはグループが所有しているすべての OneNote ノートブックのセクション グループです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e6608-p105">The section groups in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|
|<span data-ttu-id="e6608-141">セクション</span><span class="sxs-lookup"><span data-stu-id="e6608-141">sections</span></span>|<span data-ttu-id="e6608-142">[OnenoteSection](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-142">[OnenoteSection](section.md) collection</span></span>|<span data-ttu-id="e6608-p106">ユーザーまたはグループが所有しているすべての OneNote ノートブック内のセクションです。読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e6608-p106">The sections in all OneNote notebooks that are owned by the user or group.  Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="e6608-146">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6608-146">Methods</span></span>

| <span data-ttu-id="e6608-147">メソッド</span><span class="sxs-lookup"><span data-stu-id="e6608-147">Method</span></span>           | <span data-ttu-id="e6608-148">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e6608-148">Return Type</span></span>    |<span data-ttu-id="e6608-149">説明</span><span class="sxs-lookup"><span data-stu-id="e6608-149">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e6608-150">ノートブックを作成します。</span><span class="sxs-lookup"><span data-stu-id="e6608-150">Create notebook</span></span>](../api/onenote_post_notebooks.md) |[<span data-ttu-id="e6608-151">ノートブック</span><span class="sxs-lookup"><span data-stu-id="e6608-151">Notebook</span></span>](notebook.md)| <span data-ttu-id="e6608-152">ノートブックのコレクションに投稿してノートブックを作成します。</span><span class="sxs-lookup"><span data-stu-id="e6608-152">Create a notebook by posting to the notebooks collection.</span></span>|
|[<span data-ttu-id="e6608-153">ノートブックを一覧表示</span><span class="sxs-lookup"><span data-stu-id="e6608-153">List notebooks</span></span>](../api/onenote_list_notebooks.md) |<span data-ttu-id="e6608-154">[ノートブック](notebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-154">[Notebook](notebook.md) collection</span></span>| <span data-ttu-id="e6608-155">ノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e6608-155">Get a collection of notebooks.</span></span>|
|[<span data-ttu-id="e6608-156">ページを作成</span><span class="sxs-lookup"><span data-stu-id="e6608-156">Create page</span></span>](../api/onenote_post_pages.md) |[<span data-ttu-id="e6608-157">ページ</span><span class="sxs-lookup"><span data-stu-id="e6608-157">Page</span></span>](page.md)| <span data-ttu-id="e6608-158">ページのコレクションに投稿してページを作成します。</span><span class="sxs-lookup"><span data-stu-id="e6608-158">Create a page by posting to the pages collection.</span></span>|
|[<span data-ttu-id="e6608-159">ページをリスト</span><span class="sxs-lookup"><span data-stu-id="e6608-159">List pages</span></span>](../api/onenote_list_pages.md) |<span data-ttu-id="e6608-160">[ページ](page.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-160">[Page](page.md) collection</span></span>| <span data-ttu-id="e6608-161">ページのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e6608-161">Get a collection of pages.</span></span>|
|[<span data-ttu-id="e6608-162">セクション グループを一覧表示</span><span class="sxs-lookup"><span data-stu-id="e6608-162">List section groups</span></span>](../api/onenote_list_sectiongroups.md) |<span data-ttu-id="e6608-163">[SectionGroup](sectiongroup.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-163">[SectionGroup](sectiongroup.md) collection</span></span>| <span data-ttu-id="e6608-164">セクション グループのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e6608-164">Get a collection of section groups.</span></span>|
|[<span data-ttu-id="e6608-165">セクションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e6608-165">List sections</span></span>](../api/onenote_list_sections.md) |<span data-ttu-id="e6608-166">[OnenoteSection](section.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e6608-166">[OnenoteSection](section.md) collection</span></span>| <span data-ttu-id="e6608-167">セクションのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="e6608-167">Get a collection of sections.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e6608-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e6608-168">JSON Representation</span></span>
<span data-ttu-id="e6608-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e6608-169">Here is a JSON representation of the resource.</span></span>
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
