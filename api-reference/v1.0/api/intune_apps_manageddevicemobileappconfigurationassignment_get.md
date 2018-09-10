# <a name="get-manageddevicemobileappconfigurationassignment"></a><span data-ttu-id="f0977-101">Get managedDeviceMobileAppConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="f0977-101">Get managedDeviceMobileAppConfigurationAssignment</span></span>

> <span data-ttu-id="f0977-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f0977-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0977-103">[managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f0977-103">Read properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0977-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="f0977-104">Prerequisites</span></span>
<span data-ttu-id="f0977-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f0977-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f0977-107">Permission type</span></span>|<span data-ttu-id="f0977-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f0977-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0977-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f0977-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f0977-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f0977-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f0977-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f0977-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0977-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0977-112">Not supported.</span></span>|
|<span data-ttu-id="f0977-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f0977-113">Application</span></span>|<span data-ttu-id="f0977-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f0977-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0977-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f0977-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0977-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f0977-116">Optional query parameters</span></span>
<span data-ttu-id="f0977-117">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f0977-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f0977-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0977-118">Request headers</span></span>
|<span data-ttu-id="f0977-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f0977-119">Header</span></span>|<span data-ttu-id="f0977-120">値</span><span class="sxs-lookup"><span data-stu-id="f0977-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0977-121">承認</span><span class="sxs-lookup"><span data-stu-id="f0977-121">Authorization</span></span>|<span data-ttu-id="f0977-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f0977-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0977-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f0977-123">Accept</span></span>|<span data-ttu-id="f0977-124">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="f0977-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0977-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f0977-125">Request body</span></span>
<span data-ttu-id="f0977-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f0977-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0977-127">応答</span><span class="sxs-lookup"><span data-stu-id="f0977-127">Response</span></span>
<span data-ttu-id="f0977-128">成功した場合、このメソッドは `200 OK` 応答コードと応答本文で [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f0977-128">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationAssignment](../resources/intune_apps_manageddevicemobileappconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0977-129">例</span><span class="sxs-lookup"><span data-stu-id="f0977-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0977-130">要求</span><span class="sxs-lookup"><span data-stu-id="f0977-130">Request</span></span>
<span data-ttu-id="f0977-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f0977-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments/{managedDeviceMobileAppConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="f0977-132">応答</span><span class="sxs-lookup"><span data-stu-id="f0977-132">Response</span></span>
<span data-ttu-id="f0977-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f0977-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
    "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```








