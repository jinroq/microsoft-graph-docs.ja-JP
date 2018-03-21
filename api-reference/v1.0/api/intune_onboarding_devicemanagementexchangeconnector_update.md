# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="6c451-101">deviceManagementExchangeConnector の更新</span><span class="sxs-lookup"><span data-stu-id="6c451-101">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="6c451-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c451-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c451-103">[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6c451-103">Update the properties of a [calendar](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6c451-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="6c451-104">Prerequisites</span></span>
<span data-ttu-id="6c451-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c451-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6c451-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c451-107">Permission type</span></span>|<span data-ttu-id="6c451-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c451-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c451-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c451-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6c451-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c451-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6c451-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c451-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c451-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c451-112">Not supported.</span></span>|
|<span data-ttu-id="6c451-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c451-113">Application</span></span>|<span data-ttu-id="6c451-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c451-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c451-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c451-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="6c451-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c451-116">Request headers</span></span>
|<span data-ttu-id="6c451-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c451-117">Header</span></span>|<span data-ttu-id="6c451-118">値</span><span class="sxs-lookup"><span data-stu-id="6c451-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c451-119">承認</span><span class="sxs-lookup"><span data-stu-id="6c451-119">Authorization</span></span>|<span data-ttu-id="6c451-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="6c451-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6c451-121">承諾</span><span class="sxs-lookup"><span data-stu-id="6c451-121">Accept</span></span>|<span data-ttu-id="6c451-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6c451-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c451-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c451-123">Request body</span></span>
<span data-ttu-id="6c451-124">要求本文で、[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c451-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="6c451-125">次の表に、[deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6c451-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="6c451-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c451-126">Property</span></span>|<span data-ttu-id="6c451-127">型</span><span class="sxs-lookup"><span data-stu-id="6c451-127">Type</span></span>|<span data-ttu-id="6c451-128">説明</span><span class="sxs-lookup"><span data-stu-id="6c451-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c451-129">id</span><span class="sxs-lookup"><span data-stu-id="6c451-129">id</span></span>|<span data-ttu-id="6c451-130">String</span><span class="sxs-lookup"><span data-stu-id="6c451-130">String</span></span>|<span data-ttu-id="6c451-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6c451-131">Not yet documented</span></span>|
|<span data-ttu-id="6c451-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6c451-132">lastSyncDateTime</span></span>|<span data-ttu-id="6c451-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c451-133">DateTimeOffset</span></span>|<span data-ttu-id="6c451-134">Exchange Connector の最終同期日時</span><span class="sxs-lookup"><span data-stu-id="6c451-134">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="6c451-135">status</span><span class="sxs-lookup"><span data-stu-id="6c451-135">status</span></span>|<span data-ttu-id="6c451-136">String</span><span class="sxs-lookup"><span data-stu-id="6c451-136">String</span></span>|<span data-ttu-id="6c451-137">Exchange Connector の状態。可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。</span><span class="sxs-lookup"><span data-stu-id="6c451-137">Exchange Connector Status Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="6c451-138">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="6c451-138">primarySmtpAddress</span></span>|<span data-ttu-id="6c451-139">String</span><span class="sxs-lookup"><span data-stu-id="6c451-139">String</span></span>|<span data-ttu-id="6c451-140">サービス間の Exchange Connector を構成するときに使用するメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="6c451-140">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="6c451-141">serverName</span><span class="sxs-lookup"><span data-stu-id="6c451-141">ServerName</span></span>|<span data-ttu-id="6c451-142">String</span><span class="sxs-lookup"><span data-stu-id="6c451-142">String</span></span>|<span data-ttu-id="6c451-143">Exchange Connector をホストするサーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="6c451-143">The name of the server hosting the launcher component.</span></span>|
|<span data-ttu-id="6c451-144">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="6c451-144">exchangeConnectorType</span></span>|<span data-ttu-id="6c451-145">String</span><span class="sxs-lookup"><span data-stu-id="6c451-145">String</span></span>|<span data-ttu-id="6c451-146">構成されている Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="6c451-146">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="6c451-147">可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。</span><span class="sxs-lookup"><span data-stu-id="6c451-147">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="6c451-148">version</span><span class="sxs-lookup"><span data-stu-id="6c451-148">version</span></span>|<span data-ttu-id="6c451-149">String</span><span class="sxs-lookup"><span data-stu-id="6c451-149">String</span></span>|<span data-ttu-id="6c451-150">ExchangeConnectorAgent のバージョン</span><span class="sxs-lookup"><span data-stu-id="6c451-150">The version of the document.</span></span>|
|<span data-ttu-id="6c451-151">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="6c451-151">exchangeAlias</span></span>|<span data-ttu-id="6c451-152">String</span><span class="sxs-lookup"><span data-stu-id="6c451-152">String</span></span>|<span data-ttu-id="6c451-153">Exchange Server に割り当てられているエイリアス。</span><span class="sxs-lookup"><span data-stu-id="6c451-153">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="6c451-154">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="6c451-154">exchangeOrganization</span></span>|<span data-ttu-id="6c451-155">String</span><span class="sxs-lookup"><span data-stu-id="6c451-155">String</span></span>|<span data-ttu-id="6c451-156">Exchange Server に対する Exchange 組織</span><span class="sxs-lookup"><span data-stu-id="6c451-156">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="6c451-157">応答</span><span class="sxs-lookup"><span data-stu-id="6c451-157">Response</span></span>
<span data-ttu-id="6c451-158">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceManagementExchangeConnector](../resources/intune_onboarding_devicemanagementexchangeconnector.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="6c451-158">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c451-159">例</span><span class="sxs-lookup"><span data-stu-id="6c451-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="6c451-160">要求</span><span class="sxs-lookup"><span data-stu-id="6c451-160">Request</span></span>
<span data-ttu-id="6c451-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c451-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
Content-type: application/json
Content-length: 361

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="6c451-162">応答</span><span class="sxs-lookup"><span data-stu-id="6c451-162">Response</span></span>
<span data-ttu-id="6c451-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6c451-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 482

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



