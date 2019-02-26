---
title: restrictedAppsViolation を作成する
description: 新しい restrictedAppsViolation オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbba9348e8b97125651951bdb4df424dc3b9fe47
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146404"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="37207-103">restrictedAppsViolation を作成する</span><span class="sxs-lookup"><span data-stu-id="37207-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="37207-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37207-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37207-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="37207-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37207-106">新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="37207-106">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37207-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="37207-107">Prerequisites</span></span>
<span data-ttu-id="37207-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37207-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="37207-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37207-110">Permission type</span></span>|<span data-ttu-id="37207-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="37207-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37207-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37207-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37207-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37207-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37207-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37207-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37207-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37207-115">Not supported.</span></span>|
|<span data-ttu-id="37207-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37207-116">Application</span></span>|<span data-ttu-id="37207-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37207-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37207-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37207-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="37207-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37207-119">Request headers</span></span>
|<span data-ttu-id="37207-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37207-120">Header</span></span>|<span data-ttu-id="37207-121">値</span><span class="sxs-lookup"><span data-stu-id="37207-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37207-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37207-122">Authorization</span></span>|<span data-ttu-id="37207-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="37207-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37207-124">承諾</span><span class="sxs-lookup"><span data-stu-id="37207-124">Accept</span></span>|<span data-ttu-id="37207-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37207-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37207-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="37207-126">Request body</span></span>
<span data-ttu-id="37207-127">要求本文で、restrictedAppsViolation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="37207-127">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="37207-128">次の表に、restrictedAppsViolation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="37207-128">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="37207-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37207-129">Property</span></span>|<span data-ttu-id="37207-130">型</span><span class="sxs-lookup"><span data-stu-id="37207-130">Type</span></span>|<span data-ttu-id="37207-131">説明</span><span class="sxs-lookup"><span data-stu-id="37207-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37207-132">id</span><span class="sxs-lookup"><span data-stu-id="37207-132">id</span></span>|<span data-ttu-id="37207-133">文字列</span><span class="sxs-lookup"><span data-stu-id="37207-133">String</span></span>|<span data-ttu-id="37207-134">オブジェクトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="37207-134">Unique identifier for the object.</span></span> <span data-ttu-id="37207-135">accountId、deviceId、policyid、および userId から構成されます。</span><span class="sxs-lookup"><span data-stu-id="37207-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="37207-136">userId</span><span class="sxs-lookup"><span data-stu-id="37207-136">userId</span></span>|<span data-ttu-id="37207-137">String</span><span class="sxs-lookup"><span data-stu-id="37207-137">String</span></span>|<span data-ttu-id="37207-138">ユーザーの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="37207-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="37207-139">userName</span><span class="sxs-lookup"><span data-stu-id="37207-139">userName</span></span>|<span data-ttu-id="37207-140">String</span><span class="sxs-lookup"><span data-stu-id="37207-140">String</span></span>|<span data-ttu-id="37207-141">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="37207-141">User name</span></span>|
|<span data-ttu-id="37207-142">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="37207-142">managedDeviceId</span></span>|<span data-ttu-id="37207-143">String</span><span class="sxs-lookup"><span data-stu-id="37207-143">String</span></span>|<span data-ttu-id="37207-144">管理デバイスの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="37207-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="37207-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="37207-145">deviceName</span></span>|<span data-ttu-id="37207-146">String</span><span class="sxs-lookup"><span data-stu-id="37207-146">String</span></span>|<span data-ttu-id="37207-147">デバイス名</span><span class="sxs-lookup"><span data-stu-id="37207-147">Device name</span></span>|
|<span data-ttu-id="37207-148">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="37207-148">deviceConfigurationId</span></span>|<span data-ttu-id="37207-149">String</span><span class="sxs-lookup"><span data-stu-id="37207-149">String</span></span>|<span data-ttu-id="37207-150">デバイス構成プロファイルの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="37207-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="37207-151">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="37207-151">deviceConfigurationName</span></span>|<span data-ttu-id="37207-152">String</span><span class="sxs-lookup"><span data-stu-id="37207-152">String</span></span>|<span data-ttu-id="37207-153">デバイス構成プロファイル名</span><span class="sxs-lookup"><span data-stu-id="37207-153">Device configuration profile name</span></span>|
|<span data-ttu-id="37207-154">platformType</span><span class="sxs-lookup"><span data-stu-id="37207-154">platformType</span></span>|[<span data-ttu-id="37207-155">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="37207-155">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="37207-156">プラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="37207-156">Platform type.</span></span> <span data-ttu-id="37207-157">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="37207-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="37207-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="37207-158">restrictedAppsState</span></span>|[<span data-ttu-id="37207-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="37207-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="37207-160">制限付きアプリの状態。</span><span class="sxs-lookup"><span data-stu-id="37207-160">Restricted apps state.</span></span> <span data-ttu-id="37207-161">使用可能な値は、`prohibitedApps`、`notApprovedApps` です。</span><span class="sxs-lookup"><span data-stu-id="37207-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="37207-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="37207-162">restrictedApps</span></span>|<span data-ttu-id="37207-163">[manageddevicereportedapp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="37207-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="37207-164">違反した制限付きアプリの一覧</span><span class="sxs-lookup"><span data-stu-id="37207-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="37207-165">応答</span><span class="sxs-lookup"><span data-stu-id="37207-165">Response</span></span>
<span data-ttu-id="37207-166">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="37207-166">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37207-167">例</span><span class="sxs-lookup"><span data-stu-id="37207-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="37207-168">要求</span><span class="sxs-lookup"><span data-stu-id="37207-168">Request</span></span>
<span data-ttu-id="37207-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="37207-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37207-170">応答</span><span class="sxs-lookup"><span data-stu-id="37207-170">Response</span></span>
<span data-ttu-id="37207-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="37207-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




