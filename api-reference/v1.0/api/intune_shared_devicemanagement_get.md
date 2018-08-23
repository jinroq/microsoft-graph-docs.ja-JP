# <a name="get-devicemanagement"></a><span data-ttu-id="faabd-101">deviceManagement の取得</span><span class="sxs-lookup"><span data-stu-id="faabd-101">Get deviceManagement</span></span>

> <span data-ttu-id="faabd-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="faabd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="faabd-103">[deviceManagement](../resources/intune_shared_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="faabd-103">Read properties and relationships of the [deviceManagement](../resources/intune_shared_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="faabd-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="faabd-104">Prerequisites</span></span>
<span data-ttu-id="faabd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="faabd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="faabd-107">アクセス権&nbsp;型&nbsp;(によって&nbsp;ワークフロー)</span><span class="sxs-lookup"><span data-stu-id="faabd-107">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="faabd-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="faabd-108">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="faabd-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="faabd-109">Delegated (work or school account)</span></span> | |
| <span data-ttu-id="faabd-110">&nbsp; &nbsp; 監査</span><span class="sxs-lookup"><span data-stu-id="faabd-110">&nbsp; &nbsp;Auditing</span></span> | <span data-ttu-id="faabd-111">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-111">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
| <span data-ttu-id="faabd-112">&nbsp; &nbsp; 会社の用語</span><span class="sxs-lookup"><span data-stu-id="faabd-112">&nbsp; &nbsp; Company terms</span></span> | <span data-ttu-id="faabd-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="faabd-114">&nbsp; &nbsp; 企業登録</span><span class="sxs-lookup"><span data-stu-id="faabd-114">&nbsp; &nbsp; Corporate enrollment</span></span> | <span data-ttu-id="faabd-115">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="faabd-116">&nbsp; &nbsp; デバイス構成</span><span class="sxs-lookup"><span data-stu-id="faabd-116">&nbsp; &nbsp;Device configuration</span></span> | <span data-ttu-id="faabd-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="faabd-118">&nbsp; &nbsp; デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="faabd-118">&nbsp; &nbsp;Device management</span></span> | <span data-ttu-id="faabd-119">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-119">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="faabd-120">&nbsp; &nbsp; エンドポイント保護</span><span class="sxs-lookup"><span data-stu-id="faabd-120">&nbsp; &nbsp;Endpoint Protection</span></span> | <span data-ttu-id="faabd-121">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span> |
| <span data-ttu-id="faabd-122">&nbsp; &nbsp; 登録</span><span class="sxs-lookup"><span data-stu-id="faabd-122">&nbsp; &nbsp;Enrollment</span></span> | <span data-ttu-id="faabd-123">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-123">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="faabd-124">&nbsp; &nbsp; 通知</span><span class="sxs-lookup"><span data-stu-id="faabd-124">&nbsp; &nbsp;Notification</span></span> | <span data-ttu-id="faabd-125">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-125">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="faabd-126">&nbsp; &nbsp; 採用</span><span class="sxs-lookup"><span data-stu-id="faabd-126">&nbsp; &nbsp; On-boarding</span></span> | <span data-ttu-id="faabd-127">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-127">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="faabd-128">&nbsp; &nbsp; RBAC</span><span class="sxs-lookup"><span data-stu-id="faabd-128">&nbsp; &nbsp;RBAC</span></span> | <span data-ttu-id="faabd-129">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-129">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span> |
| <span data-ttu-id="faabd-130">&nbsp; &nbsp; リモート アシスタンス</span><span class="sxs-lookup"><span data-stu-id="faabd-130">remote assistance,</span></span> | <span data-ttu-id="faabd-131">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-131">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="faabd-132">&nbsp; &nbsp; 通信経費の管理パートナー</span><span class="sxs-lookup"><span data-stu-id="faabd-132">&nbsp; &nbsp;Telecom expense management partner</span></span> | <span data-ttu-id="faabd-133">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-133">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
| <span data-ttu-id="faabd-134">&nbsp; &nbsp; トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="faabd-134">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="faabd-135">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-135">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="faabd-136">&nbsp; &nbsp; Windows 情報保護</span><span class="sxs-lookup"><span data-stu-id="faabd-136">Windows information protection</span></span> | <span data-ttu-id="faabd-137">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="faabd-137">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
| <span data-ttu-id="faabd-138">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="faabd-138">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="faabd-139">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faabd-139">Not supported.</span></span>|
| <span data-ttu-id="faabd-140">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="faabd-140">Application</span></span> | <span data-ttu-id="faabd-141">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="faabd-141">Not supported.</span></span> |



## <a name="http-request"></a><span data-ttu-id="faabd-142">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="faabd-142">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement
```

## <a name="optional-query-parameters"></a><span data-ttu-id="faabd-143">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="faabd-143">Optional query parameters</span></span>
<span data-ttu-id="faabd-144">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="faabd-144">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="faabd-145">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="faabd-145">Request headers</span></span>
|<span data-ttu-id="faabd-146">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="faabd-146">Header</span></span>|<span data-ttu-id="faabd-147">値</span><span class="sxs-lookup"><span data-stu-id="faabd-147">Value</span></span>|
|:---|:---|
|<span data-ttu-id="faabd-148">承認</span><span class="sxs-lookup"><span data-stu-id="faabd-148">Authorization</span></span>|<span data-ttu-id="faabd-149">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="faabd-149">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="faabd-150">受諾</span><span class="sxs-lookup"><span data-stu-id="faabd-150">Accept</span></span>|<span data-ttu-id="faabd-151">application/json</span><span class="sxs-lookup"><span data-stu-id="faabd-151">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="faabd-152">要求本文</span><span class="sxs-lookup"><span data-stu-id="faabd-152">Request body</span></span>
<span data-ttu-id="faabd-153">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="faabd-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="faabd-154">応答</span><span class="sxs-lookup"><span data-stu-id="faabd-154">Response</span></span>
<span data-ttu-id="faabd-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagement](../resources/intune_shared_devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="faabd-155">If successful, this method returns a `200 OK` response code and [deviceManagement](../resources/intune_shared_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="faabd-156">例</span><span class="sxs-lookup"><span data-stu-id="faabd-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="faabd-157">要求</span><span class="sxs-lookup"><span data-stu-id="faabd-157">Request</span></span>
<span data-ttu-id="faabd-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="faabd-158">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement
```

### <a name="response"></a><span data-ttu-id="faabd-159">応答</span><span class="sxs-lookup"><span data-stu-id="faabd-159">Response</span></span>
<span data-ttu-id="faabd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="faabd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 918

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "0b283420-3420-0b28-2034-280b2034280b",
    "subscriptionState": "active",
    "subscriptions": "intune",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent",
      "shareAPNSData": "granted"
    },
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview",
      "totalReportedDeviceCount": 8,
      "inactiveThreatAgentDeviceCount": 14,
      "unknownStateThreatAgentDeviceCount": 2,
      "pendingSignatureUpdateDeviceCount": 1,
      "cleanDeviceCount": 0,
      "pendingFullScanDeviceCount": 10,
      "pendingRestartDeviceCount": 9,
      "pendingManualStepsDeviceCount": 13,
      "pendingOfflineScanDeviceCount": 13,
      "criticalFailuresDeviceCount": 11
    },
    "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
  }
}
```



