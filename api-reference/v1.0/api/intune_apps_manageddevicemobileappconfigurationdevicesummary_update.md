# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="accd9-101">managedDeviceMobileAppConfigurationDeviceSummary の更新</span><span class="sxs-lookup"><span data-stu-id="accd9-101">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="accd9-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="accd9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="accd9-103">[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="accd9-103">Update the properties of a [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="accd9-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="accd9-104">Prerequisites</span></span>
<span data-ttu-id="accd9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="accd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="accd9-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="accd9-107">Permission type</span></span>|<span data-ttu-id="accd9-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="accd9-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="accd9-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="accd9-109">Delegated (work or school account)</span></span>|<span data-ttu-id="accd9-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="accd9-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="accd9-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="accd9-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="accd9-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="accd9-112">Not supported.</span></span>|
|<span data-ttu-id="accd9-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="accd9-113">Application</span></span>|<span data-ttu-id="accd9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="accd9-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="accd9-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="accd9-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="accd9-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="accd9-116">Request headers</span></span>
|<span data-ttu-id="accd9-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="accd9-117">Header</span></span>|<span data-ttu-id="accd9-118">値</span><span class="sxs-lookup"><span data-stu-id="accd9-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="accd9-119">承認</span><span class="sxs-lookup"><span data-stu-id="accd9-119">Authorization</span></span>|<span data-ttu-id="accd9-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="accd9-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="accd9-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="accd9-121">Accept</span></span>|<span data-ttu-id="accd9-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="accd9-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="accd9-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="accd9-123">Request body</span></span>
<span data-ttu-id="accd9-124">要求本文で、[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="accd9-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="accd9-125">次の表に、[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="accd9-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md).</span></span>

|<span data-ttu-id="accd9-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="accd9-126">Property</span></span>|<span data-ttu-id="accd9-127">型</span><span class="sxs-lookup"><span data-stu-id="accd9-127">Type</span></span>|<span data-ttu-id="accd9-128">説明</span><span class="sxs-lookup"><span data-stu-id="accd9-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="accd9-129">ID</span><span class="sxs-lookup"><span data-stu-id="accd9-129">id</span></span>|<span data-ttu-id="accd9-130">文字列</span><span class="sxs-lookup"><span data-stu-id="accd9-130">String</span></span>|<span data-ttu-id="accd9-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="accd9-131">Key of the entity.</span></span>|
|<span data-ttu-id="accd9-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="accd9-132">pendingCount</span></span>|<span data-ttu-id="accd9-133">Int32</span><span class="sxs-lookup"><span data-stu-id="accd9-133">Int32</span></span>|<span data-ttu-id="accd9-134">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="accd9-134">Number of pending devices</span></span>|
|<span data-ttu-id="accd9-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="accd9-135">notApplicableCount</span></span>|<span data-ttu-id="accd9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="accd9-136">Int32</span></span>|<span data-ttu-id="accd9-137">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="accd9-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="accd9-138">successCount</span><span class="sxs-lookup"><span data-stu-id="accd9-138">successCount</span></span>|<span data-ttu-id="accd9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="accd9-139">Int32</span></span>|<span data-ttu-id="accd9-140">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="accd9-140">Number of succeeded devices</span></span>|
|<span data-ttu-id="accd9-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="accd9-141">errorCount</span></span>|<span data-ttu-id="accd9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="accd9-142">Int32</span></span>|<span data-ttu-id="accd9-143">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="accd9-143">Number of error devices</span></span>|
|<span data-ttu-id="accd9-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="accd9-144">failedCount</span></span>|<span data-ttu-id="accd9-145">Int32</span><span class="sxs-lookup"><span data-stu-id="accd9-145">Int32</span></span>|<span data-ttu-id="accd9-146">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="accd9-146">Number of failed devices</span></span>|
|<span data-ttu-id="accd9-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="accd9-147">lastUpdateDateTime</span></span>|<span data-ttu-id="accd9-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="accd9-148">DateTimeOffset</span></span>|<span data-ttu-id="accd9-149">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="accd9-149">Last update time</span></span>|
|<span data-ttu-id="accd9-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="accd9-150">configurationVersion</span></span>|<span data-ttu-id="accd9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="accd9-151">Int32</span></span>|<span data-ttu-id="accd9-152">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="accd9-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="accd9-153">応答</span><span class="sxs-lookup"><span data-stu-id="accd9-153">Response</span></span>
<span data-ttu-id="accd9-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="accd9-154">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="accd9-155">例</span><span class="sxs-lookup"><span data-stu-id="accd9-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="accd9-156">要求</span><span class="sxs-lookup"><span data-stu-id="accd9-156">Request</span></span>
<span data-ttu-id="accd9-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="accd9-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
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

### <a name="response"></a><span data-ttu-id="accd9-158">応答</span><span class="sxs-lookup"><span data-stu-id="accd9-158">Response</span></span>
<span data-ttu-id="accd9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="accd9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```








