# <a name="recentnotebook-resource-type"></a><span data-ttu-id="620de-101">recentNotebook リソース型</span><span class="sxs-lookup"><span data-stu-id="620de-101">recentNotebook resource type</span></span>

<span data-ttu-id="620de-102">最近アクセスした OneNote ノートブック。</span><span class="sxs-lookup"><span data-stu-id="620de-102">A recently accessed OneNote notebook.</span></span> <span data-ttu-id="620de-103">**recentNotebook** は、[notebook](notebook.md) と類似していますが、より少ないプロパティを持ちます。</span><span class="sxs-lookup"><span data-stu-id="620de-103">A **recentNotebook** is similar to a [notebook](notebook.md) but has fewer properties.</span></span>

## <a name="properties"></a><span data-ttu-id="620de-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="620de-104">Properties</span></span>
| <span data-ttu-id="620de-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="620de-105">Property</span></span>     | <span data-ttu-id="620de-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="620de-106">Type</span></span>   |<span data-ttu-id="620de-107">説明</span><span class="sxs-lookup"><span data-stu-id="620de-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="620de-108">displayName</span><span class="sxs-lookup"><span data-stu-id="620de-108">displayName</span></span>|<span data-ttu-id="620de-109">文字列</span><span class="sxs-lookup"><span data-stu-id="620de-109">String</span></span>|<span data-ttu-id="620de-110">ノートブックの名前。</span><span class="sxs-lookup"><span data-stu-id="620de-110">The name of the notebook.</span></span>|
|<span data-ttu-id="620de-111">lastAccessedTime</span><span class="sxs-lookup"><span data-stu-id="620de-111">lastAccessedTime</span></span>|<span data-ttu-id="620de-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="620de-112">DateTimeOffset</span></span>|<span data-ttu-id="620de-p102">ノートブックが最後に変更された日時。Timestamp は、ISO 8601 形式を使用した日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="620de-p102">The date and time when the notebook was last modified. The timestamp represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`. Read-only.</span></span>|
|<span data-ttu-id="620de-117">リンク</span><span class="sxs-lookup"><span data-stu-id="620de-117">links</span></span>|[<span data-ttu-id="620de-118">recentNotebookLinks</span><span class="sxs-lookup"><span data-stu-id="620de-118">recentNotebookLinks</span></span>](recentnotebooklinks.md)|<span data-ttu-id="620de-119">ノートブックを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="620de-119">Links for opening the notebook.</span></span> <span data-ttu-id="620de-120">リンクは、OneNote クライアントでノートブックを開きます (インストールされている場合)。`oneNoteClientURL`</span><span class="sxs-lookup"><span data-stu-id="620de-120">The `oneNoteClientURL` link opens the notebook in the OneNote client, if it's installed.</span></span> <span data-ttu-id="620de-121">リンクは、OneNote Online でノートブックを開きます。`oneNoteWebURL`</span><span class="sxs-lookup"><span data-stu-id="620de-121">The `oneNoteWebURL` link opens the notebook in OneNote Online.</span></span>|
|<span data-ttu-id="620de-122">sourceService</span><span class="sxs-lookup"><span data-stu-id="620de-122">sourceService</span></span>|<span data-ttu-id="620de-123">onenoteSourceService</span><span class="sxs-lookup"><span data-stu-id="620de-123">onenoteSourceService values</span></span>|<span data-ttu-id="620de-124">ノートブックが存在するバックエンド ストア (`OneDriveForBusiness` または `OneDrive` のいずれか)。</span><span class="sxs-lookup"><span data-stu-id="620de-124">The backend store where the Notebook resides, either `OneDriveForBusiness` or `OneDrive`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="620de-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="620de-125">JSON representation</span></span>

<span data-ttu-id="620de-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="620de-126">The following is a JSON representation of the resource.</span></span>

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

## <a name="methods"></a><span data-ttu-id="620de-127">メソッド</span><span class="sxs-lookup"><span data-stu-id="620de-127">Methods</span></span>

| <span data-ttu-id="620de-128">メソッド</span><span class="sxs-lookup"><span data-stu-id="620de-128">Method</span></span>           | <span data-ttu-id="620de-129">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="620de-129">Return Type</span></span>    |<span data-ttu-id="620de-130">説明</span><span class="sxs-lookup"><span data-stu-id="620de-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="620de-131">getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="620de-131">getRecentNotebooks</span></span>](../api/notebook_getrecentnotebooks.md) | <span data-ttu-id="620de-132">[ノートブック](notebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="620de-132">[notebook](notebook.md) collection</span></span> | <span data-ttu-id="620de-133">ユーザーの最近アクセスしたノートブックのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="620de-133">Get a collection of the most recently accessed notebooks for the user.</span></span> |
