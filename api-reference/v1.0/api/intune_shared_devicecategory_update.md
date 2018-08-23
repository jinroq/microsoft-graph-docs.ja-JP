# <a name="update-devicecategory"></a><span data-ttu-id="ed13b-101">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="ed13b-101">Update deviceCategory</span></span>

> <span data-ttu-id="ed13b-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ed13b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed13b-103">[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ed13b-103">Update the properties of a [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ed13b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ed13b-104">Prerequisites</span></span>
<span data-ttu-id="ed13b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ed13b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ed13b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ed13b-107">Permission type</span></span>|<span data-ttu-id="ed13b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ed13b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed13b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ed13b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ed13b-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed13b-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ed13b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ed13b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed13b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed13b-112">Not supported.</span></span>|
|<span data-ttu-id="ed13b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ed13b-113">Application</span></span>|<span data-ttu-id="ed13b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ed13b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed13b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ed13b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
```

## <a name="request-headers"></a><span data-ttu-id="ed13b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed13b-116">Request headers</span></span>
|<span data-ttu-id="ed13b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ed13b-117">Header</span></span>|<span data-ttu-id="ed13b-118">値</span><span class="sxs-lookup"><span data-stu-id="ed13b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ed13b-119">承認</span><span class="sxs-lookup"><span data-stu-id="ed13b-119">Authorization</span></span>|<span data-ttu-id="ed13b-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ed13b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ed13b-121">受諾</span><span class="sxs-lookup"><span data-stu-id="ed13b-121">Accept</span></span>|<span data-ttu-id="ed13b-122">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="ed13b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed13b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ed13b-123">Request body</span></span>
<span data-ttu-id="ed13b-124">要求本文で、[deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ed13b-124">In the request body, supply a JSON representation for the [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>

<span data-ttu-id="ed13b-125">次の表に、[deviceCategory](../resources/intune_shared_devicecategory.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ed13b-125">The following table shows the properties that are required when you create the [deviceCategory](../resources/intune_shared_devicecategory.md).</span></span>

|<span data-ttu-id="ed13b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ed13b-126">Property</span></span>|<span data-ttu-id="ed13b-127">型</span><span class="sxs-lookup"><span data-stu-id="ed13b-127">Type</span></span>|<span data-ttu-id="ed13b-128">説明</span><span class="sxs-lookup"><span data-stu-id="ed13b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed13b-129">id</span><span class="sxs-lookup"><span data-stu-id="ed13b-129">id</span></span>|<span data-ttu-id="ed13b-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ed13b-130">String</span></span>|<span data-ttu-id="ed13b-131">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ed13b-131">Unique identifier for the device category.</span></span> <span data-ttu-id="ed13b-132">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ed13b-132">Read-only.</span></span>|
|<span data-ttu-id="ed13b-133">**採用**</span><span class="sxs-lookup"><span data-stu-id="ed13b-133">**On-boarding**</span></span>|
|<span data-ttu-id="ed13b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ed13b-134">displayName</span></span>|<span data-ttu-id="ed13b-135">文字列</span><span class="sxs-lookup"><span data-stu-id="ed13b-135">String</span></span>|<span data-ttu-id="ed13b-136">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="ed13b-136">Display name for the device category.</span></span>|
|<span data-ttu-id="ed13b-137">説明</span><span class="sxs-lookup"><span data-stu-id="ed13b-137">description</span></span>|<span data-ttu-id="ed13b-138">文字列</span><span class="sxs-lookup"><span data-stu-id="ed13b-138">String</span></span>|<span data-ttu-id="ed13b-139">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="ed13b-139">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="ed13b-140">応答</span><span class="sxs-lookup"><span data-stu-id="ed13b-140">Response</span></span>
<span data-ttu-id="ed13b-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ed13b-141">If successful, this method returns a `200 OK` response code and an updated [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed13b-142">例</span><span class="sxs-lookup"><span data-stu-id="ed13b-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="ed13b-143">要求</span><span class="sxs-lookup"><span data-stu-id="ed13b-143">Request</span></span>
<span data-ttu-id="ed13b-144">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ed13b-144">Here are a couple of examples of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ed13b-145">応答</span><span class="sxs-lookup"><span data-stu-id="ed13b-145">Response</span></span>
<span data-ttu-id="ed13b-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ed13b-146">Here is an example of the response.</span></span> <span data-ttu-id="ed13b-147">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="ed13b-147">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ed13b-148">応答のプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="ed13b-148">Response properties will vary according to context.</span></span>
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



