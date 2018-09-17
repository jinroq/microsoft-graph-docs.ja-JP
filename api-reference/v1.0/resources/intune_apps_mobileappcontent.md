# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="baa45-101">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="baa45-101">mobileAppContent resource type</span></span>

> <span data-ttu-id="baa45-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="baa45-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="baa45-103">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="baa45-103">Contains content properties for a specific app version.</span></span> <span data-ttu-id="baa45-104">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="baa45-104">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="baa45-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="baa45-105">Methods</span></span>
|<span data-ttu-id="baa45-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="baa45-106">Method</span></span>|<span data-ttu-id="baa45-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="baa45-107">Return Type</span></span>|<span data-ttu-id="baa45-108">説明</span><span class="sxs-lookup"><span data-stu-id="baa45-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="baa45-109">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="baa45-109">List mobileAppContents</span></span>](../api/intune_apps_mobileappcontent_list.md)|<span data-ttu-id="baa45-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="baa45-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) collection</span></span>|<span data-ttu-id="baa45-111">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="baa45-111">List properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="baa45-112">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="baa45-112">Get mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_get.md)|[<span data-ttu-id="baa45-113">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="baa45-113">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="baa45-114">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="baa45-114">Read properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="baa45-115">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="baa45-115">Create mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_create.md)|[<span data-ttu-id="baa45-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="baa45-116">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="baa45-117">新しい [mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="baa45-117">Create a new [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="baa45-118">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="baa45-118">Delete mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_delete.md)|<span data-ttu-id="baa45-119">なし</span><span class="sxs-lookup"><span data-stu-id="baa45-119">None</span></span>|<span data-ttu-id="baa45-120">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="baa45-120">Deletes a [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span></span>|
|[<span data-ttu-id="baa45-121">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="baa45-121">Update mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_update.md)|[<span data-ttu-id="baa45-122">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="baa45-122">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="baa45-123">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="baa45-123">Update the properties of a [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="baa45-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="baa45-124">Properties</span></span>
|<span data-ttu-id="baa45-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="baa45-125">Property</span></span>|<span data-ttu-id="baa45-126">タイプ</span><span class="sxs-lookup"><span data-stu-id="baa45-126">Type</span></span>|<span data-ttu-id="baa45-127">説明</span><span class="sxs-lookup"><span data-stu-id="baa45-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baa45-128">ID</span><span class="sxs-lookup"><span data-stu-id="baa45-128">id</span></span>|<span data-ttu-id="baa45-129">文字列</span><span class="sxs-lookup"><span data-stu-id="baa45-129">String</span></span>|<span data-ttu-id="baa45-130">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="baa45-130">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="baa45-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="baa45-131">Relationships</span></span>
|<span data-ttu-id="baa45-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="baa45-132">Relationship</span></span>|<span data-ttu-id="baa45-133">型</span><span class="sxs-lookup"><span data-stu-id="baa45-133">Type</span></span>|<span data-ttu-id="baa45-134">説明</span><span class="sxs-lookup"><span data-stu-id="baa45-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baa45-135">ファイル</span><span class="sxs-lookup"><span data-stu-id="baa45-135">files</span></span>|<span data-ttu-id="baa45-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="baa45-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="baa45-137">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="baa45-137">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="baa45-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="baa45-138">JSON Representation</span></span>
<span data-ttu-id="baa45-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="baa45-139">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```








