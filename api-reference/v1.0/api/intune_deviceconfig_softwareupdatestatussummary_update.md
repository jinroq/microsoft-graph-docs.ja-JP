# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="16790-101">softwareUpdateStatusSummary の更新</span><span class="sxs-lookup"><span data-stu-id="16790-101">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="16790-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16790-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16790-103">[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="16790-103">Update the properties of a [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16790-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="16790-104">Prerequisites</span></span>
<span data-ttu-id="16790-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16790-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16790-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16790-107">Permission type</span></span>|<span data-ttu-id="16790-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16790-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16790-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16790-109">Delegated (work or school account)</span></span>|<span data-ttu-id="16790-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16790-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16790-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16790-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16790-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16790-112">Not supported.</span></span>|
|<span data-ttu-id="16790-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16790-113">Application</span></span>|<span data-ttu-id="16790-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16790-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16790-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16790-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="16790-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16790-116">Request headers</span></span>
|<span data-ttu-id="16790-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16790-117">Header</span></span>|<span data-ttu-id="16790-118">値</span><span class="sxs-lookup"><span data-stu-id="16790-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16790-119">承認</span><span class="sxs-lookup"><span data-stu-id="16790-119">Authorization</span></span>|<span data-ttu-id="16790-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="16790-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16790-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="16790-121">Accept</span></span>|<span data-ttu-id="16790-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="16790-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16790-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="16790-123">Request body</span></span>
<span data-ttu-id="16790-124">要求本文で、[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="16790-124">In the request body, supply a JSON representation for the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="16790-125">次の表に、[softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="16790-125">The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md).</span></span>

|<span data-ttu-id="16790-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16790-126">Property</span></span>|<span data-ttu-id="16790-127">型</span><span class="sxs-lookup"><span data-stu-id="16790-127">Type</span></span>|<span data-ttu-id="16790-128">説明</span><span class="sxs-lookup"><span data-stu-id="16790-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16790-129">ID</span><span class="sxs-lookup"><span data-stu-id="16790-129">id</span></span>|<span data-ttu-id="16790-130">文字列</span><span class="sxs-lookup"><span data-stu-id="16790-130">String</span></span>|<span data-ttu-id="16790-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="16790-131">Key of the entity.</span></span>|
|<span data-ttu-id="16790-132">displayName</span><span class="sxs-lookup"><span data-stu-id="16790-132">displayName</span></span>|<span data-ttu-id="16790-133">文字列</span><span class="sxs-lookup"><span data-stu-id="16790-133">String</span></span>|<span data-ttu-id="16790-134">ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="16790-134">The name of the policy.</span></span>|
|<span data-ttu-id="16790-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16790-135">compliantDeviceCount</span></span>|<span data-ttu-id="16790-136">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-136">Int32</span></span>|<span data-ttu-id="16790-137">準拠デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16790-137">Number of compliant devices.</span></span>|
|<span data-ttu-id="16790-138">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16790-138">nonCompliantDeviceCount</span></span>|<span data-ttu-id="16790-139">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-139">Int32</span></span>|<span data-ttu-id="16790-140">準拠していないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16790-140">Number of non compliant devices.</span></span>|
|<span data-ttu-id="16790-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16790-141">remediatedDeviceCount</span></span>|<span data-ttu-id="16790-142">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-142">Int32</span></span>|<span data-ttu-id="16790-143">修復済みデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16790-143">Number of remediated devices.</span></span>|
|<span data-ttu-id="16790-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16790-144">errorDeviceCount</span></span>|<span data-ttu-id="16790-145">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-145">Int32</span></span>|<span data-ttu-id="16790-146">エラーが発生したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16790-146">Number of devices had error.</span></span>|
|<span data-ttu-id="16790-147">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16790-147">unknownDeviceCount</span></span>|<span data-ttu-id="16790-148">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-148">Int32</span></span>|<span data-ttu-id="16790-149">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16790-149">Number of unknown devices.</span></span>|
|<span data-ttu-id="16790-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16790-150">conflictDeviceCount</span></span>|<span data-ttu-id="16790-151">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-151">Int32</span></span>|<span data-ttu-id="16790-152">競合デバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16790-152">Number of conflict devices.</span></span>|
|<span data-ttu-id="16790-153">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="16790-153">notApplicableDeviceCount</span></span>|<span data-ttu-id="16790-154">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-154">Int32</span></span>|<span data-ttu-id="16790-155">該当しないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="16790-155">Number of not applicable devices.</span></span>|
|<span data-ttu-id="16790-156">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="16790-156">compliantUserCount</span></span>|<span data-ttu-id="16790-157">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-157">Int32</span></span>|<span data-ttu-id="16790-158">準拠ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16790-158">Number of compliant users.</span></span>|
|<span data-ttu-id="16790-159">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="16790-159">nonCompliantUserCount</span></span>|<span data-ttu-id="16790-160">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-160">Int32</span></span>|<span data-ttu-id="16790-161">準拠していないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16790-161">Number of non compliant users.</span></span>|
|<span data-ttu-id="16790-162">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="16790-162">remediatedUserCount</span></span>|<span data-ttu-id="16790-163">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-163">Int32</span></span>|<span data-ttu-id="16790-164">修復済みユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16790-164">Number of remediated users.</span></span>|
|<span data-ttu-id="16790-165">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="16790-165">errorUserCount</span></span>|<span data-ttu-id="16790-166">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-166">Int32</span></span>|<span data-ttu-id="16790-167">エラーが発生したユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16790-167">Number of users had error.</span></span>|
|<span data-ttu-id="16790-168">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="16790-168">unknownUserCount</span></span>|<span data-ttu-id="16790-169">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-169">Int32</span></span>|<span data-ttu-id="16790-170">不明なユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16790-170">Number of unknown users.</span></span>|
|<span data-ttu-id="16790-171">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="16790-171">conflictUserCount</span></span>|<span data-ttu-id="16790-172">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-172">Int32</span></span>|<span data-ttu-id="16790-173">競合ユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16790-173">Number of conflict users.</span></span>|
|<span data-ttu-id="16790-174">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="16790-174">notApplicableUserCount</span></span>|<span data-ttu-id="16790-175">Int32</span><span class="sxs-lookup"><span data-stu-id="16790-175">Int32</span></span>|<span data-ttu-id="16790-176">該当しないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="16790-176">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="16790-177">応答</span><span class="sxs-lookup"><span data-stu-id="16790-177">Response</span></span>
<span data-ttu-id="16790-178">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="16790-178">If successful, this method returns a `200 OK` response code and an updated [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16790-179">例</span><span class="sxs-lookup"><span data-stu-id="16790-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="16790-180">要求</span><span class="sxs-lookup"><span data-stu-id="16790-180">Request</span></span>
<span data-ttu-id="16790-181">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16790-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16790-182">応答</span><span class="sxs-lookup"><span data-stu-id="16790-182">Response</span></span>
<span data-ttu-id="16790-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16790-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








