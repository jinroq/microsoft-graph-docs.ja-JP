# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="ca621-101">deviceManagementExchangeConnector の作成</span><span class="sxs-lookup"><span data-stu-id="ca621-101">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="ca621-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca621-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca621-103">新しい [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ca621-103">Create a new [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca621-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ca621-104">Prerequisites</span></span>
<span data-ttu-id="ca621-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca621-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ca621-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca621-107">Permission type</span></span>|<span data-ttu-id="ca621-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca621-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca621-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca621-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ca621-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca621-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ca621-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca621-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca621-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca621-112">Not supported.</span></span>|
|<span data-ttu-id="ca621-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca621-113">Application</span></span>|<span data-ttu-id="ca621-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca621-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca621-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca621-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="ca621-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca621-116">Request headers</span></span>
|<span data-ttu-id="ca621-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca621-117">Header</span></span>|<span data-ttu-id="ca621-118">値</span><span class="sxs-lookup"><span data-stu-id="ca621-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca621-119">承認</span><span class="sxs-lookup"><span data-stu-id="ca621-119">Authorization</span></span>|<span data-ttu-id="ca621-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="ca621-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca621-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ca621-121">Accept</span></span>|<span data-ttu-id="ca621-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ca621-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca621-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca621-123">Request body</span></span>
<span data-ttu-id="ca621-124">要求本文で、deviceManagementExchangeConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca621-124">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="ca621-125">次の表に、deviceManagementExchangeConnector の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ca621-125">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="ca621-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca621-126">Property</span></span>|<span data-ttu-id="ca621-127">型</span><span class="sxs-lookup"><span data-stu-id="ca621-127">Type</span></span>|<span data-ttu-id="ca621-128">説明</span><span class="sxs-lookup"><span data-stu-id="ca621-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca621-129">id</span><span class="sxs-lookup"><span data-stu-id="ca621-129">id</span></span>|<span data-ttu-id="ca621-130">String</span><span class="sxs-lookup"><span data-stu-id="ca621-130">String</span></span>|<span data-ttu-id="ca621-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ca621-131">Not yet documented</span></span>|
|<span data-ttu-id="ca621-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ca621-132">lastSyncDateTime</span></span>|<span data-ttu-id="ca621-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca621-133">DateTimeOffset</span></span>|<span data-ttu-id="ca621-134">Exchange Connector の最終同期日時</span><span class="sxs-lookup"><span data-stu-id="ca621-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="ca621-135">status</span><span class="sxs-lookup"><span data-stu-id="ca621-135">status</span></span>|[<span data-ttu-id="ca621-136">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="ca621-136">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="ca621-137">Exchange コネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="ca621-137">Exchange Connector Status.</span></span> <span data-ttu-id="ca621-138">可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。</span><span class="sxs-lookup"><span data-stu-id="ca621-138">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="ca621-139">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="ca621-139">primarySmtpAddress</span></span>|<span data-ttu-id="ca621-140">String</span><span class="sxs-lookup"><span data-stu-id="ca621-140">String</span></span>|<span data-ttu-id="ca621-141">サービス間の Exchange Connector を構成するときに使用するメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="ca621-141">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="ca621-142">serverName</span><span class="sxs-lookup"><span data-stu-id="ca621-142">serverName</span></span>|<span data-ttu-id="ca621-143">String</span><span class="sxs-lookup"><span data-stu-id="ca621-143">String</span></span>|<span data-ttu-id="ca621-144">Exchange サーバーの名前です。</span><span class="sxs-lookup"><span data-stu-id="ca621-144">The name of the Exchange server.</span></span>|
|<span data-ttu-id="ca621-145">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="ca621-145">connectorServerName</span></span>|<span data-ttu-id="ca621-146">String</span><span class="sxs-lookup"><span data-stu-id="ca621-146">String</span></span>|<span data-ttu-id="ca621-147">Exchange Connector をホストするサーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="ca621-147">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="ca621-148">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="ca621-148">exchangeConnectorType</span></span>|[<span data-ttu-id="ca621-149">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="ca621-149">deviceManagementExchangeConnectorType</span></span>](../resources/intune_onboarding_devicemanagementexchangeconnectortype.md)|<span data-ttu-id="ca621-150">構成されている Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="ca621-150">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="ca621-151">可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。</span><span class="sxs-lookup"><span data-stu-id="ca621-151">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="ca621-152">version</span><span class="sxs-lookup"><span data-stu-id="ca621-152">version</span></span>|<span data-ttu-id="ca621-153">String</span><span class="sxs-lookup"><span data-stu-id="ca621-153">String</span></span>|<span data-ttu-id="ca621-154">ExchangeConnectorAgent のバージョン</span><span class="sxs-lookup"><span data-stu-id="ca621-154">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="ca621-155">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="ca621-155">exchangeAlias</span></span>|<span data-ttu-id="ca621-156">String</span><span class="sxs-lookup"><span data-stu-id="ca621-156">String</span></span>|<span data-ttu-id="ca621-157">Exchange Server に割り当てられているエイリアス。</span><span class="sxs-lookup"><span data-stu-id="ca621-157">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="ca621-158">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="ca621-158">exchangeOrganization</span></span>|<span data-ttu-id="ca621-159">String</span><span class="sxs-lookup"><span data-stu-id="ca621-159">String</span></span>|<span data-ttu-id="ca621-160">Exchange Server に対する Exchange 組織</span><span class="sxs-lookup"><span data-stu-id="ca621-160">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="ca621-161">応答</span><span class="sxs-lookup"><span data-stu-id="ca621-161">Response</span></span>
<span data-ttu-id="ca621-162">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ca621-162">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca621-163">例</span><span class="sxs-lookup"><span data-stu-id="ca621-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca621-164">要求</span><span class="sxs-lookup"><span data-stu-id="ca621-164">Request</span></span>
<span data-ttu-id="ca621-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca621-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="ca621-166">応答</span><span class="sxs-lookup"><span data-stu-id="ca621-166">Response</span></span>
<span data-ttu-id="ca621-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca621-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



