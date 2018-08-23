# <a name="update-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="823d8-101">managedDeviceMobileAppConfigurationUserSummary の更新</span><span class="sxs-lookup"><span data-stu-id="823d8-101">Update managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="823d8-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="823d8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="823d8-103">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="823d8-103">Update the properties of a [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="823d8-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="823d8-104">Prerequisites</span></span>
<span data-ttu-id="823d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="823d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="823d8-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="823d8-107">Permission type</span></span>|<span data-ttu-id="823d8-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="823d8-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="823d8-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="823d8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="823d8-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="823d8-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="823d8-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="823d8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="823d8-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="823d8-112">Not supported.</span></span>|
|<span data-ttu-id="823d8-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="823d8-113">Application</span></span>|<span data-ttu-id="823d8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="823d8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="823d8-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="823d8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="823d8-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="823d8-116">Request headers</span></span>
|<span data-ttu-id="823d8-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="823d8-117">Header</span></span>|<span data-ttu-id="823d8-118">値</span><span class="sxs-lookup"><span data-stu-id="823d8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="823d8-119">承認</span><span class="sxs-lookup"><span data-stu-id="823d8-119">Authorization</span></span>|<span data-ttu-id="823d8-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="823d8-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="823d8-121">受け入れ</span><span class="sxs-lookup"><span data-stu-id="823d8-121">Accept</span></span>|<span data-ttu-id="823d8-122">アプリケーション/json</span><span class="sxs-lookup"><span data-stu-id="823d8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="823d8-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="823d8-123">Request body</span></span>
<span data-ttu-id="823d8-124">要求本文で、[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="823d8-124">In the request body, supply a JSON representation for the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object.</span></span>

<span data-ttu-id="823d8-125">次の表に、[managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="823d8-125">The following table shows the properties that are required when you create the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md).</span></span>

|<span data-ttu-id="823d8-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="823d8-126">Property</span></span>|<span data-ttu-id="823d8-127">型</span><span class="sxs-lookup"><span data-stu-id="823d8-127">Type</span></span>|<span data-ttu-id="823d8-128">説明</span><span class="sxs-lookup"><span data-stu-id="823d8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="823d8-129">id</span><span class="sxs-lookup"><span data-stu-id="823d8-129">id</span></span>|<span data-ttu-id="823d8-130">文字列</span><span class="sxs-lookup"><span data-stu-id="823d8-130">String</span></span>|<span data-ttu-id="823d8-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="823d8-131">Key of the entity.</span></span>|
|<span data-ttu-id="823d8-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="823d8-132">pendingCount</span></span>|<span data-ttu-id="823d8-133">Int32</span><span class="sxs-lookup"><span data-stu-id="823d8-133">Int32</span></span>|<span data-ttu-id="823d8-134">保留中のユーザーの数</span><span class="sxs-lookup"><span data-stu-id="823d8-134">Number of pending Users</span></span>|
|<span data-ttu-id="823d8-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="823d8-135">notApplicableCount</span></span>|<span data-ttu-id="823d8-136">Int32</span><span class="sxs-lookup"><span data-stu-id="823d8-136">Int32</span></span>|<span data-ttu-id="823d8-137">該当しないユーザーの数</span><span class="sxs-lookup"><span data-stu-id="823d8-137">Number of not applicable users.</span></span>|
|<span data-ttu-id="823d8-138">successCount</span><span class="sxs-lookup"><span data-stu-id="823d8-138">successCount</span></span>|<span data-ttu-id="823d8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="823d8-139">Int32</span></span>|<span data-ttu-id="823d8-140">成功したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="823d8-140">Number of succeeded Users</span></span>|
|<span data-ttu-id="823d8-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="823d8-141">errorCount</span></span>|<span data-ttu-id="823d8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="823d8-142">Int32</span></span>|<span data-ttu-id="823d8-143">エラー ユーザーの数</span><span class="sxs-lookup"><span data-stu-id="823d8-143">Number of error Users</span></span>|
|<span data-ttu-id="823d8-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="823d8-144">failedCount</span></span>|<span data-ttu-id="823d8-145">Int32</span><span class="sxs-lookup"><span data-stu-id="823d8-145">Int32</span></span>|<span data-ttu-id="823d8-146">失敗したユーザーの数</span><span class="sxs-lookup"><span data-stu-id="823d8-146">Number of failed Users</span></span>|
|<span data-ttu-id="823d8-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="823d8-147">lastUpdateDateTime</span></span>|<span data-ttu-id="823d8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="823d8-148">DateTimeOffset</span></span>|<span data-ttu-id="823d8-149">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="823d8-149">Last update time</span></span>|
|<span data-ttu-id="823d8-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="823d8-150">configurationVersion</span></span>|<span data-ttu-id="823d8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="823d8-151">Int32</span></span>|<span data-ttu-id="823d8-152">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="823d8-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="823d8-153">応答</span><span class="sxs-lookup"><span data-stu-id="823d8-153">Response</span></span>
<span data-ttu-id="823d8-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="823d8-154">If successful, this method returns a `200 OK` response code and an updated [managedDeviceMobileAppConfigurationUserSummary](../resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="823d8-155">例</span><span class="sxs-lookup"><span data-stu-id="823d8-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="823d8-156">要求</span><span class="sxs-lookup"><span data-stu-id="823d8-156">Request</span></span>
<span data-ttu-id="823d8-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="823d8-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
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

### <a name="response"></a><span data-ttu-id="823d8-158">応答</span><span class="sxs-lookup"><span data-stu-id="823d8-158">Response</span></span>
<span data-ttu-id="823d8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="823d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
  "id": "7b953742-3742-7b95-4237-957b4237957b",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



