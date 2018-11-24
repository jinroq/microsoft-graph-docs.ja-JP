# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="7082d-101">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="7082d-101">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="7082d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7082d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7082d-103">[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7082d-103">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7082d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="7082d-104">Prerequisites</span></span>
<span data-ttu-id="7082d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7082d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7082d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7082d-107">Permission type</span></span>|<span data-ttu-id="7082d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7082d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7082d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7082d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7082d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7082d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7082d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7082d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7082d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7082d-112">Not supported.</span></span>|
|<span data-ttu-id="7082d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7082d-113">Application</span></span>|<span data-ttu-id="7082d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7082d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7082d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7082d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7082d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7082d-116">Request headers</span></span>
|<span data-ttu-id="7082d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7082d-117">Header</span></span>|<span data-ttu-id="7082d-118">値</span><span class="sxs-lookup"><span data-stu-id="7082d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7082d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7082d-119">Authorization</span></span>|<span data-ttu-id="7082d-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7082d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7082d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7082d-121">Accept</span></span>|<span data-ttu-id="7082d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7082d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7082d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7082d-123">Request body</span></span>
<span data-ttu-id="7082d-124">要求本文で、[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7082d-124">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="7082d-125">次の表に、[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7082d-125">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="7082d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7082d-126">Property</span></span>|<span data-ttu-id="7082d-127">型</span><span class="sxs-lookup"><span data-stu-id="7082d-127">Type</span></span>|<span data-ttu-id="7082d-128">説明</span><span class="sxs-lookup"><span data-stu-id="7082d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7082d-129">id</span><span class="sxs-lookup"><span data-stu-id="7082d-129">id</span></span>|<span data-ttu-id="7082d-130">String</span><span class="sxs-lookup"><span data-stu-id="7082d-130">String</span></span>|<span data-ttu-id="7082d-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7082d-131">Key of the entity.</span></span>|
|<span data-ttu-id="7082d-132">target</span><span class="sxs-lookup"><span data-stu-id="7082d-132">target</span></span>|[<span data-ttu-id="7082d-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7082d-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7082d-134">コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="7082d-134">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="7082d-135">応答</span><span class="sxs-lookup"><span data-stu-id="7082d-135">Response</span></span>
<span data-ttu-id="7082d-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7082d-136">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7082d-137">例</span><span class="sxs-lookup"><span data-stu-id="7082d-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="7082d-138">要求</span><span class="sxs-lookup"><span data-stu-id="7082d-138">Request</span></span>
<span data-ttu-id="7082d-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7082d-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="7082d-140">応答</span><span class="sxs-lookup"><span data-stu-id="7082d-140">Response</span></span>
<span data-ttu-id="7082d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7082d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



