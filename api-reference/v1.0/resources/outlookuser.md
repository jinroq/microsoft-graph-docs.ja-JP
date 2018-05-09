# <a name="outlookuser-resource-type"></a><span data-ttu-id="1371c-101">outlookUser リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1371c-101">outlookUser resource type</span></span>


<span data-ttu-id="1371c-102">ユーザーが利用できる Outlook サービスを表します。</span><span class="sxs-lookup"><span data-stu-id="1371c-102">Represents the Outlook services available to a user.</span></span>


## <a name="methods"></a><span data-ttu-id="1371c-103">メソッド</span><span class="sxs-lookup"><span data-stu-id="1371c-103">Methods</span></span>

| <span data-ttu-id="1371c-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="1371c-104">Method</span></span>           | <span data-ttu-id="1371c-105">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1371c-105">Return Type</span></span>    |<span data-ttu-id="1371c-106">説明</span><span class="sxs-lookup"><span data-stu-id="1371c-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1371c-107">カテゴリの作成</span><span class="sxs-lookup"><span data-stu-id="1371c-107">Create category</span></span>](../api/outlookuser_post_mastercategories.md) | [<span data-ttu-id="1371c-108">outlookCategory</span><span class="sxs-lookup"><span data-stu-id="1371c-108">outlookCategory</span></span>](outlookcategory.md) |<span data-ttu-id="1371c-109">ユーザーのマスター カテゴリ リスト内に **outlookCategory** オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1371c-109">Create an **outlookCategory** object in the user's master list of categories.</span></span>|
|[<span data-ttu-id="1371c-110">カテゴリの一覧表示</span><span class="sxs-lookup"><span data-stu-id="1371c-110">List categories</span></span>](../api/outlookuser_list_mastercategories.md) | <span data-ttu-id="1371c-111">[outlookCategory](outlookcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1371c-111">[outlookCategory](outlookcategory.md) collection</span></span> |<span data-ttu-id="1371c-112">ユーザーに対して定義されているすべてのカテゴリを取得します。</span><span class="sxs-lookup"><span data-stu-id="1371c-112">Get all the categories that have been defined for the user.</span></span>|
|[<span data-ttu-id="1371c-113">supportedLanguages</span><span class="sxs-lookup"><span data-stu-id="1371c-113">supportedLanguages</span></span>](../api/outlookuser_supportedlanguages.md) | <span data-ttu-id="1371c-114">[localeInfo](localeinfo.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1371c-114">[localeInfo](localeinfo.md) collection</span></span> | <span data-ttu-id="1371c-115">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) ロケールと言語のリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1371c-115">Get the list of locales and languages that are supported for the user, as configured on the user's mailbox server.</span></span> |
|[<span data-ttu-id="1371c-116">supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="1371c-116">supportedTimeZones</span></span>](../api/outlookuser_supportedtimezones.md) | <span data-ttu-id="1371c-117">[timeZoneInformation](timezoneinformation.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1371c-117">[timeZoneInformation](timezoneinformation.md) collection</span></span> | <span data-ttu-id="1371c-118">ユーザーに対してサポートされている (ユーザーのメールボックス サーバーで構成されている) タイム ゾーンのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1371c-118">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span> |


## <a name="properties"></a><span data-ttu-id="1371c-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1371c-119">Properties</span></span>
<span data-ttu-id="1371c-120">なし</span><span class="sxs-lookup"><span data-stu-id="1371c-120">None</span></span>

## <a name="relationships"></a><span data-ttu-id="1371c-121">関係</span><span class="sxs-lookup"><span data-stu-id="1371c-121">Relationships</span></span>
| <span data-ttu-id="1371c-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1371c-122">Relationship</span></span> | <span data-ttu-id="1371c-123">型</span><span class="sxs-lookup"><span data-stu-id="1371c-123">Type</span></span>   |<span data-ttu-id="1371c-124">説明</span><span class="sxs-lookup"><span data-stu-id="1371c-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1371c-125">masterCategories</span><span class="sxs-lookup"><span data-stu-id="1371c-125">masterCategories</span></span>|<span data-ttu-id="1371c-126">[outlookCategory](../resources/outlookCategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1371c-126">[outlookCategory](../resources/outlookCategory.md) collection</span></span>| <span data-ttu-id="1371c-127">ユーザーに対して定義されているカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="1371c-127">A list of categories defined for the user.</span></span> | 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->