# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="0f711-101">deviceConfigurationUserOverview の更新</span><span class="sxs-lookup"><span data-stu-id="0f711-101">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="0f711-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0f711-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f711-103">[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f711-103">Update the properties of a [calendar](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0f711-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f711-104">Prerequisites</span></span>
<span data-ttu-id="0f711-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0f711-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f711-107">Permission type</span></span>|<span data-ttu-id="0f711-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f711-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f711-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f711-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0f711-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f711-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0f711-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f711-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f711-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f711-112">Not supported.</span></span>|
|<span data-ttu-id="0f711-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f711-113">Application</span></span>|<span data-ttu-id="0f711-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f711-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f711-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f711-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="0f711-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f711-116">Request headers</span></span>
|<span data-ttu-id="0f711-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f711-117">Header</span></span>|<span data-ttu-id="0f711-118">値</span><span class="sxs-lookup"><span data-stu-id="0f711-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f711-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f711-119">Authorization</span></span>|<span data-ttu-id="0f711-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f711-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0f711-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0f711-121">Accept</span></span>|<span data-ttu-id="0f711-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0f711-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f711-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f711-123">Request body</span></span>
<span data-ttu-id="0f711-124">要求本文で、[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f711-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="0f711-125">次の表に、[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0f711-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="0f711-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f711-126">Property</span></span>|<span data-ttu-id="0f711-127">型</span><span class="sxs-lookup"><span data-stu-id="0f711-127">Type</span></span>|<span data-ttu-id="0f711-128">説明</span><span class="sxs-lookup"><span data-stu-id="0f711-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f711-129">id</span><span class="sxs-lookup"><span data-stu-id="0f711-129">id</span></span>|<span data-ttu-id="0f711-130">String</span><span class="sxs-lookup"><span data-stu-id="0f711-130">String</span></span>|<span data-ttu-id="0f711-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0f711-131">Name of the entity.</span></span>|
|<span data-ttu-id="0f711-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="0f711-132">pendingCount</span></span>|<span data-ttu-id="0f711-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0f711-133">Int32</span></span>|<span data-ttu-id="0f711-134">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0f711-134">Number of pending Users</span></span>|
|<span data-ttu-id="0f711-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="0f711-135">notApplicableCount</span></span>|<span data-ttu-id="0f711-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0f711-136">Int32</span></span>|<span data-ttu-id="0f711-137">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="0f711-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="0f711-138">successCount</span><span class="sxs-lookup"><span data-stu-id="0f711-138">successCount</span></span>|<span data-ttu-id="0f711-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0f711-139">Int32</span></span>|<span data-ttu-id="0f711-140">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0f711-140">Number of succeeded Users</span></span>|
|<span data-ttu-id="0f711-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="0f711-141">errorCount</span></span>|<span data-ttu-id="0f711-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0f711-142">Int32</span></span>|<span data-ttu-id="0f711-143">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0f711-143">Number of error Users</span></span>|
|<span data-ttu-id="0f711-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="0f711-144">failedCount</span></span>|<span data-ttu-id="0f711-145">Int32</span><span class="sxs-lookup"><span data-stu-id="0f711-145">Int32</span></span>|<span data-ttu-id="0f711-146">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="0f711-146">Number of failed Users</span></span>|
|<span data-ttu-id="0f711-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="0f711-147">lastUpdateDateTime</span></span>|<span data-ttu-id="0f711-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f711-148">DateTimeOffset</span></span>|<span data-ttu-id="0f711-149">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="0f711-149">Last update time</span></span>|
|<span data-ttu-id="0f711-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="0f711-150">configurationVersion</span></span>|<span data-ttu-id="0f711-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0f711-151">Int32</span></span>|<span data-ttu-id="0f711-152">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="0f711-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="0f711-153">応答</span><span class="sxs-lookup"><span data-stu-id="0f711-153">Response</span></span>
<span data-ttu-id="0f711-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f711-154">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f711-155">例</span><span class="sxs-lookup"><span data-stu-id="0f711-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="0f711-156">要求</span><span class="sxs-lookup"><span data-stu-id="0f711-156">Request</span></span>
<span data-ttu-id="0f711-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f711-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
Content-type: application/json
Content-length: 212

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="0f711-158">応答</span><span class="sxs-lookup"><span data-stu-id="0f711-158">Response</span></span>
<span data-ttu-id="0f711-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f711-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 331

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserOverview",
  "id": "000e52d7-52d7-000e-d752-0e00d7520e00",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



