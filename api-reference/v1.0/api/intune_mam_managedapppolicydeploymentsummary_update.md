# <a name="update-managedapppolicydeploymentsummary"></a><span data-ttu-id="44fe7-101">managedAppPolicyDeploymentSummary の更新</span><span class="sxs-lookup"><span data-stu-id="44fe7-101">Update managedAppPolicyDeploymentSummary</span></span>

> <span data-ttu-id="44fe7-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="44fe7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44fe7-103">[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="44fe7-103">Update the properties of a [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="44fe7-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="44fe7-104">Prerequisites</span></span>
<span data-ttu-id="44fe7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44fe7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44fe7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44fe7-107">Permission type</span></span>|<span data-ttu-id="44fe7-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="44fe7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44fe7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44fe7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="44fe7-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44fe7-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="44fe7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44fe7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44fe7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44fe7-112">Not supported.</span></span>|
|<span data-ttu-id="44fe7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44fe7-113">Application</span></span>|<span data-ttu-id="44fe7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44fe7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44fe7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44fe7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/deploymentSummary
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/deploymentSummary
```

## <a name="request-headers"></a><span data-ttu-id="44fe7-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44fe7-116">Request headers</span></span>
|<span data-ttu-id="44fe7-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44fe7-117">Header</span></span>|<span data-ttu-id="44fe7-118">値</span><span class="sxs-lookup"><span data-stu-id="44fe7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44fe7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="44fe7-119">Authorization</span></span>|<span data-ttu-id="44fe7-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="44fe7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44fe7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="44fe7-121">Accept</span></span>|<span data-ttu-id="44fe7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="44fe7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44fe7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="44fe7-123">Request body</span></span>
<span data-ttu-id="44fe7-124">要求本文で、[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="44fe7-124">In the request body, supply a JSON representation for the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object.</span></span>

<span data-ttu-id="44fe7-125">次の表に、[managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="44fe7-125">The following table shows the properties that are required when you create the [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md).</span></span>

|<span data-ttu-id="44fe7-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44fe7-126">Property</span></span>|<span data-ttu-id="44fe7-127">型</span><span class="sxs-lookup"><span data-stu-id="44fe7-127">Type</span></span>|<span data-ttu-id="44fe7-128">説明</span><span class="sxs-lookup"><span data-stu-id="44fe7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44fe7-129">displayName</span><span class="sxs-lookup"><span data-stu-id="44fe7-129">displayName</span></span>|<span data-ttu-id="44fe7-130">String</span><span class="sxs-lookup"><span data-stu-id="44fe7-130">String</span></span>|<span data-ttu-id="44fe7-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="44fe7-131">Not yet documented</span></span>|
|<span data-ttu-id="44fe7-132">configurationDeployedUserCount</span><span class="sxs-lookup"><span data-stu-id="44fe7-132">configurationDeployedUserCount</span></span>|<span data-ttu-id="44fe7-133">Int32</span><span class="sxs-lookup"><span data-stu-id="44fe7-133">Int32</span></span>|<span data-ttu-id="44fe7-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="44fe7-134">Not yet documented</span></span>|
|<span data-ttu-id="44fe7-135">lastRefreshTime</span><span class="sxs-lookup"><span data-stu-id="44fe7-135">lastRefreshTime</span></span>|<span data-ttu-id="44fe7-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="44fe7-136">DateTimeOffset</span></span>|<span data-ttu-id="44fe7-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="44fe7-137">Not yet documented</span></span>|
|<span data-ttu-id="44fe7-138">configurationDeploymentSummaryPerApp</span><span class="sxs-lookup"><span data-stu-id="44fe7-138">configurationDeploymentSummaryPerApp</span></span>|<span data-ttu-id="44fe7-139">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="44fe7-139">[managedAppPolicyDeploymentSummaryPerApp](../resources/intune_mam_managedapppolicydeploymentsummaryperapp.md) collection</span></span>|<span data-ttu-id="44fe7-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="44fe7-140">Not yet documented</span></span>|
|<span data-ttu-id="44fe7-141">id</span><span class="sxs-lookup"><span data-stu-id="44fe7-141">id</span></span>|<span data-ttu-id="44fe7-142">String</span><span class="sxs-lookup"><span data-stu-id="44fe7-142">String</span></span>|<span data-ttu-id="44fe7-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="44fe7-143">Key of the entity.</span></span>|
|<span data-ttu-id="44fe7-144">version</span><span class="sxs-lookup"><span data-stu-id="44fe7-144">version</span></span>|<span data-ttu-id="44fe7-145">String</span><span class="sxs-lookup"><span data-stu-id="44fe7-145">String</span></span>|<span data-ttu-id="44fe7-146">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="44fe7-146">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="44fe7-147">応答</span><span class="sxs-lookup"><span data-stu-id="44fe7-147">Response</span></span>
<span data-ttu-id="44fe7-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="44fe7-148">If successful, this method returns a `200 OK` response code and an updated [managedAppPolicyDeploymentSummary](../resources/intune_mam_managedapppolicydeploymentsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44fe7-149">例</span><span class="sxs-lookup"><span data-stu-id="44fe7-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="44fe7-150">要求</span><span class="sxs-lookup"><span data-stu-id="44fe7-150">Request</span></span>
<span data-ttu-id="44fe7-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44fe7-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/deploymentSummary
Content-type: application/json
Content-length: 588

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="44fe7-152">応答</span><span class="sxs-lookup"><span data-stu-id="44fe7-152">Response</span></span>
<span data-ttu-id="44fe7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44fe7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 637

{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummary",
  "displayName": "Display Name value",
  "configurationDeployedUserCount": 14,
  "lastRefreshTime": "2017-01-01T00:01:30.1240368-08:00",
  "configurationDeploymentSummaryPerApp": [
    {
      "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
        "packageId": "Package Id value"
      },
      "configurationAppliedUserCount": 13
    }
  ],
  "id": "61f2f688-f688-61f2-88f6-f26188f6f261",
  "version": "Version value"
}
```



