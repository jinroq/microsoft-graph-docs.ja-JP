# <a name="update-devicecategory"></a><span data-ttu-id="44294-101">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="44294-101">Update deviceCategory</span></span>

> <span data-ttu-id="44294-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="44294-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44294-103">[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="44294-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44294-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="44294-104">Prerequisites</span></span>
<span data-ttu-id="44294-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44294-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44294-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44294-107">Permission type</span></span>|<span data-ttu-id="44294-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="44294-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44294-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44294-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="44294-110">&nbsp;&nbsp; **契約時**と</span><span class="sxs-lookup"><span data-stu-id="44294-110">&nbsp; &nbsp; **Onboarding** and</span></span> <br> <span data-ttu-id="44294-111">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="44294-111">&nbsp; &nbsp; **Device Management**</span></span>| <span data-ttu-id="44294-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44294-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="44294-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44294-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44294-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44294-114">Not supported.</span></span>|
|<span data-ttu-id="44294-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44294-115">Application</span></span>|<span data-ttu-id="44294-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44294-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44294-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44294-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="44294-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44294-118">Request headers</span></span>
|<span data-ttu-id="44294-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44294-119">Header</span></span>|<span data-ttu-id="44294-120">値</span><span class="sxs-lookup"><span data-stu-id="44294-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44294-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44294-121">Authorization</span></span>|<span data-ttu-id="44294-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="44294-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44294-123">Accept</span><span class="sxs-lookup"><span data-stu-id="44294-123">Accept</span></span>|<span data-ttu-id="44294-124">application/json</span><span class="sxs-lookup"><span data-stu-id="44294-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44294-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="44294-125">Request body</span></span>
<span data-ttu-id="44294-126">要求本文で、[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="44294-126">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="44294-127">次の表に、[deviceCategory](../resources/intune_shared_devicecategory.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="44294-127">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="44294-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44294-128">Property</span></span>|<span data-ttu-id="44294-129">型</span><span class="sxs-lookup"><span data-stu-id="44294-129">Type</span></span>|<span data-ttu-id="44294-130">説明</span><span class="sxs-lookup"><span data-stu-id="44294-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44294-131">id</span><span class="sxs-lookup"><span data-stu-id="44294-131">id</span></span>|<span data-ttu-id="44294-132">文字列</span><span class="sxs-lookup"><span data-stu-id="44294-132">String</span></span>|<span data-ttu-id="44294-133">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="44294-133">Unique identifier for the device category.</span></span> <span data-ttu-id="44294-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="44294-134">Read-only.</span></span>|
|<span data-ttu-id="44294-135">**契約時**</span><span class="sxs-lookup"><span data-stu-id="44294-135">**Onboarding**</span></span>|
|<span data-ttu-id="44294-136">displayName</span><span class="sxs-lookup"><span data-stu-id="44294-136">displayName</span></span>|<span data-ttu-id="44294-137">String</span><span class="sxs-lookup"><span data-stu-id="44294-137">String</span></span>|<span data-ttu-id="44294-138">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="44294-138">Display name for the device category.</span></span>|
|<span data-ttu-id="44294-139">説明</span><span class="sxs-lookup"><span data-stu-id="44294-139">description</span></span>|<span data-ttu-id="44294-140">String</span><span class="sxs-lookup"><span data-stu-id="44294-140">String</span></span>|<span data-ttu-id="44294-141">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="44294-141">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="44294-142">応答</span><span class="sxs-lookup"><span data-stu-id="44294-142">Response</span></span>
<span data-ttu-id="44294-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="44294-143">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44294-144">例</span><span class="sxs-lookup"><span data-stu-id="44294-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="44294-145">要求</span><span class="sxs-lookup"><span data-stu-id="44294-145">Request</span></span>
<span data-ttu-id="44294-146">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44294-146">Here are examples of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}

PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

### <a name="response"></a><span data-ttu-id="44294-147">応答</span><span class="sxs-lookup"><span data-stu-id="44294-147">Response</span></span>
<span data-ttu-id="44294-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="44294-148">Here is an example of the response.</span></span> <span data-ttu-id="44294-149">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="44294-149">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="44294-150">応答のプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="44294-150">Response properties will vary according to context.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



