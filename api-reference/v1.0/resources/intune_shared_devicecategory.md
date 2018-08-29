# <a name="devicecategory-resource-type"></a><span data-ttu-id="45701-101">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="45701-101">deviceCategory resource type</span></span>

> <span data-ttu-id="45701-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="45701-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45701-103">デバイス カテゴリは、デバイスを整理する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="45701-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="45701-104">デバイス カテゴリを使用して、会社の管理者は、自社にとって意味のある、独自のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="45701-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="45701-105">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="45701-105">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="45701-106">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="45701-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="45701-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="45701-107">Methods</span></span>
|<span data-ttu-id="45701-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="45701-108">Method</span></span>|<span data-ttu-id="45701-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="45701-109">Return Type</span></span>|<span data-ttu-id="45701-110">説明</span><span class="sxs-lookup"><span data-stu-id="45701-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45701-111">[リストの deviceCategories](../api/intune_shared_devicecategory_list.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="45701-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) collection</span></span>|<span data-ttu-id="45701-112">[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="45701-112">List properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="45701-113">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="45701-113">Get deviceCategory</span></span>](../api/intune_shared_devicecategory_get.md)|<span data-ttu-id="45701-114">[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="45701-114">Read properties and relationships of the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="45701-115">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="45701-115">Create deviceCategory</span></span>](../api/intune_shared_devicecategory_create.md)|<span data-ttu-id="45701-116">新しい [deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="45701-116">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|
|<span data-ttu-id="45701-117">[DeviceCategory を削除](../api/intune_shared_devicecategory_delete.md)。</span><span class="sxs-lookup"><span data-stu-id="45701-117">[Delete deviceCategory](../api/intune_shared_devicecategory_delete.md)</span></span>|
|[<span data-ttu-id="45701-118">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="45701-118">Update deviceCategory</span></span>](../api/intune_shared_devicecategory_update.md)|<span data-ttu-id="45701-119">[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="45701-119">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="45701-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45701-120">Properties</span></span>
|<span data-ttu-id="45701-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45701-121">Property</span></span>|<span data-ttu-id="45701-122">タイプ</span><span class="sxs-lookup"><span data-stu-id="45701-122">Type</span></span>|<span data-ttu-id="45701-123">説明</span><span class="sxs-lookup"><span data-stu-id="45701-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45701-124">ID</span><span class="sxs-lookup"><span data-stu-id="45701-124">id</span></span>|<span data-ttu-id="45701-125">文字列</span><span class="sxs-lookup"><span data-stu-id="45701-125">String</span></span>|<span data-ttu-id="45701-126">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="45701-126">Unique identifier for the device category.</span></span> <span data-ttu-id="45701-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="45701-127">Read-only.</span></span>|
|<span data-ttu-id="45701-128">**採用**</span><span class="sxs-lookup"><span data-stu-id="45701-128">**On-boarding**</span></span>|
|<span data-ttu-id="45701-129">displayName</span><span class="sxs-lookup"><span data-stu-id="45701-129">displayName</span></span>|<span data-ttu-id="45701-130">文字列</span><span class="sxs-lookup"><span data-stu-id="45701-130">String</span></span>|<span data-ttu-id="45701-131">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="45701-131">Display name for the device category.</span></span>|
|<span data-ttu-id="45701-132">説明</span><span class="sxs-lookup"><span data-stu-id="45701-132">description</span></span>|<span data-ttu-id="45701-133">文字列</span><span class="sxs-lookup"><span data-stu-id="45701-133">String</span></span>|<span data-ttu-id="45701-134">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="45701-134">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45701-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="45701-135">Relationships</span></span>
<span data-ttu-id="45701-136">なし</span><span class="sxs-lookup"><span data-stu-id="45701-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45701-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45701-137">JSON Representation</span></span>
<span data-ttu-id="45701-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="45701-138">Here is a JSON representation of the resource.</span></span>
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



