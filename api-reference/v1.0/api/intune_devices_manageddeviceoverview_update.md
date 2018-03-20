# <a name="update-manageddeviceoverview"></a><span data-ttu-id="dfb95-101">managedDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="dfb95-101">Update managedDeviceOverview</span></span>

> <span data-ttu-id="dfb95-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dfb95-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfb95-103">[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dfb95-103">Update the properties of a [calendar](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dfb95-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="dfb95-104">Prerequisites</span></span>
<span data-ttu-id="dfb95-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfb95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dfb95-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dfb95-107">Permission type</span></span>|<span data-ttu-id="dfb95-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dfb95-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfb95-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dfb95-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dfb95-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfb95-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="dfb95-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dfb95-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfb95-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfb95-112">Not supported.</span></span>|
|<span data-ttu-id="dfb95-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dfb95-113">Application</span></span>|<span data-ttu-id="dfb95-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfb95-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfb95-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dfb95-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDeviceOverview
```

## <a name="request-headers"></a><span data-ttu-id="dfb95-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfb95-116">Request headers</span></span>
|<span data-ttu-id="dfb95-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dfb95-117">Header</span></span>|<span data-ttu-id="dfb95-118">値</span><span class="sxs-lookup"><span data-stu-id="dfb95-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfb95-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfb95-119">Authorization</span></span>|<span data-ttu-id="dfb95-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dfb95-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="dfb95-121">Accept</span><span class="sxs-lookup"><span data-stu-id="dfb95-121">Accept</span></span>|<span data-ttu-id="dfb95-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dfb95-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfb95-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="dfb95-123">Request body</span></span>
<span data-ttu-id="dfb95-124">要求本文で、[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dfb95-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_devices_manageddeviceoverview.md) object.</span></span>

<span data-ttu-id="dfb95-125">次の表に、[managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dfb95-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="dfb95-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfb95-126">Property</span></span>|<span data-ttu-id="dfb95-127">型</span><span class="sxs-lookup"><span data-stu-id="dfb95-127">Type</span></span>|<span data-ttu-id="dfb95-128">説明</span><span class="sxs-lookup"><span data-stu-id="dfb95-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfb95-129">id</span><span class="sxs-lookup"><span data-stu-id="dfb95-129">id</span></span>|<span data-ttu-id="dfb95-130">String</span><span class="sxs-lookup"><span data-stu-id="dfb95-130">String</span></span>|<span data-ttu-id="dfb95-131">概要の一意識別子</span><span class="sxs-lookup"><span data-stu-id="dfb95-131">Unique Identifier for the summary</span></span>|
|<span data-ttu-id="dfb95-132">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dfb95-132">enrolledDeviceCount</span></span>|<span data-ttu-id="dfb95-133">Int32</span><span class="sxs-lookup"><span data-stu-id="dfb95-133">Int32</span></span>|<span data-ttu-id="dfb95-134">登録済みデバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="dfb95-134">Total enrolled device count.</span></span> <span data-ttu-id="dfb95-135">Intune PC エージェントで管理されている PC デバイスは含まれません</span><span class="sxs-lookup"><span data-stu-id="dfb95-135">Does not include PC devices managed via Intune PC Agent</span></span>|
|<span data-ttu-id="dfb95-136">mdmEnrolledCount</span><span class="sxs-lookup"><span data-stu-id="dfb95-136">mdmEnrolledCount</span></span>|<span data-ttu-id="dfb95-137">Int32</span><span class="sxs-lookup"><span data-stu-id="dfb95-137">Int32</span></span>|<span data-ttu-id="dfb95-138">MDM に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="dfb95-138">The number of devices enrolled in MDM</span></span>|
|<span data-ttu-id="dfb95-139">dualEnrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="dfb95-139">dualEnrolledDeviceCount</span></span>|<span data-ttu-id="dfb95-140">Int32</span><span class="sxs-lookup"><span data-stu-id="dfb95-140">Int32</span></span>|<span data-ttu-id="dfb95-141">MDM と EAS の両方に登録されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="dfb95-141">The number of devices enrolled in both MDM and EAS</span></span>|
|<span data-ttu-id="dfb95-142">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="dfb95-142">deviceOperatingSystemSummary</span></span>|[<span data-ttu-id="dfb95-143">deviceOperatingSystemSummary</span><span class="sxs-lookup"><span data-stu-id="dfb95-143">deviceOperatingSystemSummary</span></span>](../resources/intune_devices_deviceoperatingsystemsummary.md)|<span data-ttu-id="dfb95-144">デバイスのオペレーティング システムの概要。</span><span class="sxs-lookup"><span data-stu-id="dfb95-144">Device operating system summary.</span></span>|
|<span data-ttu-id="dfb95-145">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="dfb95-145">deviceExchangeAccessStateSummary</span></span>|[<span data-ttu-id="dfb95-146">deviceExchangeAccessStateSummary</span><span class="sxs-lookup"><span data-stu-id="dfb95-146">deviceExchangeAccessStateSummary</span></span>](../resources/intune_devices_deviceexchangeaccessstatesummary.md)|<span data-ttu-id="dfb95-147">Intune での Exchange アクセス状態の配布</span><span class="sxs-lookup"><span data-stu-id="dfb95-147">Distribution of Exchange Access State in Intune</span></span>|



## <a name="response"></a><span data-ttu-id="dfb95-148">応答</span><span class="sxs-lookup"><span data-stu-id="dfb95-148">Response</span></span>
<span data-ttu-id="dfb95-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedDeviceOverview](../resources/intune_devices_manageddeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dfb95-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfb95-150">例</span><span class="sxs-lookup"><span data-stu-id="dfb95-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="dfb95-151">要求</span><span class="sxs-lookup"><span data-stu-id="dfb95-151">Request</span></span>
<span data-ttu-id="dfb95-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dfb95-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
Content-type: application/json
Content-length: 625

{
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```

### <a name="response"></a><span data-ttu-id="dfb95-153">応答</span><span class="sxs-lookup"><span data-stu-id="dfb95-153">Response</span></span>
<span data-ttu-id="dfb95-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dfb95-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 734

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "42a91653-1653-42a9-5316-a9425316a942",
  "enrolledDeviceCount": 3,
  "mdmEnrolledCount": 0,
  "dualEnrolledDeviceCount": 7,
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
    "androidCount": 12,
    "iosCount": 8,
    "macOSCount": 10,
    "windowsMobileCount": 2,
    "windowsCount": 12,
    "unknownCount": 12
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": 2,
    "blockedDeviceCount": 2,
    "quarantinedDeviceCount": 6,
    "unknownDeviceCount": 2,
    "unavailableDeviceCount": 6
  }
}
```



