# <a name="devicecategory-resource-type"></a><span data-ttu-id="b2648-101">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2648-101">deviceCategory resource type</span></span>

> <span data-ttu-id="b2648-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2648-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2648-103">デバイス カテゴリは、デバイスを整理する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="b2648-103">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="b2648-104">デバイス カテゴリを使用して、会社の管理者は、自社にとって意味のある、独自のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="b2648-104">Using device categories, company administrators can define their own categories that make sense to their company.</span></span> <span data-ttu-id="b2648-105">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="b2648-105">These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="b2648-106">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="b2648-106">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>
## <a name="methods"></a><span data-ttu-id="b2648-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b2648-107">Methods</span></span>
|<span data-ttu-id="b2648-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b2648-108">Method</span></span>|<span data-ttu-id="b2648-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b2648-109">Return Type</span></span>|<span data-ttu-id="b2648-110">説明</span><span class="sxs-lookup"><span data-stu-id="b2648-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b2648-111">deviceCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="b2648-111">List deviceCategories</span></span>](../api/intune_onboarding_devicecategory_list.md)|<span data-ttu-id="b2648-112">[deviceCategory](../resources/intune_onboarding_devicecategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b2648-112">[deviceCategory](../resources/intune_onboarding_devicecategory.md) collection</span></span>|<span data-ttu-id="b2648-113">[deviceCategory](../resources/intune_onboarding_devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b2648-113">List properties and relationships of the [deviceCategory](../resources/intune_onboarding_devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="b2648-114">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="b2648-114">Get deviceCategory</span></span>](../api/intune_onboarding_devicecategory_get.md)|[<span data-ttu-id="b2648-115">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b2648-115">deviceCategory</span></span>](../resources/intune_onboarding_devicecategory.md)|<span data-ttu-id="b2648-116">[deviceCategory](../resources/intune_onboarding_devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b2648-116">Read properties and relationships of [plannerPlanDetails](../resources/intune_onboarding_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b2648-117">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="b2648-117">Create deviceCategory</span></span>](../api/intune_onboarding_devicecategory_create.md)|[<span data-ttu-id="b2648-118">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b2648-118">deviceCategory</span></span>](../resources/intune_onboarding_devicecategory.md)|<span data-ttu-id="b2648-119">新しい [deviceCategory](../resources/intune_onboarding_devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b2648-119">Create a new [plannerBucket](../resources/intune_onboarding_devicecategory.md) object.</span></span>|
|[<span data-ttu-id="b2648-120">deviceCategory の削除</span><span class="sxs-lookup"><span data-stu-id="b2648-120">Delete deviceCategory</span></span>](../api/intune_onboarding_devicecategory_delete.md)|<span data-ttu-id="b2648-121">なし</span><span class="sxs-lookup"><span data-stu-id="b2648-121">None</span></span>|<span data-ttu-id="b2648-122">[deviceCategory](../resources/intune_onboarding_devicecategory.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b2648-122">Deletes a [deviceCategory](../resources/intune_onboarding_devicecategory.md).</span></span>|
|[<span data-ttu-id="b2648-123">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="b2648-123">Update deviceCategory</span></span>](../api/intune_onboarding_devicecategory_update.md)|[<span data-ttu-id="b2648-124">deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b2648-124">deviceCategory</span></span>](../resources/intune_onboarding_devicecategory.md)|<span data-ttu-id="b2648-125">[deviceCategory](../resources/intune_onboarding_devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b2648-125">Update the properties of a [calendar](../resources/intune_onboarding_devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b2648-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2648-126">Properties</span></span>
|<span data-ttu-id="b2648-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2648-127">Property</span></span>|<span data-ttu-id="b2648-128">型</span><span class="sxs-lookup"><span data-stu-id="b2648-128">Type</span></span>|<span data-ttu-id="b2648-129">説明</span><span class="sxs-lookup"><span data-stu-id="b2648-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2648-130">id</span><span class="sxs-lookup"><span data-stu-id="b2648-130">id</span></span>|<span data-ttu-id="b2648-131">String</span><span class="sxs-lookup"><span data-stu-id="b2648-131">String</span></span>|<span data-ttu-id="b2648-132">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b2648-132">Unique identifier for the device category.</span></span> <span data-ttu-id="b2648-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2648-133">Read-only.</span></span>|
|<span data-ttu-id="b2648-134">displayName</span><span class="sxs-lookup"><span data-stu-id="b2648-134">displayName</span></span>|<span data-ttu-id="b2648-135">String</span><span class="sxs-lookup"><span data-stu-id="b2648-135">String</span></span>|<span data-ttu-id="b2648-136">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="b2648-136">Display name for the device category.</span></span>|
|<span data-ttu-id="b2648-137">description</span><span class="sxs-lookup"><span data-stu-id="b2648-137">description</span></span>|<span data-ttu-id="b2648-138">String</span><span class="sxs-lookup"><span data-stu-id="b2648-138">String</span></span>|<span data-ttu-id="b2648-139">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="b2648-139">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2648-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b2648-140">Relationships</span></span>
<span data-ttu-id="b2648-141">なし</span><span class="sxs-lookup"><span data-stu-id="b2648-141">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b2648-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2648-142">JSON Representation</span></span>
<span data-ttu-id="b2648-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b2648-143">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



