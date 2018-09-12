# <a name="create-devicecomplianceuserstatus"></a><span data-ttu-id="cf9b6-101">deviceComplianceUserStatus の作成</span><span class="sxs-lookup"><span data-stu-id="cf9b6-101">Create deviceComplianceUserStatus</span></span>

> <span data-ttu-id="cf9b6-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf9b6-103">新しい [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-103">Create a new [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf9b6-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="cf9b6-104">Prerequisites</span></span>
<span data-ttu-id="cf9b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf9b6-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf9b6-107">Permission type</span></span>|<span data-ttu-id="cf9b6-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf9b6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf9b6-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf9b6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cf9b6-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf9b6-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf9b6-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf9b6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf9b6-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-112">Not supported.</span></span>|
|<span data-ttu-id="cf9b6-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf9b6-113">Application</span></span>|<span data-ttu-id="cf9b6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf9b6-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf9b6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="cf9b6-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf9b6-116">Request headers</span></span>
|<span data-ttu-id="cf9b6-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf9b6-117">Header</span></span>|<span data-ttu-id="cf9b6-118">値</span><span class="sxs-lookup"><span data-stu-id="cf9b6-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf9b6-119">承認</span><span class="sxs-lookup"><span data-stu-id="cf9b6-119">Authorization</span></span>|<span data-ttu-id="cf9b6-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf9b6-121">承諾</span><span class="sxs-lookup"><span data-stu-id="cf9b6-121">Accept</span></span>|<span data-ttu-id="cf9b6-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cf9b6-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf9b6-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf9b6-123">Request body</span></span>
<span data-ttu-id="cf9b6-124">要求本文で、deviceComplianceUserStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-124">In the request body, supply a JSON representation for the deviceComplianceUserStatus object.</span></span>

<span data-ttu-id="cf9b6-125">次の表に、deviceComplianceUserStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-125">The following table shows the properties that are required when you create the deviceComplianceUserStatus.</span></span>

|<span data-ttu-id="cf9b6-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf9b6-126">Property</span></span>|<span data-ttu-id="cf9b6-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="cf9b6-127">Type</span></span>|<span data-ttu-id="cf9b6-128">説明</span><span class="sxs-lookup"><span data-stu-id="cf9b6-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf9b6-129">id</span><span class="sxs-lookup"><span data-stu-id="cf9b6-129">id</span></span>|<span data-ttu-id="cf9b6-130">文字列</span><span class="sxs-lookup"><span data-stu-id="cf9b6-130">String</span></span>|<span data-ttu-id="cf9b6-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-131">Key of the entity.</span></span>|
|<span data-ttu-id="cf9b6-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="cf9b6-132">userDisplayName</span></span>|<span data-ttu-id="cf9b6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="cf9b6-133">String</span></span>|<span data-ttu-id="cf9b6-134">DevicePolicyStatus のユーザー名。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="cf9b6-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="cf9b6-135">devicesCount</span></span>|<span data-ttu-id="cf9b6-136">Int32</span><span class="sxs-lookup"><span data-stu-id="cf9b6-136">Int32</span></span>|<span data-ttu-id="cf9b6-137">そのユーザーのデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-137">Devices count for that user.</span></span>|
|<span data-ttu-id="cf9b6-138">状態</span><span class="sxs-lookup"><span data-stu-id="cf9b6-138">status</span></span>|[<span data-ttu-id="cf9b6-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="cf9b6-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="cf9b6-p102">コンプライアンス ポリシー レポートの状態。使用可能な値は `unknown`、 `notApplicable`、 `compliant`、 `remediated`、 `nonCompliant`、 `error`、 `conflict`、 `notAssigned`です。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-p102">Compliance status of the policy report. The possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="cf9b6-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf9b6-142">lastReportedDateTime</span></span>|<span data-ttu-id="cf9b6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf9b6-143">DateTimeOffset</span></span>|<span data-ttu-id="cf9b6-144">ポリシー レポートの最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="cf9b6-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cf9b6-145">userPrincipalName</span></span>|<span data-ttu-id="cf9b6-146">文字列</span><span class="sxs-lookup"><span data-stu-id="cf9b6-146">String</span></span>|<span data-ttu-id="cf9b6-147">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="cf9b6-148">応答</span><span class="sxs-lookup"><span data-stu-id="cf9b6-148">Response</span></span>
<span data-ttu-id="cf9b6-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf9b6-150">例</span><span class="sxs-lookup"><span data-stu-id="cf9b6-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf9b6-151">要求</span><span class="sxs-lookup"><span data-stu-id="cf9b6-151">Request</span></span>
<span data-ttu-id="cf9b6-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="cf9b6-153">応答</span><span class="sxs-lookup"><span data-stu-id="cf9b6-153">Response</span></span>
<span data-ttu-id="cf9b6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf9b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








