# <a name="profilephoto-resource-type"></a><span data-ttu-id="853f9-101">profilePhoto リソースの種類</span><span class="sxs-lookup"><span data-stu-id="853f9-101">profilePhoto resource type</span></span>
<span data-ttu-id="853f9-p101">Exchange Online からアクセスされるユーザー、グループ、または Outlook の連絡先のプロフィール写真。base 64 でエンコードされていないバイナリ データです。</span><span class="sxs-lookup"><span data-stu-id="853f9-p101">A profile photo of a user, group or an Outlook contact accessed from Exchange Online. It's binary data not encoded in base-64.</span></span>

<span data-ttu-id="853f9-104">Exchange Online 上でサポートされている HD Photo のサイズは次のとおりです。'48x48'、'64x64'、'96x96'、'120x120'、'240x240'、'360x360'、'432x432'、'504x504'、'648x648'。</span><span class="sxs-lookup"><span data-stu-id="853f9-104">The supported sizes of HD photos on Exchange Online are as follows: '48x48', '64x64', '96x96', '120x120', '240x240', '360x360','432x432', '504x504', and '648x648'.</span></span> 

## <a name="methods"></a><span data-ttu-id="853f9-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="853f9-105">Methods</span></span>

| <span data-ttu-id="853f9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="853f9-106">Method</span></span>       | <span data-ttu-id="853f9-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="853f9-107">Return Type</span></span>  |<span data-ttu-id="853f9-108">説明</span><span class="sxs-lookup"><span data-stu-id="853f9-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="853f9-109">ProfilePhoto を取得する</span><span class="sxs-lookup"><span data-stu-id="853f9-109">Get profilePhoto</span></span>](../api/profilephoto_get.md) | [<span data-ttu-id="853f9-110">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="853f9-110">profilePhoto</span></span>](profilephoto.md) |<span data-ttu-id="853f9-111">指定した **profilePhoto** またはそのメタデータ (profilePhoto プロパティ) を取得します。</span><span class="sxs-lookup"><span data-stu-id="853f9-111">Get the specified **profilePhoto** or its metadata (profilePhoto properties).</span></span>|
|[<span data-ttu-id="853f9-112">更新</span><span class="sxs-lookup"><span data-stu-id="853f9-112">Update</span></span>](../api/profilephoto_update.md) | [<span data-ttu-id="853f9-113">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="853f9-113">profilePhoto</span></span>](profilephoto.md)  |<span data-ttu-id="853f9-p102">指定されたユーザー、グループ、または連絡先に写真を割り当てます。写真はバイナリ形式にする必要があります。既存の写真が置き換えられます (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="853f9-p102">Assign a photo to the specified user, group, or contact. The photo should be in binary. It replaces the existing photo, if any.</span></span>|

## <a name="properties"></a><span data-ttu-id="853f9-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="853f9-117">Properties</span></span>
| <span data-ttu-id="853f9-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="853f9-118">Property</span></span>     | <span data-ttu-id="853f9-119">タイプ</span><span class="sxs-lookup"><span data-stu-id="853f9-119">Type</span></span>   |<span data-ttu-id="853f9-120">説明</span><span class="sxs-lookup"><span data-stu-id="853f9-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="853f9-121">ID</span><span class="sxs-lookup"><span data-stu-id="853f9-121">id</span></span>|<span data-ttu-id="853f9-122">文字列</span><span class="sxs-lookup"><span data-stu-id="853f9-122">string</span></span>|<span data-ttu-id="853f9-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="853f9-123">Read-only.</span></span>|
|<span data-ttu-id="853f9-124">height</span><span class="sxs-lookup"><span data-stu-id="853f9-124">height</span></span>|<span data-ttu-id="853f9-125">int32</span><span class="sxs-lookup"><span data-stu-id="853f9-125">int32</span></span>|<span data-ttu-id="853f9-p103">写真の高さ。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="853f9-p103">The height of the photo. Read-only.</span></span>|
|<span data-ttu-id="853f9-128">width</span><span class="sxs-lookup"><span data-stu-id="853f9-128">width</span></span>|<span data-ttu-id="853f9-129">int32</span><span class="sxs-lookup"><span data-stu-id="853f9-129">int32</span></span>|<span data-ttu-id="853f9-p104">写真の幅。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="853f9-p104">The width of the photo. Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="853f9-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="853f9-132">Relationships</span></span>
<span data-ttu-id="853f9-133">なし</span><span class="sxs-lookup"><span data-stu-id="853f9-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="853f9-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="853f9-134">JSON representation</span></span>

<span data-ttu-id="853f9-135">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="853f9-135">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "isMediaEntity": true,
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.profilePhoto"
}-->

```json
{
  "id": "240X240",
  "height": 240,
  "width": 240
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profilePhoto resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
