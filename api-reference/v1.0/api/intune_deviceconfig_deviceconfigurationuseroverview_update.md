# <a name="update-deviceconfigurationuseroverview"></a><span data-ttu-id="53b91-101">deviceConfigurationUserOverview の更新</span><span class="sxs-lookup"><span data-stu-id="53b91-101">Update deviceConfigurationUserOverview</span></span>

> <span data-ttu-id="53b91-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="53b91-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="53b91-103">[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="53b91-103">Update the properties of a [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="53b91-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="53b91-104">Prerequisites</span></span>
<span data-ttu-id="53b91-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53b91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="53b91-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53b91-107">Permission type</span></span>|<span data-ttu-id="53b91-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="53b91-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53b91-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53b91-109">Delegated (work or school account)</span></span>|<span data-ttu-id="53b91-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53b91-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="53b91-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53b91-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53b91-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53b91-112">Not supported.</span></span>|
|<span data-ttu-id="53b91-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53b91-113">Application</span></span>|<span data-ttu-id="53b91-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53b91-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53b91-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53b91-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="53b91-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53b91-116">Request headers</span></span>
|<span data-ttu-id="53b91-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53b91-117">Header</span></span>|<span data-ttu-id="53b91-118">値</span><span class="sxs-lookup"><span data-stu-id="53b91-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53b91-119">承認</span><span class="sxs-lookup"><span data-stu-id="53b91-119">Authorization</span></span>|<span data-ttu-id="53b91-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="53b91-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53b91-121">受託</span><span class="sxs-lookup"><span data-stu-id="53b91-121">Accept</span></span>|<span data-ttu-id="53b91-122">application/json</span><span class="sxs-lookup"><span data-stu-id="53b91-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53b91-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="53b91-123">Request body</span></span>
<span data-ttu-id="53b91-124">要求本文で、[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="53b91-124">In the request body, supply a JSON representation for the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object.</span></span>

<span data-ttu-id="53b91-125">次の表に、[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="53b91-125">The following table shows the properties that are required when you create the [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md).</span></span>

|<span data-ttu-id="53b91-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53b91-126">Property</span></span>|<span data-ttu-id="53b91-127">型</span><span class="sxs-lookup"><span data-stu-id="53b91-127">Type</span></span>|<span data-ttu-id="53b91-128">説明</span><span class="sxs-lookup"><span data-stu-id="53b91-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53b91-129">id</span><span class="sxs-lookup"><span data-stu-id="53b91-129">id</span></span>|<span data-ttu-id="53b91-130">文字列</span><span class="sxs-lookup"><span data-stu-id="53b91-130">String</span></span>|<span data-ttu-id="53b91-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="53b91-131">Key of the entity.</span></span>|
|<span data-ttu-id="53b91-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="53b91-132">pendingCount</span></span>|<span data-ttu-id="53b91-133">Int32</span><span class="sxs-lookup"><span data-stu-id="53b91-133">Int32</span></span>|<span data-ttu-id="53b91-134">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="53b91-134">Number of pending Users</span></span>|
|<span data-ttu-id="53b91-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="53b91-135">notApplicableCount</span></span>|<span data-ttu-id="53b91-136">Int32</span><span class="sxs-lookup"><span data-stu-id="53b91-136">Int32</span></span>|<span data-ttu-id="53b91-137">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="53b91-137">Number of not applicable users.</span></span>|
|<span data-ttu-id="53b91-138">successCount</span><span class="sxs-lookup"><span data-stu-id="53b91-138">successCount</span></span>|<span data-ttu-id="53b91-139">Int32</span><span class="sxs-lookup"><span data-stu-id="53b91-139">Int32</span></span>|<span data-ttu-id="53b91-140">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="53b91-140">Number of succeeded Users</span></span>|
|<span data-ttu-id="53b91-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="53b91-141">errorCount</span></span>|<span data-ttu-id="53b91-142">Int32</span><span class="sxs-lookup"><span data-stu-id="53b91-142">Int32</span></span>|<span data-ttu-id="53b91-143">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="53b91-143">Number of error Users</span></span>|
|<span data-ttu-id="53b91-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="53b91-144">failedCount</span></span>|<span data-ttu-id="53b91-145">Int32</span><span class="sxs-lookup"><span data-stu-id="53b91-145">Int32</span></span>|<span data-ttu-id="53b91-146">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="53b91-146">Number of failed Users</span></span>|
|<span data-ttu-id="53b91-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="53b91-147">lastUpdateDateTime</span></span>|<span data-ttu-id="53b91-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53b91-148">DateTimeOffset</span></span>|<span data-ttu-id="53b91-149">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="53b91-149">Last update time</span></span>|
|<span data-ttu-id="53b91-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="53b91-150">configurationVersion</span></span>|<span data-ttu-id="53b91-151">Int32</span><span class="sxs-lookup"><span data-stu-id="53b91-151">Int32</span></span>|<span data-ttu-id="53b91-152">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="53b91-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="53b91-153">応答</span><span class="sxs-lookup"><span data-stu-id="53b91-153">Response</span></span>
<span data-ttu-id="53b91-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="53b91-154">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53b91-155">例</span><span class="sxs-lookup"><span data-stu-id="53b91-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="53b91-156">要求</span><span class="sxs-lookup"><span data-stu-id="53b91-156">Request</span></span>
<span data-ttu-id="53b91-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53b91-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53b91-158">応答</span><span class="sxs-lookup"><span data-stu-id="53b91-158">Response</span></span>
<span data-ttu-id="53b91-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53b91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



