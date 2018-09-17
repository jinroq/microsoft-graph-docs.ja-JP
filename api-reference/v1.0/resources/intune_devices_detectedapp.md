# <a name="detectedapp-resource-type"></a><span data-ttu-id="e3d4c-101">detectedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e3d4c-101">detectedApp resource type</span></span>

> <span data-ttu-id="e3d4c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3d4c-103">管理対象デバイスにインストールされている管理対象アプリまたは非管理対象アプリです。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-103">A managed or unmanaged app that is installed on a managed device.</span></span> <span data-ttu-id="e3d4c-104">非管理対象アプリは、会社所有のデバイスにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-104">Unmanaged apps will only appear for devices marked as corporate owned.</span></span>
## <a name="methods"></a><span data-ttu-id="e3d4c-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3d4c-105">Methods</span></span>
|<span data-ttu-id="e3d4c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e3d4c-106">Method</span></span>|<span data-ttu-id="e3d4c-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e3d4c-107">Return Type</span></span>|<span data-ttu-id="e3d4c-108">説明</span><span class="sxs-lookup"><span data-stu-id="e3d4c-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e3d4c-109">detectedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="e3d4c-109">List detectedApps</span></span>](../api/intune_devices_detectedapp_list.md)|<span data-ttu-id="e3d4c-110">[detectedApp](../resources/intune_devices_detectedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3d4c-110">[detectedApp](../resources/intune_devices_detectedapp.md) collection</span></span>|<span data-ttu-id="e3d4c-111">[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-111">List properties and relationships of the [detectedApp](../resources/intune_devices_detectedapp.md) objects.</span></span>|
|[<span data-ttu-id="e3d4c-112">detectedApp の取得</span><span class="sxs-lookup"><span data-stu-id="e3d4c-112">Get detectedApp</span></span>](../api/intune_devices_detectedapp_get.md)|[<span data-ttu-id="e3d4c-113">detectedApp</span><span class="sxs-lookup"><span data-stu-id="e3d4c-113">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="e3d4c-114">[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-114">Read properties and relationships of the [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>|
|[<span data-ttu-id="e3d4c-115">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="e3d4c-115">Create detectedApp</span></span>](../api/intune_devices_detectedapp_create.md)|[<span data-ttu-id="e3d4c-116">detectedApp</span><span class="sxs-lookup"><span data-stu-id="e3d4c-116">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="e3d4c-117">新しい [detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-117">Create a new [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>|
|[<span data-ttu-id="e3d4c-118">detectedApp の削除</span><span class="sxs-lookup"><span data-stu-id="e3d4c-118">Delete detectedApp</span></span>](../api/intune_devices_detectedapp_delete.md)|<span data-ttu-id="e3d4c-119">なし</span><span class="sxs-lookup"><span data-stu-id="e3d4c-119">None</span></span>|<span data-ttu-id="e3d4c-120">[detectedApp](../resources/intune_devices_detectedapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-120">Deletes a [detectedApp](../resources/intune_devices_detectedapp.md).</span></span>|
|[<span data-ttu-id="e3d4c-121">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="e3d4c-121">Update detectedApp</span></span>](../api/intune_devices_detectedapp_update.md)|[<span data-ttu-id="e3d4c-122">detectedApp</span><span class="sxs-lookup"><span data-stu-id="e3d4c-122">detectedApp</span></span>](../resources/intune_devices_detectedapp.md)|<span data-ttu-id="e3d4c-123">[detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-123">Update the properties of a [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e3d4c-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3d4c-124">Properties</span></span>
|<span data-ttu-id="e3d4c-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3d4c-125">Property</span></span>|<span data-ttu-id="e3d4c-126">タイプ</span><span class="sxs-lookup"><span data-stu-id="e3d4c-126">Type</span></span>|<span data-ttu-id="e3d4c-127">説明</span><span class="sxs-lookup"><span data-stu-id="e3d4c-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3d4c-128">ID</span><span class="sxs-lookup"><span data-stu-id="e3d4c-128">id</span></span>|<span data-ttu-id="e3d4c-129">文字列</span><span class="sxs-lookup"><span data-stu-id="e3d4c-129">String</span></span>|<span data-ttu-id="e3d4c-130">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-130">The unique Identifier for the detected application.</span></span> <span data-ttu-id="e3d4c-131">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-131">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="e3d4c-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-132">Read-only.</span></span>|
|<span data-ttu-id="e3d4c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e3d4c-133">displayName</span></span>|<span data-ttu-id="e3d4c-134">文字列</span><span class="sxs-lookup"><span data-stu-id="e3d4c-134">String</span></span>|<span data-ttu-id="e3d4c-135">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-135">Name of the discovered application.</span></span> <span data-ttu-id="e3d4c-136">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="e3d4c-136">Read-only</span></span>|
|<span data-ttu-id="e3d4c-137">バージョン</span><span class="sxs-lookup"><span data-stu-id="e3d4c-137">version</span></span>|<span data-ttu-id="e3d4c-138">文字列</span><span class="sxs-lookup"><span data-stu-id="e3d4c-138">String</span></span>|<span data-ttu-id="e3d4c-139">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-139">Version of the discovered application.</span></span> <span data-ttu-id="e3d4c-140">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="e3d4c-140">Read-only</span></span>|
|<span data-ttu-id="e3d4c-141">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="e3d4c-141">sizeInByte</span></span>|<span data-ttu-id="e3d4c-142">Int64</span><span class="sxs-lookup"><span data-stu-id="e3d4c-142">Int64</span></span>|<span data-ttu-id="e3d4c-143">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-143">Discovered application size in bytes.</span></span> <span data-ttu-id="e3d4c-144">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="e3d4c-144">Read-only</span></span>|
|<span data-ttu-id="e3d4c-145">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e3d4c-145">deviceCount</span></span>|<span data-ttu-id="e3d4c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="e3d4c-146">Int32</span></span>|<span data-ttu-id="e3d4c-147">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e3d4c-147">The number of devices that have installed this application</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3d4c-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e3d4c-148">Relationships</span></span>
|<span data-ttu-id="e3d4c-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e3d4c-149">Relationship</span></span>|<span data-ttu-id="e3d4c-150">型</span><span class="sxs-lookup"><span data-stu-id="e3d4c-150">Type</span></span>|<span data-ttu-id="e3d4c-151">説明</span><span class="sxs-lookup"><span data-stu-id="e3d4c-151">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3d4c-152">managedDevices</span><span class="sxs-lookup"><span data-stu-id="e3d4c-152">managedDevices</span></span>|<span data-ttu-id="e3d4c-153">[managedDevice](../resources/intune_devices_manageddevice.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3d4c-153">[managedDevice](../resources/intune_devices_manageddevice.md) collection</span></span>|<span data-ttu-id="e3d4c-154">検出されたアプリケーションがインストールされているデバイス</span><span class="sxs-lookup"><span data-stu-id="e3d4c-154">The devices that have the discovered application installed</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e3d4c-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e3d4c-155">JSON Representation</span></span>
<span data-ttu-id="e3d4c-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e3d4c-156">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}-->
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








