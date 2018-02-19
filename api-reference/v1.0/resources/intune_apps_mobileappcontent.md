# <a name="mobileappcontent-resource-type"></a><span data-ttu-id="93981-101">mobileAppContent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="93981-101">mobileAppContent resource type</span></span>

> <span data-ttu-id="93981-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="93981-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="93981-103">特定のアプリのバージョンに関するコンテンツのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="93981-103">Contains content properties for a specific app version.</span></span> <span data-ttu-id="93981-104">各 mobileAppContent には、複数の mobileAppContentFile を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="93981-104">Each mobileAppContent can have multiple mobileAppContentFile.</span></span>
## <a name="methods"></a><span data-ttu-id="93981-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="93981-105">Methods</span></span>
|<span data-ttu-id="93981-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="93981-106">Method</span></span>|<span data-ttu-id="93981-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="93981-107">Return Type</span></span>|<span data-ttu-id="93981-108">説明</span><span class="sxs-lookup"><span data-stu-id="93981-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="93981-109">mobileAppContents のリスト</span><span class="sxs-lookup"><span data-stu-id="93981-109">List mobileAppContents</span></span>](../api/intune_apps_mobileappcontent_list.md)|<span data-ttu-id="93981-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93981-110">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) collection</span></span>|<span data-ttu-id="93981-111">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="93981-111">List properties and relationships of the [mobileAppContent](../resources/intune_apps_mobileappcontent.md) objects.</span></span>|
|[<span data-ttu-id="93981-112">MobileAppContent の取得</span><span class="sxs-lookup"><span data-stu-id="93981-112">Get mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_get.md)|[<span data-ttu-id="93981-113">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="93981-113">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="93981-114">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="93981-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="93981-115">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="93981-115">Create mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_create.md)|[<span data-ttu-id="93981-116">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="93981-116">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="93981-117">新しい [mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="93981-117">Create a new [plannerBucket](../resources/intune_apps_mobileappcontent.md) object.</span></span>|
|[<span data-ttu-id="93981-118">mobileAppContent の削除</span><span class="sxs-lookup"><span data-stu-id="93981-118">Delete mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_delete.md)|<span data-ttu-id="93981-119">なし</span><span class="sxs-lookup"><span data-stu-id="93981-119">None</span></span>|<span data-ttu-id="93981-120">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="93981-120">Deletes a [mobileAppContent](../resources/intune_apps_mobileappcontent.md).</span></span>|
|[<span data-ttu-id="93981-121">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="93981-121">Update mobileAppContent</span></span>](../api/intune_apps_mobileappcontent_update.md)|[<span data-ttu-id="93981-122">mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="93981-122">mobileAppContent</span></span>](../resources/intune_apps_mobileappcontent.md)|<span data-ttu-id="93981-123">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="93981-123">Update the properties of a [calendar](../resources/intune_apps_mobileappcontent.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="93981-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93981-124">Properties</span></span>
|<span data-ttu-id="93981-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="93981-125">Property</span></span>|<span data-ttu-id="93981-126">型</span><span class="sxs-lookup"><span data-stu-id="93981-126">Type</span></span>|<span data-ttu-id="93981-127">説明</span><span class="sxs-lookup"><span data-stu-id="93981-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93981-128">id</span><span class="sxs-lookup"><span data-stu-id="93981-128">id</span></span>|<span data-ttu-id="93981-129">String</span><span class="sxs-lookup"><span data-stu-id="93981-129">String</span></span>|<span data-ttu-id="93981-130">アプリのコンテンツのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="93981-130">The app content version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93981-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93981-131">Relationships</span></span>
|<span data-ttu-id="93981-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="93981-132">Relationship</span></span>|<span data-ttu-id="93981-133">型</span><span class="sxs-lookup"><span data-stu-id="93981-133">Type</span></span>|<span data-ttu-id="93981-134">説明</span><span class="sxs-lookup"><span data-stu-id="93981-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93981-135">files</span><span class="sxs-lookup"><span data-stu-id="93981-135">files</span></span>|<span data-ttu-id="93981-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="93981-136">[mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) collection</span></span>|<span data-ttu-id="93981-137">このアプリのコンテンツのバージョンに関するファイルのリストです。</span><span class="sxs-lookup"><span data-stu-id="93981-137">The list of files for this app content version.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="93981-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="93981-138">JSON Representation</span></span>
<span data-ttu-id="93981-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="93981-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "String (identifier)"
}
```



