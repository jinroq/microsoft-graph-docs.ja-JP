# <a name="update-managedmobileapp"></a><span data-ttu-id="8c2f1-101">managedMobileApp の更新</span><span class="sxs-lookup"><span data-stu-id="8c2f1-101">Update managedMobileApp</span></span>

> <span data-ttu-id="8c2f1-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c2f1-103">[managedMobileApp](../resources/intune_mam_managedmobileapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-103">Update the properties of a [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c2f1-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="8c2f1-104">Prerequisites</span></span>
<span data-ttu-id="8c2f1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8c2f1-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c2f1-107">Permission type</span></span>|<span data-ttu-id="8c2f1-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c2f1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c2f1-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c2f1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8c2f1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c2f1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8c2f1-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c2f1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c2f1-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-112">Not supported.</span></span>|
|<span data-ttu-id="8c2f1-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c2f1-113">Application</span></span>|<span data-ttu-id="8c2f1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c2f1-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c2f1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="8c2f1-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c2f1-116">Request headers</span></span>
|<span data-ttu-id="8c2f1-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c2f1-117">Header</span></span>|<span data-ttu-id="8c2f1-118">値</span><span class="sxs-lookup"><span data-stu-id="8c2f1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c2f1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c2f1-119">Authorization</span></span>|<span data-ttu-id="8c2f1-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c2f1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8c2f1-121">Accept</span></span>|<span data-ttu-id="8c2f1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8c2f1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c2f1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c2f1-123">Request body</span></span>
<span data-ttu-id="8c2f1-124">要求本文で、[managedMobileApp](../resources/intune_mam_managedmobileapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-124">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>

<span data-ttu-id="8c2f1-125">次の表に、[managedMobileApp](../resources/intune_mam_managedmobileapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-125">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span></span>

|<span data-ttu-id="8c2f1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c2f1-126">Property</span></span>|<span data-ttu-id="8c2f1-127">型</span><span class="sxs-lookup"><span data-stu-id="8c2f1-127">Type</span></span>|<span data-ttu-id="8c2f1-128">説明</span><span class="sxs-lookup"><span data-stu-id="8c2f1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c2f1-129">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8c2f1-129">mobileAppIdentifier</span></span>|[<span data-ttu-id="8c2f1-130">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8c2f1-130">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="8c2f1-131">対象のオペレーティング システムの種類のアプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-131">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="8c2f1-132">id</span><span class="sxs-lookup"><span data-stu-id="8c2f1-132">id</span></span>|<span data-ttu-id="8c2f1-133">String</span><span class="sxs-lookup"><span data-stu-id="8c2f1-133">String</span></span>|<span data-ttu-id="8c2f1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-134">Key of the entity.</span></span>|
|<span data-ttu-id="8c2f1-135">version</span><span class="sxs-lookup"><span data-stu-id="8c2f1-135">version</span></span>|<span data-ttu-id="8c2f1-136">String</span><span class="sxs-lookup"><span data-stu-id="8c2f1-136">String</span></span>|<span data-ttu-id="8c2f1-137">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-137">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="8c2f1-138">応答</span><span class="sxs-lookup"><span data-stu-id="8c2f1-138">Response</span></span>
<span data-ttu-id="8c2f1-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedMobileApp](../resources/intune_mam_managedmobileapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-139">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c2f1-140">例</span><span class="sxs-lookup"><span data-stu-id="8c2f1-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c2f1-141">要求</span><span class="sxs-lookup"><span data-stu-id="8c2f1-141">Request</span></span>
<span data-ttu-id="8c2f1-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="8c2f1-143">応答</span><span class="sxs-lookup"><span data-stu-id="8c2f1-143">Response</span></span>
<span data-ttu-id="8c2f1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c2f1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```



