# <a name="create-detectedapp"></a><span data-ttu-id="5967c-101">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="5967c-101">Create detectedApp</span></span>

> <span data-ttu-id="5967c-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5967c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5967c-103">新しい [detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5967c-103">Create a new [plannerBucket](../resources/intune_devices_detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5967c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5967c-104">Prerequisites</span></span>
<span data-ttu-id="5967c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5967c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5967c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5967c-107">Permission type</span></span>|<span data-ttu-id="5967c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5967c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5967c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5967c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5967c-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5967c-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5967c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5967c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5967c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5967c-112">Not supported.</span></span>|
|<span data-ttu-id="5967c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5967c-113">Application</span></span>|<span data-ttu-id="5967c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5967c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5967c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5967c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="5967c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5967c-116">Request headers</span></span>
|<span data-ttu-id="5967c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5967c-117">Header</span></span>|<span data-ttu-id="5967c-118">値</span><span class="sxs-lookup"><span data-stu-id="5967c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5967c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5967c-119">Authorization</span></span>|<span data-ttu-id="5967c-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5967c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5967c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5967c-121">Accept</span></span>|<span data-ttu-id="5967c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5967c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5967c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5967c-123">Request body</span></span>
<span data-ttu-id="5967c-124">要求本文で、detectedApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5967c-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5967c-125">次の表に、detectedApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5967c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5967c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5967c-126">Property</span></span>|<span data-ttu-id="5967c-127">型</span><span class="sxs-lookup"><span data-stu-id="5967c-127">Type</span></span>|<span data-ttu-id="5967c-128">説明</span><span class="sxs-lookup"><span data-stu-id="5967c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5967c-129">id</span><span class="sxs-lookup"><span data-stu-id="5967c-129">id</span></span>|<span data-ttu-id="5967c-130">String</span><span class="sxs-lookup"><span data-stu-id="5967c-130">String</span></span>|<span data-ttu-id="5967c-131">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5967c-131">The unique Identifier for the detected application.</span></span> <span data-ttu-id="5967c-132">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="5967c-132">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="5967c-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5967c-133">Read-only.</span></span>|
|<span data-ttu-id="5967c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="5967c-134">displayName</span></span>|<span data-ttu-id="5967c-135">String</span><span class="sxs-lookup"><span data-stu-id="5967c-135">String</span></span>|<span data-ttu-id="5967c-136">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="5967c-136">Name of the discovered application.</span></span> <span data-ttu-id="5967c-137">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="5967c-137">Read-only</span></span>|
|<span data-ttu-id="5967c-138">version</span><span class="sxs-lookup"><span data-stu-id="5967c-138">version</span></span>|<span data-ttu-id="5967c-139">String</span><span class="sxs-lookup"><span data-stu-id="5967c-139">String</span></span>|<span data-ttu-id="5967c-140">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="5967c-140">Version of the discovered application.</span></span> <span data-ttu-id="5967c-141">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="5967c-141">Read-only</span></span>|
|<span data-ttu-id="5967c-142">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="5967c-142">sizeInByte</span></span>|<span data-ttu-id="5967c-143">Int64</span><span class="sxs-lookup"><span data-stu-id="5967c-143">Int64</span></span>|<span data-ttu-id="5967c-144">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="5967c-144">Discovered application size in bytes.</span></span> <span data-ttu-id="5967c-145">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="5967c-145">Read-only</span></span>|
|<span data-ttu-id="5967c-146">deviceCount</span><span class="sxs-lookup"><span data-stu-id="5967c-146">deviceCount</span></span>|<span data-ttu-id="5967c-147">Int32</span><span class="sxs-lookup"><span data-stu-id="5967c-147">Int32</span></span>|<span data-ttu-id="5967c-148">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5967c-148">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="5967c-149">応答</span><span class="sxs-lookup"><span data-stu-id="5967c-149">Response</span></span>
<span data-ttu-id="5967c-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5967c-150">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_devices_detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5967c-151">例</span><span class="sxs-lookup"><span data-stu-id="5967c-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="5967c-152">要求</span><span class="sxs-lookup"><span data-stu-id="5967c-152">Request</span></span>
<span data-ttu-id="5967c-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5967c-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="5967c-154">応答</span><span class="sxs-lookup"><span data-stu-id="5967c-154">Response</span></span>
<span data-ttu-id="5967c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5967c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```



