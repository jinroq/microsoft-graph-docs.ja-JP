# <a name="detectedapp-resource-type"></a><span data-ttu-id="f17b8-101">detectedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f17b8-101">detectedApp resource type</span></span>

> <span data-ttu-id="f17b8-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f17b8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f17b8-103">管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。</span><span class="sxs-lookup"><span data-stu-id="f17b8-103">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="f17b8-104">非管理対象アプリは、会社所有のデバイスにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="f17b8-104">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="f17b8-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f17b8-105">Methods</span></span>
|<span data-ttu-id="f17b8-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f17b8-106">Method</span></span>|<span data-ttu-id="f17b8-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f17b8-107">Return Type</span></span>|<span data-ttu-id="f17b8-108">説明</span><span class="sxs-lookup"><span data-stu-id="f17b8-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f17b8-109">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="f17b8-109">List detectedApps</span></span>](../api/intune_devices_detectedapp_list.md)|<span data-ttu-id="f17b8-110">[detectedApp](../resources/intune_devices_detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f17b8-110">[detectedApp](../resources/intune_devices_detectedapp.md) collection</span></span>|<span data-ttu-id="f17b8-111">[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f17b8-111">List properties and relationships of the [detectedApp](../resources/intune_devices_detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="f17b8-112">detectedApp の取得</span><span class="sxs-lookup"><span data-stu-id="f17b8-112">Get detectedApp</span></span>](../api/intune_devices_detectedapp_get.md)|[<span data-ttu-id="f17b8-113">detectedApp</span><span class="sxs-lookup"><span data-stu-id="f17b8-113">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="f17b8-114">[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f17b8-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_devices_detectedapp.md) object.</span></span>|
|[<span data-ttu-id="f17b8-115">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="f17b8-115">Create detectedApp</span></span>](../api/intune_devices_detectedapp_create.md)|[<span data-ttu-id="f17b8-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="f17b8-116">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="f17b8-117">新しい [detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f17b8-117">Create a new [plannerBucket](../resources/intune_devices_detectedapp.md) object.</span></span>|
|[<span data-ttu-id="f17b8-118">detectedApp の削除</span><span class="sxs-lookup"><span data-stu-id="f17b8-118">Delete detectedApp</span></span>](../api/intune_devices_detectedapp_delete.md)|<span data-ttu-id="f17b8-119">なし</span><span class="sxs-lookup"><span data-stu-id="f17b8-119">None</span></span>|<span data-ttu-id="f17b8-120">[detectedApp](../resources/intune_devices_detectedapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="f17b8-120">Deletes a [detectedApp](../resources/intune_devices_detectedapp.md).</span></span>|
|[<span data-ttu-id="f17b8-121">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="f17b8-121">Update detectedApp</span></span>](../api/intune_devices_detectedapp_update.md)|[<span data-ttu-id="f17b8-122">detectedApp</span><span class="sxs-lookup"><span data-stu-id="f17b8-122">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="f17b8-123">[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f17b8-123">Update the properties of a [calendar](../resources/intune_devices_detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f17b8-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f17b8-124">Properties</span></span>
|<span data-ttu-id="f17b8-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f17b8-125">Property</span></span>|<span data-ttu-id="f17b8-126">型</span><span class="sxs-lookup"><span data-stu-id="f17b8-126">Type</span></span>|<span data-ttu-id="f17b8-127">説明</span><span class="sxs-lookup"><span data-stu-id="f17b8-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f17b8-128">id</span><span class="sxs-lookup"><span data-stu-id="f17b8-128">id</span></span>|<span data-ttu-id="f17b8-129">String</span><span class="sxs-lookup"><span data-stu-id="f17b8-129">String</span></span>|<span data-ttu-id="f17b8-130">検出されたアプリケーションの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="f17b8-130">The unique Identifier for the detected application.</span></span> <span data-ttu-id="f17b8-131">これは、Intune によって、アプリケーション作成時に自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="f17b8-131">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="f17b8-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f17b8-132">Read-only.</span></span>|
|<span data-ttu-id="f17b8-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f17b8-133">displayName</span></span>|<span data-ttu-id="f17b8-134">String</span><span class="sxs-lookup"><span data-stu-id="f17b8-134">String</span></span>|<span data-ttu-id="f17b8-135">検出されたアプリケーションの名前です。</span><span class="sxs-lookup"><span data-stu-id="f17b8-135">Name of the discovered application.</span></span> <span data-ttu-id="f17b8-136">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="f17b8-136">Read-only</span></span>|
|<span data-ttu-id="f17b8-137">version</span><span class="sxs-lookup"><span data-stu-id="f17b8-137">version</span></span>|<span data-ttu-id="f17b8-138">String</span><span class="sxs-lookup"><span data-stu-id="f17b8-138">String</span></span>|<span data-ttu-id="f17b8-139">検出されたアプリケーションのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="f17b8-139">Version of the discovered application.</span></span> <span data-ttu-id="f17b8-140">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="f17b8-140">Read-only</span></span>|
|<span data-ttu-id="f17b8-141">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="f17b8-141">sizeInByte</span></span>|<span data-ttu-id="f17b8-142">Int64</span><span class="sxs-lookup"><span data-stu-id="f17b8-142">Int64</span></span>|<span data-ttu-id="f17b8-143">検出されたアプリケーションのサイズ (バイト単位) です。</span><span class="sxs-lookup"><span data-stu-id="f17b8-143">Discovered application size in bytes.</span></span> <span data-ttu-id="f17b8-144">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="f17b8-144">Read-only</span></span>|
|<span data-ttu-id="f17b8-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="f17b8-145">deviceCount</span></span>|<span data-ttu-id="f17b8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f17b8-146">Int32</span></span>|<span data-ttu-id="f17b8-147">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="f17b8-147">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="f17b8-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f17b8-148">Relationships</span></span>
|<span data-ttu-id="f17b8-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f17b8-149">Relationship</span></span>|<span data-ttu-id="f17b8-150">型</span><span class="sxs-lookup"><span data-stu-id="f17b8-150">Type</span></span>|<span data-ttu-id="f17b8-151">説明</span><span class="sxs-lookup"><span data-stu-id="f17b8-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f17b8-152">managedDevices</span><span class="sxs-lookup"><span data-stu-id="f17b8-152">managedDevices</span></span>|<span data-ttu-id="f17b8-153">[managedDevice](../resources/intune_devices_manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f17b8-153">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="f17b8-154">検出されたアプリケーションがインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="f17b8-154">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f17b8-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f17b8-155">JSON Representation</span></span>
<span data-ttu-id="f17b8-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f17b8-156">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```


