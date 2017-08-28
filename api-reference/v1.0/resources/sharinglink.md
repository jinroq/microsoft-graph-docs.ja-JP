# <a name="sharinglink-resource-type"></a><span data-ttu-id="d7b74-101">SharingLink リソースタイプ</span><span class="sxs-lookup"><span data-stu-id="d7b74-101">SharingLink resource type</span></span>

<span data-ttu-id="d7b74-102">**SharingLink** リソースは、リンク関連のデータ項目を 1 つの構造にグループ化します。</span><span class="sxs-lookup"><span data-stu-id="d7b74-102">The **SharingLink** resource groups link-related data items into a single structure.</span></span>

<span data-ttu-id="d7b74-103">[**Permission**](permission.md) リソースが非 null の **sharingLink** ファセットを持つ場合、アクセス許可は (ユーザーやグループに与えられているアクセス許可ではなく) 共有リンクを表します。</span><span class="sxs-lookup"><span data-stu-id="d7b74-103">If a [**Permission**](permission.md) resource has a non-null **sharingLink** facet, the permission represents a sharing link (as opposed to permissions granted to a person or group).</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7b74-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7b74-104">JSON representation</span></span>

<span data-ttu-id="d7b74-105">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d7b74-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "application", "scope" ],
  "@odata.type": "microsoft.graph.sharingLink"
}-->

```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "type": "view | edit",
  "scope": "anonymous | organization",
  "webUrl": "url"
}
```

## <a name="properties"></a><span data-ttu-id="d7b74-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7b74-106">Properties</span></span>

| <span data-ttu-id="d7b74-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7b74-107">Property</span></span>    | <span data-ttu-id="d7b74-108">型</span><span class="sxs-lookup"><span data-stu-id="d7b74-108">Type</span></span>                    | <span data-ttu-id="d7b74-109">説明</span><span class="sxs-lookup"><span data-stu-id="d7b74-109">Description</span></span>                                                                                                                                                                                             |
|:------------|:------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d7b74-110">application</span><span class="sxs-lookup"><span data-stu-id="d7b74-110">application</span></span> | [<span data-ttu-id="d7b74-111">identity</span><span class="sxs-lookup"><span data-stu-id="d7b74-111">identity</span></span>](identity.md) | <span data-ttu-id="d7b74-112">リンクが関連付けられているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="d7b74-112">The app the link is associated with.</span></span>                                                                                                                                                                    |
| <span data-ttu-id="d7b74-113">type</span><span class="sxs-lookup"><span data-stu-id="d7b74-113">type</span></span>        | <span data-ttu-id="d7b74-114">String</span><span class="sxs-lookup"><span data-stu-id="d7b74-114">String</span></span>                  | <span data-ttu-id="d7b74-115">作成されたリンクの種類。</span><span class="sxs-lookup"><span data-stu-id="d7b74-115">The type of the link created.</span></span>                                                                                                                                                                           |
| <span data-ttu-id="d7b74-116">scope</span><span class="sxs-lookup"><span data-stu-id="d7b74-116">scope</span></span>       | <span data-ttu-id="d7b74-117">String</span><span class="sxs-lookup"><span data-stu-id="d7b74-117">String</span></span>                  | <span data-ttu-id="d7b74-p101">このアクセス許可によって表されるリンクの範囲です。値 `anonymous` は、すべてのユーザーがリンクを使用できることを示し、`organization` は同じテナントにサインインしたユーザーのみがリンクを使用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="d7b74-p101">The scope of the link represented by this permission. Value `anonymous` indicates the link is usable by anyone, `organization` indicates the link is only usable for users signed into the same tenant.</span></span> |
| <span data-ttu-id="d7b74-120">webUrl</span><span class="sxs-lookup"><span data-stu-id="d7b74-120">webUrl</span></span>      | <span data-ttu-id="d7b74-121">String</span><span class="sxs-lookup"><span data-stu-id="d7b74-121">String</span></span>                  | <span data-ttu-id="d7b74-122">OneDrive の web サイト上で、項目をブラウザーに開く URL です。</span><span class="sxs-lookup"><span data-stu-id="d7b74-122">A URL that opens the item in the browser on the OneDrive website.</span></span>                                                                                                                                       |

## <a name="type-enumeration"></a><span data-ttu-id="d7b74-123">Type 列挙</span><span class="sxs-lookup"><span data-stu-id="d7b74-123">Type enumeration</span></span>

<span data-ttu-id="d7b74-124">この表は、**type** プロパティの可能な値を定義します。</span><span class="sxs-lookup"><span data-stu-id="d7b74-124">This table defines the possible values for the **type** property:</span></span>

| <span data-ttu-id="d7b74-125">値</span><span class="sxs-lookup"><span data-stu-id="d7b74-125">Value</span></span>   | <span data-ttu-id="d7b74-126">ロール</span><span class="sxs-lookup"><span data-stu-id="d7b74-126">Role</span></span>    | <span data-ttu-id="d7b74-127">説明</span><span class="sxs-lookup"><span data-stu-id="d7b74-127">Description</span></span>                                                                     |
|:--------|:--------|:--------------------------------------------------------------------------------|
| `view`  | `read`  | <span data-ttu-id="d7b74-128">読み取り専用のアクセスを許可する、閲覧専用の共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="d7b74-128">A view-only sharing link, allowing read-only access.</span></span>                            |
| `edit`  | `write` | <span data-ttu-id="d7b74-129">読み取り / 書き込みのアクセスを許可する、編集共有リンクです。</span><span class="sxs-lookup"><span data-stu-id="d7b74-129">An edit sharing link, allowing read-write access.</span></span>                               |

## <a name="scope-enumeration"></a><span data-ttu-id="d7b74-130">スコープ列挙</span><span class="sxs-lookup"><span data-stu-id="d7b74-130">Scope enumeration</span></span>

| <span data-ttu-id="d7b74-131">値</span><span class="sxs-lookup"><span data-stu-id="d7b74-131">Value</span></span>          | <span data-ttu-id="d7b74-132">説明</span><span class="sxs-lookup"><span data-stu-id="d7b74-132">Description</span></span>                                                                                                                 |
|:---------------|:----------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="d7b74-133">共有リンクは誰でも使用可能です。</span><span class="sxs-lookup"><span data-stu-id="d7b74-133">The sharing link is available for anyone to use.</span></span>                                                                            |
| `organization` | <span data-ttu-id="d7b74-p102">共有リンクは、同じ組織 (テナント) 内のすべてのユーザーが使用可能です。OneDrive Personal では使用できません。</span><span class="sxs-lookup"><span data-stu-id="d7b74-p102">The sharing link is available for anyone within the same organization (tenant) to use. Not available for OneDrive Personal.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sharingLink resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
