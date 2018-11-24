# <a name="create-devicecategory"></a><span data-ttu-id="7052a-101">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="7052a-101">Create deviceCategory</span></span>

> <span data-ttu-id="7052a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7052a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7052a-103">新しい [deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7052a-103">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7052a-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7052a-104">Prerequisites</span></span>
<span data-ttu-id="7052a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7052a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7052a-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7052a-107">Permission type</span></span>|<span data-ttu-id="7052a-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7052a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7052a-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7052a-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7052a-110">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="7052a-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="7052a-111">DeviceManagementManaged Devices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7052a-111">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="7052a-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7052a-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7052a-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7052a-113">Not supported.</span></span>|
|<span data-ttu-id="7052a-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7052a-114">Application</span></span>|<span data-ttu-id="7052a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7052a-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7052a-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7052a-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="7052a-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7052a-117">Request headers</span></span>
|<span data-ttu-id="7052a-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7052a-118">Header</span></span>|<span data-ttu-id="7052a-119">値</span><span class="sxs-lookup"><span data-stu-id="7052a-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7052a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7052a-120">Authorization</span></span>|<span data-ttu-id="7052a-121">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7052a-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7052a-122">Accept</span><span class="sxs-lookup"><span data-stu-id="7052a-122">Accept</span></span>|<span data-ttu-id="7052a-123">application/json</span><span class="sxs-lookup"><span data-stu-id="7052a-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7052a-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="7052a-124">Request body</span></span>
<span data-ttu-id="7052a-125">要求本文で、deviceCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7052a-125">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="7052a-126">次の表に、deviceCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7052a-126">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="7052a-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7052a-127">Property</span></span>|<span data-ttu-id="7052a-128">型</span><span class="sxs-lookup"><span data-stu-id="7052a-128">Type</span></span>|<span data-ttu-id="7052a-129">説明</span><span class="sxs-lookup"><span data-stu-id="7052a-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7052a-130">id</span><span class="sxs-lookup"><span data-stu-id="7052a-130">id</span></span>|<span data-ttu-id="7052a-131">文字列</span><span class="sxs-lookup"><span data-stu-id="7052a-131">String</span></span>|<span data-ttu-id="7052a-132">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7052a-132">Unique identifier for the device category.</span></span> <span data-ttu-id="7052a-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="7052a-133">Read-only.</span></span>|
|<span data-ttu-id="7052a-134">**契約時**</span><span class="sxs-lookup"><span data-stu-id="7052a-134">**Onboarding**</span></span>|
|<span data-ttu-id="7052a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7052a-135">displayName</span></span>|<span data-ttu-id="7052a-136">String</span><span class="sxs-lookup"><span data-stu-id="7052a-136">String</span></span>|<span data-ttu-id="7052a-137">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="7052a-137">Display name for the device category.</span></span>|
|<span data-ttu-id="7052a-138">説明</span><span class="sxs-lookup"><span data-stu-id="7052a-138">description</span></span>|<span data-ttu-id="7052a-139">String</span><span class="sxs-lookup"><span data-stu-id="7052a-139">String</span></span>|<span data-ttu-id="7052a-140">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="7052a-140">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="7052a-141">応答</span><span class="sxs-lookup"><span data-stu-id="7052a-141">Response</span></span>
<span data-ttu-id="7052a-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCategory](../resources/intune_shared_devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7052a-142">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7052a-143">例</span><span class="sxs-lookup"><span data-stu-id="7052a-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="7052a-144">要求</span><span class="sxs-lookup"><span data-stu-id="7052a-144">Request</span></span>
<span data-ttu-id="7052a-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7052a-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="7052a-146">応答</span><span class="sxs-lookup"><span data-stu-id="7052a-146">Response</span></span>
<span data-ttu-id="7052a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7052a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



