# <a name="devicecategory-resource-type"></a><span data-ttu-id="4a87f-101">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4a87f-101">deviceCategory resource type</span></span>

> <span data-ttu-id="4a87f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a87f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a87f-103">デバイス カテゴリは、デバイスを整理する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="4a87f-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="4a87f-104">デバイス カテゴリを使用して、会社の管理者は、自社にとって意味のある、独自のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="4a87f-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="4a87f-105">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="4a87f-105"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="4a87f-106">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="4a87f-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="4a87f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4a87f-107">Methods</span></span>
|<span data-ttu-id="4a87f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4a87f-108">Method</span></span>|<span data-ttu-id="4a87f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4a87f-109">Return Type</span></span>|<span data-ttu-id="4a87f-110">説明</span><span class="sxs-lookup"><span data-stu-id="4a87f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a87f-111">[リストの deviceCategories](../api/intune_shared_devicecategory_list.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4a87f-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) collection</span></span>|<span data-ttu-id="4a87f-112">[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4a87f-112">List properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="4a87f-113">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="4a87f-113">Get deviceCategory</span></span>](../api/intune_shared_devicecategory_get.md)|<span data-ttu-id="4a87f-114">[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4a87f-114">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="4a87f-115">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="4a87f-115">Create deviceCategory</span></span>](../api/intune_shared_devicecategory_create.md)|<span data-ttu-id="4a87f-116">新しい [deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4a87f-116">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|<span data-ttu-id="4a87f-117">[DeviceCategory を削除](../api/intune_shared_devicecategory_delete.md)します。</span><span class="sxs-lookup"><span data-stu-id="4a87f-117">[Delete deviceCategory](../api/intune_shared_devicecategory_delete.md).</span></span>|
|[<span data-ttu-id="4a87f-118">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="4a87f-118">Update deviceCategory</span></span>](../api/intune_shared_devicecategory_update.md)|<span data-ttu-id="4a87f-119">[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4a87f-119">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4a87f-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a87f-120">Properties</span></span>
|<span data-ttu-id="4a87f-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a87f-121">Property</span></span>|<span data-ttu-id="4a87f-122">型</span><span class="sxs-lookup"><span data-stu-id="4a87f-122">Type</span></span>|<span data-ttu-id="4a87f-123">説明</span><span class="sxs-lookup"><span data-stu-id="4a87f-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a87f-124">id</span><span class="sxs-lookup"><span data-stu-id="4a87f-124">id</span></span>|<span data-ttu-id="4a87f-125">文字列</span><span class="sxs-lookup"><span data-stu-id="4a87f-125">String</span></span>|<span data-ttu-id="4a87f-126">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4a87f-126">Unique identifier for the device category.</span></span> <span data-ttu-id="4a87f-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4a87f-127">Read-only.</span></span>|
|<span data-ttu-id="4a87f-128">**契約時**</span><span class="sxs-lookup"><span data-stu-id="4a87f-128">**Onboarding**</span></span>|
|<span data-ttu-id="4a87f-129">displayName</span><span class="sxs-lookup"><span data-stu-id="4a87f-129">displayName</span></span>|<span data-ttu-id="4a87f-130">String</span><span class="sxs-lookup"><span data-stu-id="4a87f-130">String</span></span>|<span data-ttu-id="4a87f-131">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="4a87f-131">Display name for the device category.</span></span>|
|<span data-ttu-id="4a87f-132">説明</span><span class="sxs-lookup"><span data-stu-id="4a87f-132">description</span></span>|<span data-ttu-id="4a87f-133">String</span><span class="sxs-lookup"><span data-stu-id="4a87f-133">String</span></span>|<span data-ttu-id="4a87f-134">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="4a87f-134">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a87f-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4a87f-135">Relationships</span></span>
<span data-ttu-id="4a87f-136">なし</span><span class="sxs-lookup"><span data-stu-id="4a87f-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a87f-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4a87f-137">JSON Representation</span></span>
<span data-ttu-id="4a87f-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4a87f-138">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



