# <a name="educationroot-resource-type"></a><span data-ttu-id="0ffe6-101">educationRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0ffe6-101">educationRoot resource type</span></span>

<span data-ttu-id="0ffe6-102">名前空間は、教育機関に固有の機能を公開します。`/education`</span><span class="sxs-lookup"><span data-stu-id="0ffe6-102">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="0ffe6-103">名前空間の一部のオブジェクトは、Microsoft Graph の別の部分 (たとえば、[users](user.md)) にあります。`/education`</span><span class="sxs-lookup"><span data-stu-id="0ffe6-103">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="0ffe6-104">教育機関の名前空間は、これらのオブジェクトに教育機関固有のプロパティと機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-104">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="0ffe6-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0ffe6-105">Methods</span></span>

| <span data-ttu-id="0ffe6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0ffe6-106">Method</span></span>           | <span data-ttu-id="0ffe6-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0ffe6-107">Return Type</span></span>    |<span data-ttu-id="0ffe6-108">説明</span><span class="sxs-lookup"><span data-stu-id="0ffe6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0ffe6-109">educationClass を作成</span><span class="sxs-lookup"><span data-stu-id="0ffe6-109">Create educationClass</span></span>](../api/educationroot_post_classes.md) |[<span data-ttu-id="0ffe6-110">educationClass</span><span class="sxs-lookup"><span data-stu-id="0ffe6-110">educationClass</span></span>](educationclass.md)| <span data-ttu-id="0ffe6-111">クラス コレクションに投稿して、新しい **educationClass** を作成します。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-111">Create a new **educationClass** by posting to the classes collection.</span></span>|
|[<span data-ttu-id="0ffe6-112">classes をリスト</span><span class="sxs-lookup"><span data-stu-id="0ffe6-112">List classes</span></span>](../api/educationroot_list_classes.md) |<span data-ttu-id="0ffe6-113">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0ffe6-113">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="0ffe6-114">**educationClass** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-114">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="0ffe6-115">educationSchool を作成</span><span class="sxs-lookup"><span data-stu-id="0ffe6-115">Create educationSchool</span></span>](../api/educationroot_post_schools.md) |[<span data-ttu-id="0ffe6-116">educationSchool</span><span class="sxs-lookup"><span data-stu-id="0ffe6-116">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="0ffe6-117">学校コレクションに投稿して、新しい **educationSchool** を作成します。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-117">Create a new **educationSchool** by posting to the schools collection.</span></span>|
|[<span data-ttu-id="0ffe6-118">schools をリスト</span><span class="sxs-lookup"><span data-stu-id="0ffe6-118">List schools</span></span>](../api/educationroot_list_schools.md) |<span data-ttu-id="0ffe6-119">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0ffe6-119">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="0ffe6-120">**educationSchool** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-120">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="0ffe6-121">educationUser を作成</span><span class="sxs-lookup"><span data-stu-id="0ffe6-121">Create educationUser</span></span>](../api/educationroot_post_users.md) |[<span data-ttu-id="0ffe6-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="0ffe6-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="0ffe6-123">ユーザー コレクションに投稿して、新しい **educationUser** を作成します。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-123">Create a new **educationUser** by posting to the users collection.</span></span>|
|[<span data-ttu-id="0ffe6-124">user をリスト</span><span class="sxs-lookup"><span data-stu-id="0ffe6-124">List users</span></span>](../api/educationroot_list_users.md) |<span data-ttu-id="0ffe6-125">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0ffe6-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="0ffe6-126">**educationUser** オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-126">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="0ffe6-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ffe6-127">Properties</span></span>
<span data-ttu-id="0ffe6-128">なし</span><span class="sxs-lookup"><span data-stu-id="0ffe6-128">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="0ffe6-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0ffe6-129">Relationships</span></span>
| <span data-ttu-id="0ffe6-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0ffe6-130">Relationship</span></span> | <span data-ttu-id="0ffe6-131">型</span><span class="sxs-lookup"><span data-stu-id="0ffe6-131">Type</span></span>   |<span data-ttu-id="0ffe6-132">説明</span><span class="sxs-lookup"><span data-stu-id="0ffe6-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ffe6-133">classes</span><span class="sxs-lookup"><span data-stu-id="0ffe6-133">classes</span></span>|<span data-ttu-id="0ffe6-134">[educationClass](educationclass.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0ffe6-134">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="0ffe6-p102">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="0ffe6-137">me</span><span class="sxs-lookup"><span data-stu-id="0ffe6-137">me</span></span>|[<span data-ttu-id="0ffe6-138">educationUser</span><span class="sxs-lookup"><span data-stu-id="0ffe6-138">educationUser</span></span>](educationuser.md)| <span data-ttu-id="0ffe6-p103">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="0ffe6-141">schools</span><span class="sxs-lookup"><span data-stu-id="0ffe6-141">schools</span></span>|<span data-ttu-id="0ffe6-142">[educationSchool](educationschool.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0ffe6-142">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="0ffe6-p104">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="0ffe6-145">users</span><span class="sxs-lookup"><span data-stu-id="0ffe6-145">users</span></span>|<span data-ttu-id="0ffe6-146">[educationUser](educationuser.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0ffe6-146">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="0ffe6-p105">読み取り専用。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-p105">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ffe6-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0ffe6-149">JSON representation</span></span>
<span data-ttu-id="0ffe6-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0ffe6-150">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.educationRoot"
}-->

```json
{
}
```

<!-- {
  "blockType": "request",
  "name": "get_education"
}-->
```http
GET https://graph.microsoft.com/v1.0/education
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->