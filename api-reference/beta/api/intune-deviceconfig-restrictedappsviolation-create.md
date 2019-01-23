---
title: RestrictedAppsViolation を作成します。
description: 新しい restrictedAppsViolation オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a12707bde6b1feb852e2e91a4a28f9d0c3fb639
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411863"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="9e8f1-103">RestrictedAppsViolation を作成します。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="9e8f1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e8f1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e8f1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e8f1-107">新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-107">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e8f1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e8f1-108">Prerequisites</span></span>
<span data-ttu-id="9e8f1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9e8f1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e8f1-111">Permission type</span></span>|<span data-ttu-id="9e8f1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e8f1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e8f1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e8f1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e8f1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e8f1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e8f1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e8f1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e8f1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-116">Not supported.</span></span>|
|<span data-ttu-id="9e8f1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e8f1-117">Application</span></span>|<span data-ttu-id="9e8f1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e8f1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e8f1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="9e8f1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e8f1-120">Request headers</span></span>
|<span data-ttu-id="9e8f1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e8f1-121">Header</span></span>|<span data-ttu-id="9e8f1-122">値</span><span class="sxs-lookup"><span data-stu-id="9e8f1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e8f1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e8f1-123">Authorization</span></span>|<span data-ttu-id="9e8f1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e8f1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e8f1-125">Accept</span></span>|<span data-ttu-id="9e8f1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e8f1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e8f1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e8f1-127">Request body</span></span>
<span data-ttu-id="9e8f1-128">要求の本文に restrictedAppsViolation オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-128">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="9e8f1-129">次の表は、restrictedAppsViolation を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-129">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="9e8f1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e8f1-130">Property</span></span>|<span data-ttu-id="9e8f1-131">型</span><span class="sxs-lookup"><span data-stu-id="9e8f1-131">Type</span></span>|<span data-ttu-id="9e8f1-132">説明</span><span class="sxs-lookup"><span data-stu-id="9e8f1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e8f1-133">id</span><span class="sxs-lookup"><span data-stu-id="9e8f1-133">id</span></span>|<span data-ttu-id="9e8f1-134">String</span><span class="sxs-lookup"><span data-stu-id="9e8f1-134">String</span></span>|<span data-ttu-id="9e8f1-135">オブジェクトの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-135">Unique identifier for the object.</span></span> <span data-ttu-id="9e8f1-136">"Accountid"、deviceId、policyId、およびユーザー Id から構成されます。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-136">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="9e8f1-137">userId</span><span class="sxs-lookup"><span data-stu-id="9e8f1-137">userId</span></span>|<span data-ttu-id="9e8f1-138">String</span><span class="sxs-lookup"><span data-stu-id="9e8f1-138">String</span></span>|<span data-ttu-id="9e8f1-139">ユーザーの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-139">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="9e8f1-140">userName</span><span class="sxs-lookup"><span data-stu-id="9e8f1-140">userName</span></span>|<span data-ttu-id="9e8f1-141">String</span><span class="sxs-lookup"><span data-stu-id="9e8f1-141">String</span></span>|<span data-ttu-id="9e8f1-142">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="9e8f1-142">User name</span></span>|
|<span data-ttu-id="9e8f1-143">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="9e8f1-143">managedDeviceId</span></span>|<span data-ttu-id="9e8f1-144">String</span><span class="sxs-lookup"><span data-stu-id="9e8f1-144">String</span></span>|<span data-ttu-id="9e8f1-145">管理対象デバイスの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-145">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="9e8f1-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="9e8f1-146">deviceName</span></span>|<span data-ttu-id="9e8f1-147">String</span><span class="sxs-lookup"><span data-stu-id="9e8f1-147">String</span></span>|<span data-ttu-id="9e8f1-148">デバイス名</span><span class="sxs-lookup"><span data-stu-id="9e8f1-148">Device name</span></span>|
|<span data-ttu-id="9e8f1-149">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="9e8f1-149">deviceConfigurationId</span></span>|<span data-ttu-id="9e8f1-150">String</span><span class="sxs-lookup"><span data-stu-id="9e8f1-150">String</span></span>|<span data-ttu-id="9e8f1-151">デバイス構成プロファイルの一意の識別子の Guid にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-151">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="9e8f1-152">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="9e8f1-152">deviceConfigurationName</span></span>|<span data-ttu-id="9e8f1-153">String</span><span class="sxs-lookup"><span data-stu-id="9e8f1-153">String</span></span>|<span data-ttu-id="9e8f1-154">デバイス構成のプロファイル名</span><span class="sxs-lookup"><span data-stu-id="9e8f1-154">Device configuration profile name</span></span>|
|<span data-ttu-id="9e8f1-155">platformType</span><span class="sxs-lookup"><span data-stu-id="9e8f1-155">platformType</span></span>|[<span data-ttu-id="9e8f1-156">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="9e8f1-156">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="9e8f1-157">プラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-157">Platform type.</span></span> <span data-ttu-id="9e8f1-158">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="9e8f1-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="9e8f1-159">restrictedAppsState</span></span>|[<span data-ttu-id="9e8f1-160">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="9e8f1-160">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="9e8f1-161">アプリケーションの状態を制限します。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-161">Restricted apps state.</span></span> <span data-ttu-id="9e8f1-162">使用可能な値は、`prohibitedApps`、`notApprovedApps` です。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-162">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="9e8f1-163">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="9e8f1-163">restrictedApps</span></span>|<span data-ttu-id="9e8f1-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9e8f1-164">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="9e8f1-165">違反した制限されたアプリケーションの一覧</span><span class="sxs-lookup"><span data-stu-id="9e8f1-165">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="9e8f1-166">応答</span><span class="sxs-lookup"><span data-stu-id="9e8f1-166">Response</span></span>
<span data-ttu-id="9e8f1-167">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-167">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e8f1-168">例</span><span class="sxs-lookup"><span data-stu-id="9e8f1-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e8f1-169">要求</span><span class="sxs-lookup"><span data-stu-id="9e8f1-169">Request</span></span>
<span data-ttu-id="9e8f1-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationRestrictedAppsViolations
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
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

### <a name="response"></a><span data-ttu-id="9e8f1-171">応答</span><span class="sxs-lookup"><span data-stu-id="9e8f1-171">Response</span></span>
<span data-ttu-id="9e8f1-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e8f1-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




