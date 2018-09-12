# <a name="create-detectedapp"></a><span data-ttu-id="4382b-101">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="4382b-101">Create detectedApp</span></span>

> <span data-ttu-id="4382b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4382b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4382b-103">新しい [detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4382b-103">Create a new [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4382b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="4382b-104">Prerequisites</span></span>
<span data-ttu-id="4382b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4382b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4382b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4382b-107">Permission type</span></span>|<span data-ttu-id="4382b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4382b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4382b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4382b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4382b-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4382b-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4382b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4382b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4382b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4382b-112">Not supported.</span></span>|
|<span data-ttu-id="4382b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4382b-113">Application</span></span>|<span data-ttu-id="4382b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4382b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4382b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4382b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="4382b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4382b-116">Request headers</span></span>
|<span data-ttu-id="4382b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4382b-117">Header</span></span>|<span data-ttu-id="4382b-118">値</span><span class="sxs-lookup"><span data-stu-id="4382b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4382b-119">承認</span><span class="sxs-lookup"><span data-stu-id="4382b-119">Authorization</span></span>|<span data-ttu-id="4382b-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4382b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4382b-121">承諾</span><span class="sxs-lookup"><span data-stu-id="4382b-121">Accept</span></span>|<span data-ttu-id="4382b-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="4382b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4382b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4382b-123">Request body</span></span>
<span data-ttu-id="4382b-124">要求本文で、detectedApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4382b-124">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="4382b-125">次の表に、detectedApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4382b-125">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="4382b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4382b-126">Property</span></span>|<span data-ttu-id="4382b-127">型</span><span class="sxs-lookup"><span data-stu-id="4382b-127">Type</span></span>|<span data-ttu-id="4382b-128">説明</span><span class="sxs-lookup"><span data-stu-id="4382b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4382b-129">ID</span><span class="sxs-lookup"><span data-stu-id="4382b-129">id</span></span>|<span data-ttu-id="4382b-130">文字列</span><span class="sxs-lookup"><span data-stu-id="4382b-130">String</span></span>|<span data-ttu-id="4382b-131">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4382b-131">The unique Identifier for the detected application.</span></span> <span data-ttu-id="4382b-132">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="4382b-132">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="4382b-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4382b-133">Read-only.</span></span>|
|<span data-ttu-id="4382b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="4382b-134">displayName</span></span>|<span data-ttu-id="4382b-135">文字列</span><span class="sxs-lookup"><span data-stu-id="4382b-135">String</span></span>|<span data-ttu-id="4382b-136">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="4382b-136">Name of the discovered application.</span></span> <span data-ttu-id="4382b-137">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="4382b-137">Read-only</span></span>|
|<span data-ttu-id="4382b-138">バージョン</span><span class="sxs-lookup"><span data-stu-id="4382b-138">version</span></span>|<span data-ttu-id="4382b-139">文字列</span><span class="sxs-lookup"><span data-stu-id="4382b-139">String</span></span>|<span data-ttu-id="4382b-140">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4382b-140">Version of the discovered application.</span></span> <span data-ttu-id="4382b-141">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="4382b-141">Read-only</span></span>|
|<span data-ttu-id="4382b-142">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="4382b-142">sizeInByte</span></span>|<span data-ttu-id="4382b-143">Int64</span><span class="sxs-lookup"><span data-stu-id="4382b-143">Int64</span></span>|<span data-ttu-id="4382b-144">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="4382b-144">Discovered application size in bytes.</span></span> <span data-ttu-id="4382b-145">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="4382b-145">Read-only</span></span>|
|<span data-ttu-id="4382b-146">deviceCount</span><span class="sxs-lookup"><span data-stu-id="4382b-146">deviceCount</span></span>|<span data-ttu-id="4382b-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4382b-147">Int32</span></span>|<span data-ttu-id="4382b-148">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="4382b-148">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="4382b-149">応答</span><span class="sxs-lookup"><span data-stu-id="4382b-149">Response</span></span>
<span data-ttu-id="4382b-150">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [detectedApp](../resources/intune_devices_detectedapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4382b-150">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune_devices_detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4382b-151">例</span><span class="sxs-lookup"><span data-stu-id="4382b-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="4382b-152">要求</span><span class="sxs-lookup"><span data-stu-id="4382b-152">Request</span></span>
<span data-ttu-id="4382b-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4382b-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4382b-154">応答</span><span class="sxs-lookup"><span data-stu-id="4382b-154">Response</span></span>
<span data-ttu-id="4382b-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4382b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








