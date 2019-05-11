---
title: RestrictedAppsViolation を作成する
description: 新しい restrictedAppsViolation オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5aea694e901948a7c288083f5372bde2dd68f494
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922691"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="d87e7-103">RestrictedAppsViolation を作成する</span><span class="sxs-lookup"><span data-stu-id="d87e7-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="d87e7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d87e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d87e7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d87e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d87e7-106">新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d87e7-106">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d87e7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d87e7-107">Prerequisites</span></span>
<span data-ttu-id="d87e7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d87e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d87e7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d87e7-110">Permission type</span></span>|<span data-ttu-id="d87e7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d87e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d87e7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d87e7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d87e7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87e7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d87e7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d87e7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d87e7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d87e7-115">Not supported.</span></span>|
|<span data-ttu-id="d87e7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d87e7-116">Application</span></span>|<span data-ttu-id="d87e7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d87e7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d87e7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d87e7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="d87e7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d87e7-119">Request headers</span></span>
|<span data-ttu-id="d87e7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d87e7-120">Header</span></span>|<span data-ttu-id="d87e7-121">値</span><span class="sxs-lookup"><span data-stu-id="d87e7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d87e7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d87e7-122">Authorization</span></span>|<span data-ttu-id="d87e7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d87e7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d87e7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d87e7-124">Accept</span></span>|<span data-ttu-id="d87e7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d87e7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d87e7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d87e7-126">Request body</span></span>
<span data-ttu-id="d87e7-127">要求本文で、restrictedAppsViolation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d87e7-127">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="d87e7-128">次の表に、restrictedAppsViolation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d87e7-128">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="d87e7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d87e7-129">Property</span></span>|<span data-ttu-id="d87e7-130">型</span><span class="sxs-lookup"><span data-stu-id="d87e7-130">Type</span></span>|<span data-ttu-id="d87e7-131">説明</span><span class="sxs-lookup"><span data-stu-id="d87e7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d87e7-132">id</span><span class="sxs-lookup"><span data-stu-id="d87e7-132">id</span></span>|<span data-ttu-id="d87e7-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d87e7-133">String</span></span>|<span data-ttu-id="d87e7-134">オブジェクトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d87e7-134">Unique identifier for the object.</span></span> <span data-ttu-id="d87e7-135">AccountId、deviceId、policyId、および userId から構成されます。</span><span class="sxs-lookup"><span data-stu-id="d87e7-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="d87e7-136">userId</span><span class="sxs-lookup"><span data-stu-id="d87e7-136">userId</span></span>|<span data-ttu-id="d87e7-137">String</span><span class="sxs-lookup"><span data-stu-id="d87e7-137">String</span></span>|<span data-ttu-id="d87e7-138">ユーザーの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="d87e7-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="d87e7-139">userName</span><span class="sxs-lookup"><span data-stu-id="d87e7-139">userName</span></span>|<span data-ttu-id="d87e7-140">String</span><span class="sxs-lookup"><span data-stu-id="d87e7-140">String</span></span>|<span data-ttu-id="d87e7-141">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="d87e7-141">User name</span></span>|
|<span data-ttu-id="d87e7-142">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="d87e7-142">managedDeviceId</span></span>|<span data-ttu-id="d87e7-143">String</span><span class="sxs-lookup"><span data-stu-id="d87e7-143">String</span></span>|<span data-ttu-id="d87e7-144">管理デバイスの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="d87e7-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="d87e7-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="d87e7-145">deviceName</span></span>|<span data-ttu-id="d87e7-146">String</span><span class="sxs-lookup"><span data-stu-id="d87e7-146">String</span></span>|<span data-ttu-id="d87e7-147">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="d87e7-147">Device name</span></span>|
|<span data-ttu-id="d87e7-148">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="d87e7-148">deviceConfigurationId</span></span>|<span data-ttu-id="d87e7-149">String</span><span class="sxs-lookup"><span data-stu-id="d87e7-149">String</span></span>|<span data-ttu-id="d87e7-150">デバイス構成プロファイルの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="d87e7-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="d87e7-151">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="d87e7-151">deviceConfigurationName</span></span>|<span data-ttu-id="d87e7-152">String</span><span class="sxs-lookup"><span data-stu-id="d87e7-152">String</span></span>|<span data-ttu-id="d87e7-153">デバイス構成プロファイル名</span><span class="sxs-lookup"><span data-stu-id="d87e7-153">Device configuration profile name</span></span>|
|<span data-ttu-id="d87e7-154">platformType</span><span class="sxs-lookup"><span data-stu-id="d87e7-154">platformType</span></span>|[<span data-ttu-id="d87e7-155">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="d87e7-155">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="d87e7-156">プラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="d87e7-156">Platform type.</span></span> <span data-ttu-id="d87e7-157">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="d87e7-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="d87e7-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="d87e7-158">restrictedAppsState</span></span>|[<span data-ttu-id="d87e7-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="d87e7-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="d87e7-160">制限付きアプリの状態。</span><span class="sxs-lookup"><span data-stu-id="d87e7-160">Restricted apps state.</span></span> <span data-ttu-id="d87e7-161">可能な値は、`prohibitedApps`、`notApprovedApps` です。</span><span class="sxs-lookup"><span data-stu-id="d87e7-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="d87e7-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="d87e7-162">restrictedApps</span></span>|<span data-ttu-id="d87e7-163">[Manageddevicereportedapp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d87e7-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="d87e7-164">違反した制限付きアプリの一覧</span><span class="sxs-lookup"><span data-stu-id="d87e7-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="d87e7-165">応答</span><span class="sxs-lookup"><span data-stu-id="d87e7-165">Response</span></span>
<span data-ttu-id="d87e7-166">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d87e7-166">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d87e7-167">例</span><span class="sxs-lookup"><span data-stu-id="d87e7-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="d87e7-168">要求</span><span class="sxs-lookup"><span data-stu-id="d87e7-168">Request</span></span>
<span data-ttu-id="d87e7-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d87e7-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d87e7-170">応答</span><span class="sxs-lookup"><span data-stu-id="d87e7-170">Response</span></span>
<span data-ttu-id="d87e7-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d87e7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




