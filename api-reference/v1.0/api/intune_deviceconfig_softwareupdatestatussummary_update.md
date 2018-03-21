# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="258e7-101">softwareUpdateStatusSummary の更新</span><span class="sxs-lookup"><span data-stu-id="258e7-101">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="258e7-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="258e7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="258e7-103">[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="258e7-103">Update the properties of a [calendar](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="258e7-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="258e7-104">Prerequisites</span></span>
<span data-ttu-id="258e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="258e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="258e7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="258e7-107">Permission type</span></span>|<span data-ttu-id="258e7-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="258e7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="258e7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="258e7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="258e7-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="258e7-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="258e7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="258e7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="258e7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="258e7-112">Not supported.</span></span>|
|<span data-ttu-id="258e7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="258e7-113">Application</span></span>|<span data-ttu-id="258e7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="258e7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="258e7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="258e7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="258e7-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="258e7-116">Request headers</span></span>
|<span data-ttu-id="258e7-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="258e7-117">Header</span></span>|<span data-ttu-id="258e7-118">値</span><span class="sxs-lookup"><span data-stu-id="258e7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="258e7-119">承認</span><span class="sxs-lookup"><span data-stu-id="258e7-119">Authorization</span></span>|<span data-ttu-id="258e7-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="258e7-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="258e7-121">承諾</span><span class="sxs-lookup"><span data-stu-id="258e7-121">Accept</span></span>|<span data-ttu-id="258e7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="258e7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="258e7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="258e7-123">Request body</span></span>
<span data-ttu-id="258e7-124">要求本文で、[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="258e7-124">In the request body, supply a JSON representation of [Calendar](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="258e7-125">次の表に、[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="258e7-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="258e7-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="258e7-126">Property</span></span>|<span data-ttu-id="258e7-127">型</span><span class="sxs-lookup"><span data-stu-id="258e7-127">Type</span></span>|<span data-ttu-id="258e7-128">説明</span><span class="sxs-lookup"><span data-stu-id="258e7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="258e7-129">id</span><span class="sxs-lookup"><span data-stu-id="258e7-129">id</span></span>|<span data-ttu-id="258e7-130">String</span><span class="sxs-lookup"><span data-stu-id="258e7-130">String</span></span>|<span data-ttu-id="258e7-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="258e7-131">Name of the entity.</span></span>|
|<span data-ttu-id="258e7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="258e7-132">displayName</span></span>|<span data-ttu-id="258e7-133">String</span><span class="sxs-lookup"><span data-stu-id="258e7-133">String</span></span>|<span data-ttu-id="258e7-134">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="258e7-134">The friendly name of the DLP policy for this event.</span></span>|
|<span data-ttu-id="258e7-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="258e7-135">compliantDeviceCount</span></span>|<span data-ttu-id="258e7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-136">Int32</span></span>|<span data-ttu-id="258e7-137">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-137">Number of compliant devices.</span></span>|
|<span data-ttu-id="258e7-138">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="258e7-138">nonCompliantDeviceCount</span></span>|<span data-ttu-id="258e7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-139">Int32</span></span>|<span data-ttu-id="258e7-140">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-140">Number of non compliant devices.</span></span>|
|<span data-ttu-id="258e7-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="258e7-141">remediatedDeviceCount</span></span>|<span data-ttu-id="258e7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-142">Int32</span></span>|<span data-ttu-id="258e7-143">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-143">Number of remediated devices.</span></span>|
|<span data-ttu-id="258e7-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="258e7-144">errorDeviceCount</span></span>|<span data-ttu-id="258e7-145">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-145">Int32</span></span>|<span data-ttu-id="258e7-146">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-146">Number of devices had error.</span></span>|
|<span data-ttu-id="258e7-147">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="258e7-147">unknownDeviceCount</span></span>|<span data-ttu-id="258e7-148">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-148">Int32</span></span>|<span data-ttu-id="258e7-149">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-149">Number of unknown devices.</span></span>|
|<span data-ttu-id="258e7-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="258e7-150">conflictDeviceCount</span></span>|<span data-ttu-id="258e7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-151">Int32</span></span>|<span data-ttu-id="258e7-152">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-152">Number of conflict devices.</span></span>|
|<span data-ttu-id="258e7-153">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="258e7-153">notApplicableDeviceCount</span></span>|<span data-ttu-id="258e7-154">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-154">Int32</span></span>|<span data-ttu-id="258e7-155">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-155">Number of not applicable devices.</span></span>|
|<span data-ttu-id="258e7-156">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="258e7-156">compliantUserCount</span></span>|<span data-ttu-id="258e7-157">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-157">Int32</span></span>|<span data-ttu-id="258e7-158">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-158">Number of users: 542</span></span>|
|<span data-ttu-id="258e7-159">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="258e7-159">nonCompliantUserCount</span></span>|<span data-ttu-id="258e7-160">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-160">Int32</span></span>|<span data-ttu-id="258e7-161">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-161">Number of non compliant users.</span></span>|
|<span data-ttu-id="258e7-162">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="258e7-162">remediatedUserCount</span></span>|<span data-ttu-id="258e7-163">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-163">Int32</span></span>|<span data-ttu-id="258e7-164">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-164">Number of users: 542</span></span>|
|<span data-ttu-id="258e7-165">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="258e7-165">errorUserCount</span></span>|<span data-ttu-id="258e7-166">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-166">Int32</span></span>|<span data-ttu-id="258e7-167">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-167">Number of users had error.</span></span>|
|<span data-ttu-id="258e7-168">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="258e7-168">unknownUserCount</span></span>|<span data-ttu-id="258e7-169">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-169">Int32</span></span>|<span data-ttu-id="258e7-170">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-170">Number of users: 542</span></span>|
|<span data-ttu-id="258e7-171">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="258e7-171">conflictUserCount</span></span>|<span data-ttu-id="258e7-172">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-172">Int32</span></span>|<span data-ttu-id="258e7-173">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-173">Number of users: 542</span></span>|
|<span data-ttu-id="258e7-174">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="258e7-174">notApplicableUserCount</span></span>|<span data-ttu-id="258e7-175">Int32</span><span class="sxs-lookup"><span data-stu-id="258e7-175">Int32</span></span>|<span data-ttu-id="258e7-176">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="258e7-176">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="258e7-177">応答</span><span class="sxs-lookup"><span data-stu-id="258e7-177">Response</span></span>
<span data-ttu-id="258e7-178">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="258e7-178">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="258e7-179">例</span><span class="sxs-lookup"><span data-stu-id="258e7-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="258e7-180">要求</span><span class="sxs-lookup"><span data-stu-id="258e7-180">Request</span></span>
<span data-ttu-id="258e7-181">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="258e7-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 452

{
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="258e7-182">応答</span><span class="sxs-lookup"><span data-stu-id="258e7-182">Response</span></span>
<span data-ttu-id="258e7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="258e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```



