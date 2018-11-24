# <a name="create-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="1d768-101">managedDeviceMobileAppConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="1d768-101">Create managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="1d768-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d768-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d768-103">新しい [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1d768-103">Create a new [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1d768-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="1d768-104">Prerequisites</span></span>
<span data-ttu-id="1d768-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d768-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1d768-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d768-107">Permission type</span></span>|<span data-ttu-id="1d768-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d768-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d768-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d768-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1d768-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d768-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1d768-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d768-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d768-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d768-112">Not supported.</span></span>|
|<span data-ttu-id="1d768-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d768-113">Application</span></span>|<span data-ttu-id="1d768-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d768-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d768-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d768-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1d768-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d768-116">Request headers</span></span>
|<span data-ttu-id="1d768-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d768-117">Header</span></span>|<span data-ttu-id="1d768-118">値</span><span class="sxs-lookup"><span data-stu-id="1d768-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d768-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d768-119">Authorization</span></span>|<span data-ttu-id="1d768-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1d768-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d768-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1d768-121">Accept</span></span>|<span data-ttu-id="1d768-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1d768-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d768-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d768-123">Request body</span></span>
<span data-ttu-id="1d768-124">要求本文で、managedDeviceMobileAppConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d768-124">In the request body, supply a JSON representation for the managedDeviceMobileAppConfigurationAssignment object.</span></span>

<span data-ttu-id="1d768-125">次の表に、managedDeviceMobileAppConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1d768-125">The following table shows the properties that are required when you create the managedDeviceMobileAppConfigurationAssignment.</span></span>

|<span data-ttu-id="1d768-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d768-126">Property</span></span>|<span data-ttu-id="1d768-127">型</span><span class="sxs-lookup"><span data-stu-id="1d768-127">Type</span></span>|<span data-ttu-id="1d768-128">説明</span><span class="sxs-lookup"><span data-stu-id="1d768-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d768-129">id</span><span class="sxs-lookup"><span data-stu-id="1d768-129">id</span></span>|<span data-ttu-id="1d768-130">String</span><span class="sxs-lookup"><span data-stu-id="1d768-130">String</span></span>|<span data-ttu-id="1d768-131">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1d768-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="1d768-132">target</span><span class="sxs-lookup"><span data-stu-id="1d768-132">target</span></span>|[<span data-ttu-id="1d768-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1d768-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1d768-134">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="1d768-134">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="1d768-135">応答</span><span class="sxs-lookup"><span data-stu-id="1d768-135">Response</span></span>
<span data-ttu-id="1d768-136">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1d768-136">If successful, this method returns a `201 Created` response code and a [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d768-137">例</span><span class="sxs-lookup"><span data-stu-id="1d768-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="1d768-138">要求</span><span class="sxs-lookup"><span data-stu-id="1d768-138">Request</span></span>
<span data-ttu-id="1d768-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1d768-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="1d768-140">応答</span><span class="sxs-lookup"><span data-stu-id="1d768-140">Response</span></span>
<span data-ttu-id="1d768-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d768-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
  "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



