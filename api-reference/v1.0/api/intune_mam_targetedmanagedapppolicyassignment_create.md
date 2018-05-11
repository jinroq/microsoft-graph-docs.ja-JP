# <a name="create-targetedmanagedapppolicyassignment"></a><span data-ttu-id="513c0-101">targetedManagedAppPolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="513c0-101">Create targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="513c0-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="513c0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="513c0-103">新しい [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="513c0-103">Create a new [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="513c0-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="513c0-104">Prerequisites</span></span>
<span data-ttu-id="513c0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="513c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="513c0-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="513c0-107">Permission type</span></span>|<span data-ttu-id="513c0-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="513c0-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="513c0-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="513c0-109">Delegated (work or school account)</span></span>|<span data-ttu-id="513c0-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="513c0-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="513c0-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="513c0-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="513c0-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="513c0-112">Not supported.</span></span>|
|<span data-ttu-id="513c0-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="513c0-113">Application</span></span>|<span data-ttu-id="513c0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="513c0-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="513c0-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="513c0-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
POST /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="513c0-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="513c0-116">Request headers</span></span>
|<span data-ttu-id="513c0-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="513c0-117">Header</span></span>|<span data-ttu-id="513c0-118">値</span><span class="sxs-lookup"><span data-stu-id="513c0-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="513c0-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="513c0-119">Authorization</span></span>|<span data-ttu-id="513c0-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="513c0-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="513c0-121">Accept</span><span class="sxs-lookup"><span data-stu-id="513c0-121">Accept</span></span>|<span data-ttu-id="513c0-122">application/json</span><span class="sxs-lookup"><span data-stu-id="513c0-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="513c0-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="513c0-123">Request body</span></span>
<span data-ttu-id="513c0-124">要求本文で、targetedManagedAppPolicyAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="513c0-124">In the request body, supply a JSON representation for the targetedManagedAppPolicyAssignment object.</span></span>

<span data-ttu-id="513c0-125">次の表に、targetedManagedAppPolicyAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="513c0-125">The following table shows the properties that are required when you create the targetedManagedAppPolicyAssignment.</span></span>

|<span data-ttu-id="513c0-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="513c0-126">Property</span></span>|<span data-ttu-id="513c0-127">型</span><span class="sxs-lookup"><span data-stu-id="513c0-127">Type</span></span>|<span data-ttu-id="513c0-128">説明</span><span class="sxs-lookup"><span data-stu-id="513c0-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="513c0-129">id</span><span class="sxs-lookup"><span data-stu-id="513c0-129">id</span></span>|<span data-ttu-id="513c0-130">String</span><span class="sxs-lookup"><span data-stu-id="513c0-130">String</span></span>|<span data-ttu-id="513c0-131">ID</span><span class="sxs-lookup"><span data-stu-id="513c0-131">Id</span></span>|
|<span data-ttu-id="513c0-132">target</span><span class="sxs-lookup"><span data-stu-id="513c0-132">target</span></span>|[<span data-ttu-id="513c0-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="513c0-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_mam_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="513c0-134">グループまたはアプリの展開の識別子</span><span class="sxs-lookup"><span data-stu-id="513c0-134">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="513c0-135">応答</span><span class="sxs-lookup"><span data-stu-id="513c0-135">Response</span></span>
<span data-ttu-id="513c0-136">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="513c0-136">If successful, this method returns a `201 Created` response code and a [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="513c0-137">例</span><span class="sxs-lookup"><span data-stu-id="513c0-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="513c0-138">要求</span><span class="sxs-lookup"><span data-stu-id="513c0-138">Request</span></span>
<span data-ttu-id="513c0-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="513c0-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="513c0-140">応答</span><span class="sxs-lookup"><span data-stu-id="513c0-140">Response</span></span>
<span data-ttu-id="513c0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="513c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



