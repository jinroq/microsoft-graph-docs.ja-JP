# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="ce4f9-101">deviceComplianceUserStatus の作成</span><span class="sxs-lookup"><span data-stu-id="ce4f9-101">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="ce4f9-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce4f9-103">新しい [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce4f9-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce4f9-104">Prerequisites</span></span>
<span data-ttu-id="ce4f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ce4f9-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce4f9-107">Permission type</span></span>|<span data-ttu-id="ce4f9-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce4f9-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce4f9-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce4f9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ce4f9-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce4f9-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ce4f9-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce4f9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce4f9-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-112">Not supported.</span></span>|
|<span data-ttu-id="ce4f9-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce4f9-113">Application</span></span>|<span data-ttu-id="ce4f9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce4f9-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce4f9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="ce4f9-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce4f9-116">Request headers</span></span>
|<span data-ttu-id="ce4f9-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce4f9-117">Header</span></span>|<span data-ttu-id="ce4f9-118">値</span><span class="sxs-lookup"><span data-stu-id="ce4f9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce4f9-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce4f9-119">Authorization</span></span>|<span data-ttu-id="ce4f9-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ce4f9-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ce4f9-121">Accept</span></span>|<span data-ttu-id="ce4f9-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ce4f9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce4f9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce4f9-123">Request body</span></span>
<span data-ttu-id="ce4f9-124">要求本文で、deviceComplianceUserStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ce4f9-125">次の表に、deviceComplianceUserStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ce4f9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce4f9-126">Property</span></span>|<span data-ttu-id="ce4f9-127">型</span><span class="sxs-lookup"><span data-stu-id="ce4f9-127">Type</span></span>|<span data-ttu-id="ce4f9-128">説明</span><span class="sxs-lookup"><span data-stu-id="ce4f9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce4f9-129">id</span><span class="sxs-lookup"><span data-stu-id="ce4f9-129">id</span></span>|<span data-ttu-id="ce4f9-130">String</span><span class="sxs-lookup"><span data-stu-id="ce4f9-130">String</span></span>|<span data-ttu-id="ce4f9-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-131">Name of the entity.</span></span>|
|<span data-ttu-id="ce4f9-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="ce4f9-132">userDisplayName</span></span>|<span data-ttu-id="ce4f9-133">String</span><span class="sxs-lookup"><span data-stu-id="ce4f9-133">String</span></span>|<span data-ttu-id="ce4f9-134">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="ce4f9-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="ce4f9-135">devicesCount</span></span>|<span data-ttu-id="ce4f9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="ce4f9-136">Int32</span></span>|<span data-ttu-id="ce4f9-137">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-137">Devices count for that user.</span></span>|
|<span data-ttu-id="ce4f9-138">status</span><span class="sxs-lookup"><span data-stu-id="ce4f9-138">status</span></span>|<span data-ttu-id="ce4f9-139">String</span><span class="sxs-lookup"><span data-stu-id="ce4f9-139">String</span></span>|<span data-ttu-id="ce4f9-140">ポリシー レポートのコンプライアンスの状態。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-140">Compliance status of the policy report.</span></span> <span data-ttu-id="ce4f9-141">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="ce4f9-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce4f9-142">lastReportedDateTime</span></span>|<span data-ttu-id="ce4f9-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce4f9-143">DateTimeOffset</span></span>|<span data-ttu-id="ce4f9-144">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="ce4f9-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ce4f9-145">userPrincipalName</span></span>|<span data-ttu-id="ce4f9-146">String</span><span class="sxs-lookup"><span data-stu-id="ce4f9-146">String</span></span>|<span data-ttu-id="ce4f9-147">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-147">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="ce4f9-148">応答</span><span class="sxs-lookup"><span data-stu-id="ce4f9-148">Response</span></span>
<span data-ttu-id="ce4f9-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-149">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce4f9-150">例</span><span class="sxs-lookup"><span data-stu-id="ce4f9-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce4f9-151">要求</span><span class="sxs-lookup"><span data-stu-id="ce4f9-151">Request</span></span>
<span data-ttu-id="ce4f9-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
Content-type: application/json
Content-length: 287

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="ce4f9-153">応答</span><span class="sxs-lookup"><span data-stu-id="ce4f9-153">Response</span></span>
<span data-ttu-id="ce4f9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce4f9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 336

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "a0b566cd-66cd-a0b5-cd66-b5a0cd66b5a0",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



