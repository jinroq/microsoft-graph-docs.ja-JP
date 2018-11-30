---
title: RestrictedAppsViolation を更新します。
description: RestrictedAppsViolation オブジェクトのプロパティを更新します。
ms.openlocfilehash: ad6fcfd8571890a06877f503520533f2907fd3cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066529"
---
# <a name="update-restrictedappsviolation"></a><span data-ttu-id="d7eba-103">RestrictedAppsViolation を更新します。</span><span class="sxs-lookup"><span data-stu-id="d7eba-103">Update restrictedAppsViolation</span></span>

> <span data-ttu-id="d7eba-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d7eba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7eba-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7eba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d7eba-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7eba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d7eba-107">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d7eba-107">Update the properties of a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d7eba-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d7eba-108">Prerequisites</span></span>
<span data-ttu-id="d7eba-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7eba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7eba-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7eba-111">Permission type</span></span>|<span data-ttu-id="d7eba-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7eba-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d7eba-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7eba-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d7eba-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7eba-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d7eba-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7eba-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d7eba-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7eba-116">Not supported.</span></span>|
|<span data-ttu-id="d7eba-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7eba-117">Application</span></span>|<span data-ttu-id="d7eba-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7eba-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d7eba-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7eba-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
```

## <a name="request-headers"></a><span data-ttu-id="d7eba-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7eba-120">Request headers</span></span>
|<span data-ttu-id="d7eba-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7eba-121">Header</span></span>|<span data-ttu-id="d7eba-122">値</span><span class="sxs-lookup"><span data-stu-id="d7eba-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d7eba-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7eba-123">Authorization</span></span>|<span data-ttu-id="d7eba-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d7eba-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d7eba-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d7eba-125">Accept</span></span>|<span data-ttu-id="d7eba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d7eba-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7eba-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7eba-127">Request body</span></span>
<span data-ttu-id="d7eba-128">要求の本文に[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d7eba-128">In the request body, supply a JSON representation for the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

<span data-ttu-id="d7eba-129">[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="d7eba-129">The following table shows the properties that are required when you create the [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md).</span></span>

|<span data-ttu-id="d7eba-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7eba-130">Property</span></span>|<span data-ttu-id="d7eba-131">型</span><span class="sxs-lookup"><span data-stu-id="d7eba-131">Type</span></span>|<span data-ttu-id="d7eba-132">説明</span><span class="sxs-lookup"><span data-stu-id="d7eba-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7eba-133">id</span><span class="sxs-lookup"><span data-stu-id="d7eba-133">id</span></span>|<span data-ttu-id="d7eba-134">String</span><span class="sxs-lookup"><span data-stu-id="d7eba-134">String</span></span>|<span data-ttu-id="d7eba-135">オブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="d7eba-135">Unique identifier for the object.</span></span> <span data-ttu-id="d7eba-136">"Accountid"、deviceId、policyId、およびユーザー Id から構成されます。</span><span class="sxs-lookup"><span data-stu-id="d7eba-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="d7eba-137">userId</span><span class="sxs-lookup"><span data-stu-id="d7eba-137">userId</span></span>|<span data-ttu-id="d7eba-138">String</span><span class="sxs-lookup"><span data-stu-id="d7eba-138">String</span></span>|<span data-ttu-id="d7eba-139">ユーザーの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7eba-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="d7eba-140">userName</span><span class="sxs-lookup"><span data-stu-id="d7eba-140">userName</span></span>|<span data-ttu-id="d7eba-141">String</span><span class="sxs-lookup"><span data-stu-id="d7eba-141">String</span></span>|<span data-ttu-id="d7eba-142">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="d7eba-142">User name</span></span>|
|<span data-ttu-id="d7eba-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d7eba-143">managedDeviceId</span></span>|<span data-ttu-id="d7eba-144">String</span><span class="sxs-lookup"><span data-stu-id="d7eba-144">String</span></span>|<span data-ttu-id="d7eba-145">管理対象デバイスの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7eba-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="d7eba-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="d7eba-146">deviceName</span></span>|<span data-ttu-id="d7eba-147">String</span><span class="sxs-lookup"><span data-stu-id="d7eba-147">String</span></span>|<span data-ttu-id="d7eba-148">デバイス名</span><span class="sxs-lookup"><span data-stu-id="d7eba-148">Device name</span></span>|
|<span data-ttu-id="d7eba-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="d7eba-149">deviceConfigurationId</span></span>|<span data-ttu-id="d7eba-150">String</span><span class="sxs-lookup"><span data-stu-id="d7eba-150">String</span></span>|<span data-ttu-id="d7eba-151">デバイス構成プロファイルの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7eba-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="d7eba-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="d7eba-152">deviceConfigurationName</span></span>|<span data-ttu-id="d7eba-153">String</span><span class="sxs-lookup"><span data-stu-id="d7eba-153">String</span></span>|<span data-ttu-id="d7eba-154">デバイス構成のプロファイル名</span><span class="sxs-lookup"><span data-stu-id="d7eba-154">Device configuration profile name</span></span>|
|<span data-ttu-id="d7eba-155">platformType</span><span class="sxs-lookup"><span data-stu-id="d7eba-155">platformType</span></span>|[<span data-ttu-id="d7eba-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="d7eba-156">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="d7eba-157">プラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="d7eba-157">Platform type.</span></span> <span data-ttu-id="d7eba-158">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="d7eba-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="d7eba-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="d7eba-159">restrictedAppsState</span></span>|[<span data-ttu-id="d7eba-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="d7eba-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="d7eba-161">アプリケーションの状態を制限します。</span><span class="sxs-lookup"><span data-stu-id="d7eba-161">Restricted apps state.</span></span> <span data-ttu-id="d7eba-162">使用可能な値は、`prohibitedApps`、`notApprovedApps` です。</span><span class="sxs-lookup"><span data-stu-id="d7eba-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="d7eba-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="d7eba-163">restrictedApps</span></span>|<span data-ttu-id="d7eba-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d7eba-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="d7eba-165">違反した制限されたアプリケーションの一覧</span><span class="sxs-lookup"><span data-stu-id="d7eba-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="d7eba-166">応答</span><span class="sxs-lookup"><span data-stu-id="d7eba-166">Response</span></span>
<span data-ttu-id="d7eba-167">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d7eba-167">If successful, this method returns a `200 OK` response code and an updated [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7eba-168">例</span><span class="sxs-lookup"><span data-stu-id="d7eba-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="d7eba-169">要求</span><span class="sxs-lookup"><span data-stu-id="d7eba-169">Request</span></span>
<span data-ttu-id="d7eba-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d7eba-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations/{restrictedAppsViolationId}
Content-type: application/json
Content-length: 502

{
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="d7eba-171">応答</span><span class="sxs-lookup"><span data-stu-id="d7eba-171">Response</span></span>
<span data-ttu-id="d7eba-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d7eba-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "53f99903-9903-53f9-0399-f9530399f953",
  "userId": "User Id value",
  "userName": "User Name value",
  "managedDeviceId": "Managed Device Id value",
  "deviceName": "Device Name value",
  "deviceConfigurationId": "Device Configuration Id value",
  "deviceConfigurationName": "Device Configuration Name value",
  "platformType": "androidForWork",
  "restrictedAppsState": "notApprovedApps",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "App Id value"
    }
  ]
}
```





