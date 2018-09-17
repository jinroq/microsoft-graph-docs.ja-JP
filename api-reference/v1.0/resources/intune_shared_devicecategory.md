# <a name="devicecategory-resource-type"></a><span data-ttu-id="17263-101">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="17263-101">deviceCategory resource type</span></span>

> <span data-ttu-id="17263-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="17263-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17263-103">デバイス カテゴリは、デバイスを整理する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="17263-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="17263-104">デバイス カテゴリを使用して、会社の管理者は、自社にとって意味のある、独自のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="17263-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="17263-105">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="17263-105">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="17263-106">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="17263-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="17263-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="17263-107">Methods</span></span>
|<span data-ttu-id="17263-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="17263-108">Method</span></span>|<span data-ttu-id="17263-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="17263-109">Return Type</span></span>|<span data-ttu-id="17263-110">説明</span><span class="sxs-lookup"><span data-stu-id="17263-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17263-111">[deviceCategories をリストする](../api/intune_shared_devicecategory_list.md) オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="17263-111">[List deviceCategories](../api/intune_shared_devicecategory_list.md) objects.</span></span>|
|<span data-ttu-id="17263-112">[deviceCategory を取得する](../api/intune_shared_devicecategory_get.md) オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="17263-112">[Get deviceCategory](../api/intune_shared_devicecategory_get.md) object.</span></span>|
|<span data-ttu-id="17263-113">[DeviceCategory を作成する](../api/intune_shared_devicecategory_create.md) オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="17263-113">Create a new [deviceCategory](../api/intune_shared_devicecategory_create.md) object.</span></span>|
|<span data-ttu-id="17263-114">[DeviceCategory を削除する](../api/intune_shared_devicecategory_delete.md)。</span><span class="sxs-lookup"><span data-stu-id="17263-114">Delete deviceCategory</span></span>|
|<span data-ttu-id="17263-115">[deviceCategory を更新する](../api/intune_shared_devicecategory_update.md) オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="17263-115">Update the properties of a [deviceCategory](../api/intune_shared_devicecategory_update.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="17263-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17263-116">Properties</span></span>
|<span data-ttu-id="17263-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17263-117">Property</span></span>|<span data-ttu-id="17263-118">型</span><span class="sxs-lookup"><span data-stu-id="17263-118">Type</span></span>|<span data-ttu-id="17263-119">説明</span><span class="sxs-lookup"><span data-stu-id="17263-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17263-120">ID</span><span class="sxs-lookup"><span data-stu-id="17263-120">id</span></span>|<span data-ttu-id="17263-121">文字列</span><span class="sxs-lookup"><span data-stu-id="17263-121">String</span></span>|<span data-ttu-id="17263-122">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="17263-122">Unique identifier for the device category.</span></span> <span data-ttu-id="17263-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="17263-123">Read-only.</span></span>|
|<span data-ttu-id="17263-124">**採用**</span><span class="sxs-lookup"><span data-stu-id="17263-124">**On-boarding**</span></span>|
|<span data-ttu-id="17263-125">displayName</span><span class="sxs-lookup"><span data-stu-id="17263-125">displayName</span></span>|<span data-ttu-id="17263-126">文字列</span><span class="sxs-lookup"><span data-stu-id="17263-126">String</span></span>|<span data-ttu-id="17263-127">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="17263-127">Display name for the device category.</span></span>|
|<span data-ttu-id="17263-128">説明</span><span class="sxs-lookup"><span data-stu-id="17263-128">description</span></span>|<span data-ttu-id="17263-129">文字列</span><span class="sxs-lookup"><span data-stu-id="17263-129">String</span></span>|<span data-ttu-id="17263-130">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="17263-130">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17263-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="17263-131">Relationships</span></span>
<span data-ttu-id="17263-132">なし</span><span class="sxs-lookup"><span data-stu-id="17263-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17263-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17263-133">JSON Representation</span></span>
<span data-ttu-id="17263-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17263-134">Here is a JSON representation of the resource.</span></span>
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



