---
title: settingStateDeviceSummary の作成
description: 新しい settingStateDeviceSummary オブジェクトを作成します。
ms.openlocfilehash: 8176db0e79e0775ceaa970089942eb3acda1ba37
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023669"
---
# <a name="create-settingstatedevicesummary"></a><span data-ttu-id="9d6dd-103">settingStateDeviceSummary の作成</span><span class="sxs-lookup"><span data-stu-id="9d6dd-103">Create settingStateDeviceSummary</span></span>

> <span data-ttu-id="9d6dd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d6dd-105">新しい [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-105">Create a new [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d6dd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9d6dd-106">Prerequisites</span></span>
<span data-ttu-id="9d6dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d6dd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d6dd-109">Permission type</span></span>|<span data-ttu-id="9d6dd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d6dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d6dd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d6dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d6dd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d6dd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d6dd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d6dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d6dd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-114">Not supported.</span></span>|
|<span data-ttu-id="9d6dd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d6dd-115">Application</span></span>|<span data-ttu-id="9d6dd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d6dd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d6dd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="9d6dd-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d6dd-118">Request headers</span></span>
|<span data-ttu-id="9d6dd-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d6dd-119">Header</span></span>|<span data-ttu-id="9d6dd-120">値</span><span class="sxs-lookup"><span data-stu-id="9d6dd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d6dd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d6dd-121">Authorization</span></span>|<span data-ttu-id="9d6dd-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d6dd-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9d6dd-123">Accept</span></span>|<span data-ttu-id="9d6dd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9d6dd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d6dd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d6dd-125">Request body</span></span>
<span data-ttu-id="9d6dd-126">要求本文で、settingStateDeviceSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-126">In the request body, supply a JSON representation for the settingStateDeviceSummary object.</span></span>

<span data-ttu-id="9d6dd-127">次の表に、settingStateDeviceSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-127">The following table shows the properties that are required when you create the settingStateDeviceSummary.</span></span>

|<span data-ttu-id="9d6dd-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d6dd-128">Property</span></span>|<span data-ttu-id="9d6dd-129">型</span><span class="sxs-lookup"><span data-stu-id="9d6dd-129">Type</span></span>|<span data-ttu-id="9d6dd-130">説明</span><span class="sxs-lookup"><span data-stu-id="9d6dd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d6dd-131">id</span><span class="sxs-lookup"><span data-stu-id="9d6dd-131">id</span></span>|<span data-ttu-id="9d6dd-132">String</span><span class="sxs-lookup"><span data-stu-id="9d6dd-132">String</span></span>|<span data-ttu-id="9d6dd-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-133">Key of the entity.</span></span>|
|<span data-ttu-id="9d6dd-134">settingName</span><span class="sxs-lookup"><span data-stu-id="9d6dd-134">settingName</span></span>|<span data-ttu-id="9d6dd-135">String</span><span class="sxs-lookup"><span data-stu-id="9d6dd-135">String</span></span>|<span data-ttu-id="9d6dd-136">設定の名前</span><span class="sxs-lookup"><span data-stu-id="9d6dd-136">Name of the setting</span></span>|
|<span data-ttu-id="9d6dd-137">instancePath</span><span class="sxs-lookup"><span data-stu-id="9d6dd-137">instancePath</span></span>|<span data-ttu-id="9d6dd-138">String</span><span class="sxs-lookup"><span data-stu-id="9d6dd-138">String</span></span>|<span data-ttu-id="9d6dd-139">設定の InstancePath の名前</span><span class="sxs-lookup"><span data-stu-id="9d6dd-139">Name of the InstancePath for the setting</span></span>|
|<span data-ttu-id="9d6dd-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d6dd-140">unknownDeviceCount</span></span>|<span data-ttu-id="9d6dd-141">Int32</span><span class="sxs-lookup"><span data-stu-id="9d6dd-141">Int32</span></span>|<span data-ttu-id="9d6dd-142">設定の不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9d6dd-142">Device Unkown count for the setting</span></span>|
|<span data-ttu-id="9d6dd-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d6dd-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="9d6dd-144">Int32</span><span class="sxs-lookup"><span data-stu-id="9d6dd-144">Int32</span></span>|<span data-ttu-id="9d6dd-145">設定の該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9d6dd-145">Device Not Applicable count for the setting</span></span>|
|<span data-ttu-id="9d6dd-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d6dd-146">compliantDeviceCount</span></span>|<span data-ttu-id="9d6dd-147">Int32</span><span class="sxs-lookup"><span data-stu-id="9d6dd-147">Int32</span></span>|<span data-ttu-id="9d6dd-148">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9d6dd-148">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="9d6dd-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d6dd-149">remediatedDeviceCount</span></span>|<span data-ttu-id="9d6dd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="9d6dd-150">Int32</span></span>|<span data-ttu-id="9d6dd-151">設定の準拠しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9d6dd-151">Device Compliant count for the setting</span></span>|
|<span data-ttu-id="9d6dd-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d6dd-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="9d6dd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="9d6dd-153">Int32</span></span>|<span data-ttu-id="9d6dd-154">設定の準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="9d6dd-154">Device NonCompliant count for the setting</span></span>|
|<span data-ttu-id="9d6dd-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d6dd-155">errorDeviceCount</span></span>|<span data-ttu-id="9d6dd-156">Int32</span><span class="sxs-lookup"><span data-stu-id="9d6dd-156">Int32</span></span>|<span data-ttu-id="9d6dd-157">設定のデバイス エラーの数</span><span class="sxs-lookup"><span data-stu-id="9d6dd-157">Device error count for the setting</span></span>|
|<span data-ttu-id="9d6dd-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="9d6dd-158">conflictDeviceCount</span></span>|<span data-ttu-id="9d6dd-159">Int32</span><span class="sxs-lookup"><span data-stu-id="9d6dd-159">Int32</span></span>|<span data-ttu-id="9d6dd-160">設定のデバイス競合エラーの数</span><span class="sxs-lookup"><span data-stu-id="9d6dd-160">Device conflict error count for the setting</span></span>|



## <a name="response"></a><span data-ttu-id="9d6dd-161">応答</span><span class="sxs-lookup"><span data-stu-id="9d6dd-161">Response</span></span>
<span data-ttu-id="9d6dd-162">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-162">If successful, this method returns a `201 Created` response code and a [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d6dd-163">例</span><span class="sxs-lookup"><span data-stu-id="9d6dd-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d6dd-164">要求</span><span class="sxs-lookup"><span data-stu-id="9d6dd-164">Request</span></span>
<span data-ttu-id="9d6dd-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="9d6dd-166">応答</span><span class="sxs-lookup"><span data-stu-id="9d6dd-166">Response</span></span>
<span data-ttu-id="9d6dd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d6dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
  "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
  "settingName": "Setting Name value",
  "instancePath": "Instance Path value",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



