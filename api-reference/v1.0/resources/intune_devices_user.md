# <a name="user-resource-type"></a><span data-ttu-id="e45f3-101">user リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e45f3-101">user resource type</span></span>

> <span data-ttu-id="e45f3-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e45f3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e45f3-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e45f3-103">Not yet documented</span></span>
## <a name="methods"></a><span data-ttu-id="e45f3-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="e45f3-104">Methods</span></span>
|<span data-ttu-id="e45f3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e45f3-105">Method</span></span>|<span data-ttu-id="e45f3-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e45f3-106">Return Type</span></span>|<span data-ttu-id="e45f3-107">説明</span><span class="sxs-lookup"><span data-stu-id="e45f3-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e45f3-108">List users</span><span class="sxs-lookup"><span data-stu-id="e45f3-108">List users</span></span>](../api/intune_devices_user_list.md)|<span data-ttu-id="e45f3-109">[user](../resources/intune_devices_user.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e45f3-109">[user](../resources/intune_devices_user.md) collection</span></span>|<span data-ttu-id="e45f3-110">[user](../resources/intune_devices_user.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e45f3-110">List properties and relationships of the [user](../resources/intune_devices_user.md) objects.</span></span>|
|[<span data-ttu-id="e45f3-111">Get user</span><span class="sxs-lookup"><span data-stu-id="e45f3-111">Get user</span></span>](../api/intune_devices_user_get.md)|[<span data-ttu-id="e45f3-112">user</span><span class="sxs-lookup"><span data-stu-id="e45f3-112">user</span></span>](../resources/intune_devices_user.md)|<span data-ttu-id="e45f3-113">[user](../resources/intune_devices_user.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e45f3-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_user.md) object.</span></span>|
|[<span data-ttu-id="e45f3-114">Create user</span><span class="sxs-lookup"><span data-stu-id="e45f3-114">Create user</span></span>](../api/intune_devices_user_create.md)|[<span data-ttu-id="e45f3-115">user</span><span class="sxs-lookup"><span data-stu-id="e45f3-115">user</span></span>](../resources/intune_devices_user.md)|<span data-ttu-id="e45f3-116">新しい [user](../resources/intune_devices_user.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e45f3-116">Create a new user object.</span></span>|
|[<span data-ttu-id="e45f3-117">Delete user</span><span class="sxs-lookup"><span data-stu-id="e45f3-117">Delete user</span></span>](../api/intune_devices_user_delete.md)|<span data-ttu-id="e45f3-118">なし</span><span class="sxs-lookup"><span data-stu-id="e45f3-118">None</span></span>|<span data-ttu-id="e45f3-119">[user](../resources/intune_devices_user.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e45f3-119">Deletes a [user](../resources/intune_devices_user.md).</span></span>|
|[<span data-ttu-id="e45f3-120">Update user</span><span class="sxs-lookup"><span data-stu-id="e45f3-120">Update user</span></span>](../api/intune_devices_user_update.md)|[<span data-ttu-id="e45f3-121">user</span><span class="sxs-lookup"><span data-stu-id="e45f3-121">user</span></span>](../resources/intune_devices_user.md)|<span data-ttu-id="e45f3-122">[user](../resources/intune_devices_user.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e45f3-122">Update the properties of a user object.</span></span>|
|[<span data-ttu-id="e45f3-123">removeAllDevicesFromManagement アクション</span><span class="sxs-lookup"><span data-stu-id="e45f3-123">removeAllDevicesFromManagement action</span></span>](../api/intune_devices_user_removealldevicesfrommanagement.md)|<span data-ttu-id="e45f3-124">なし</span><span class="sxs-lookup"><span data-stu-id="e45f3-124">None</span></span>|<span data-ttu-id="e45f3-125">対象ユーザーの管理からすべてのデバイスを破棄します</span><span class="sxs-lookup"><span data-stu-id="e45f3-125">Retire all devices from management for this user</span></span>|

## <a name="properties"></a><span data-ttu-id="e45f3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e45f3-126">Properties</span></span>
|<span data-ttu-id="e45f3-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e45f3-127">Property</span></span>|<span data-ttu-id="e45f3-128">型</span><span class="sxs-lookup"><span data-stu-id="e45f3-128">Type</span></span>|<span data-ttu-id="e45f3-129">説明</span><span class="sxs-lookup"><span data-stu-id="e45f3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45f3-130">id</span><span class="sxs-lookup"><span data-stu-id="e45f3-130">id</span></span>|<span data-ttu-id="e45f3-131">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e45f3-131">String</span></span>|<span data-ttu-id="e45f3-132">ユーザーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e45f3-132">Unique identifier of the folder.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e45f3-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e45f3-133">Relationships</span></span>
|<span data-ttu-id="e45f3-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e45f3-134">Relationship</span></span>|<span data-ttu-id="e45f3-135">型</span><span class="sxs-lookup"><span data-stu-id="e45f3-135">Type</span></span>|<span data-ttu-id="e45f3-136">説明</span><span class="sxs-lookup"><span data-stu-id="e45f3-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45f3-137">managedDevices</span><span class="sxs-lookup"><span data-stu-id="e45f3-137">managedDevices</span></span>|<span data-ttu-id="e45f3-138">[managedDevice](../resources/intune_devices_manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e45f3-138">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="e45f3-139">対象ユーザーに関連付けられている管理対象デバイス。</span><span class="sxs-lookup"><span data-stu-id="e45f3-139">The managed devices associated with the user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e45f3-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e45f3-140">JSON Representation</span></span>
<span data-ttu-id="e45f3-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e45f3-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.user",
  "id": "String (identifier)"
}
```



