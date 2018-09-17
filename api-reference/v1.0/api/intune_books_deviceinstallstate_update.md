# <a name="update-deviceinstallstate"></a><span data-ttu-id="781a5-101">deviceInstallState の更新</span><span class="sxs-lookup"><span data-stu-id="781a5-101">Update deviceInstallState</span></span>

> <span data-ttu-id="781a5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="781a5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="781a5-103">[deviceInstallState](../resources/intune_books_deviceinstallstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="781a5-103">Update the properties of a [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="781a5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="781a5-104">Prerequisites</span></span>
<span data-ttu-id="781a5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="781a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="781a5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="781a5-107">Permission type</span></span>|<span data-ttu-id="781a5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="781a5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="781a5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="781a5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="781a5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="781a5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="781a5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="781a5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="781a5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="781a5-112">Not supported.</span></span>|
|<span data-ttu-id="781a5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="781a5-113">Application</span></span>|<span data-ttu-id="781a5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="781a5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="781a5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="781a5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates/{deviceInstallStateId}
```

## <a name="request-headers"></a><span data-ttu-id="781a5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="781a5-116">Request headers</span></span>
|<span data-ttu-id="781a5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="781a5-117">Header</span></span>|<span data-ttu-id="781a5-118">値</span><span class="sxs-lookup"><span data-stu-id="781a5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="781a5-119">承認</span><span class="sxs-lookup"><span data-stu-id="781a5-119">Authorization</span></span>|<span data-ttu-id="781a5-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="781a5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="781a5-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="781a5-121">Accept</span></span>|<span data-ttu-id="781a5-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="781a5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="781a5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="781a5-123">Request body</span></span>
<span data-ttu-id="781a5-124">要求本文で、[deviceInstallState](../resources/intune_books_deviceinstallstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="781a5-124">In the request body, supply a JSON representation for the [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object.</span></span>

<span data-ttu-id="781a5-125">次の表に、[deviceInstallState](../resources/intune_books_deviceinstallstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="781a5-125">The following table shows the properties that are required when you create the [deviceInstallState](../resources/intune_books_deviceinstallstate.md).</span></span>

|<span data-ttu-id="781a5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="781a5-126">Property</span></span>|<span data-ttu-id="781a5-127">型</span><span class="sxs-lookup"><span data-stu-id="781a5-127">Type</span></span>|<span data-ttu-id="781a5-128">説明</span><span class="sxs-lookup"><span data-stu-id="781a5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="781a5-129">ID</span><span class="sxs-lookup"><span data-stu-id="781a5-129">id</span></span>|<span data-ttu-id="781a5-130">文字列</span><span class="sxs-lookup"><span data-stu-id="781a5-130">String</span></span>|<span data-ttu-id="781a5-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="781a5-131">Key of the entity.</span></span>|
|<span data-ttu-id="781a5-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="781a5-132">deviceName</span></span>|<span data-ttu-id="781a5-133">文字列</span><span class="sxs-lookup"><span data-stu-id="781a5-133">String</span></span>|<span data-ttu-id="781a5-134">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="781a5-134">Device name.</span></span>|
|<span data-ttu-id="781a5-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="781a5-135">deviceId</span></span>|<span data-ttu-id="781a5-136">文字列</span><span class="sxs-lookup"><span data-stu-id="781a5-136">String</span></span>|<span data-ttu-id="781a5-137">デバイス ID。</span><span class="sxs-lookup"><span data-stu-id="781a5-137">Device Id.</span></span>|
|<span data-ttu-id="781a5-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="781a5-138">lastSyncDateTime</span></span>|<span data-ttu-id="781a5-139">DateTimeOffset
</span><span class="sxs-lookup"><span data-stu-id="781a5-139">DateTimeOffset</span></span>|<span data-ttu-id="781a5-140">最後の同期日時。</span><span class="sxs-lookup"><span data-stu-id="781a5-140">Last sync date and time.</span></span>|
|<span data-ttu-id="781a5-141">installState</span><span class="sxs-lookup"><span data-stu-id="781a5-141">installState</span></span>|[<span data-ttu-id="781a5-142">installState</span><span class="sxs-lookup"><span data-stu-id="781a5-142">installState</span></span>](../resources/intune_books_installstate.md)|<span data-ttu-id="781a5-143">電子ブックのインストールの状態です。</span><span class="sxs-lookup"><span data-stu-id="781a5-143">The install state of the eBook.</span></span> <span data-ttu-id="781a5-144">可能な値は、`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="781a5-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="781a5-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="781a5-145">errorCode</span></span>|<span data-ttu-id="781a5-146">文字列</span><span class="sxs-lookup"><span data-stu-id="781a5-146">String</span></span>|<span data-ttu-id="781a5-147">インストール失敗のエラー コード。</span><span class="sxs-lookup"><span data-stu-id="781a5-147">The error code for install failures.</span></span>|
|<span data-ttu-id="781a5-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="781a5-148">osVersion</span></span>|<span data-ttu-id="781a5-149">文字列</span><span class="sxs-lookup"><span data-stu-id="781a5-149">String</span></span>|<span data-ttu-id="781a5-150">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="781a5-150">OS Version.</span></span>|
|<span data-ttu-id="781a5-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="781a5-151">osDescription</span></span>|<span data-ttu-id="781a5-152">文字列</span><span class="sxs-lookup"><span data-stu-id="781a5-152">String</span></span>|<span data-ttu-id="781a5-153">OS の説明。</span><span class="sxs-lookup"><span data-stu-id="781a5-153">OS Description.</span></span>|
|<span data-ttu-id="781a5-154">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="781a5-154">userName</span></span>|<span data-ttu-id="781a5-155">文字列</span><span class="sxs-lookup"><span data-stu-id="781a5-155">String</span></span>|<span data-ttu-id="781a5-156">デバイスのユーザー名。</span><span class="sxs-lookup"><span data-stu-id="781a5-156">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="781a5-157">応答</span><span class="sxs-lookup"><span data-stu-id="781a5-157">Response</span></span>
<span data-ttu-id="781a5-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceInstallState](../resources/intune_books_deviceinstallstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="781a5-158">If successful, this method returns a `200 OK` response code and an updated [deviceInstallState](../resources/intune_books_deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="781a5-159">例</span><span class="sxs-lookup"><span data-stu-id="781a5-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="781a5-160">要求</span><span class="sxs-lookup"><span data-stu-id="781a5-160">Request</span></span>
<span data-ttu-id="781a5-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="781a5-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates/{deviceInstallStateId}
Content-type: application/json
Content-length: 317

{
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="781a5-162">応答</span><span class="sxs-lookup"><span data-stu-id="781a5-162">Response</span></span>
<span data-ttu-id="781a5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="781a5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```








