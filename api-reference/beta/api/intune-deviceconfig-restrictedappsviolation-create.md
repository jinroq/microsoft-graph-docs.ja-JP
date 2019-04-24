---
title: restrictedAppsViolation を作成する
description: 新しい restrictedAppsViolation オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1c207bc34403f831d86d9849faf2287210d7bb5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518185"
---
# <a name="create-restrictedappsviolation"></a><span data-ttu-id="7ff8b-103">restrictedAppsViolation を作成する</span><span class="sxs-lookup"><span data-stu-id="7ff8b-103">Create restrictedAppsViolation</span></span>

> <span data-ttu-id="7ff8b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ff8b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ff8b-106">新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-106">Create a new [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ff8b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7ff8b-107">Prerequisites</span></span>
<span data-ttu-id="7ff8b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ff8b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7ff8b-110">Permission type</span></span>|<span data-ttu-id="7ff8b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7ff8b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ff8b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7ff8b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ff8b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ff8b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7ff8b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7ff8b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ff8b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-115">Not supported.</span></span>|
|<span data-ttu-id="7ff8b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7ff8b-116">Application</span></span>|<span data-ttu-id="7ff8b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ff8b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7ff8b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurationRestrictedAppsViolations
```

## <a name="request-headers"></a><span data-ttu-id="7ff8b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ff8b-119">Request headers</span></span>
|<span data-ttu-id="7ff8b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ff8b-120">Header</span></span>|<span data-ttu-id="7ff8b-121">値</span><span class="sxs-lookup"><span data-stu-id="7ff8b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ff8b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ff8b-122">Authorization</span></span>|<span data-ttu-id="7ff8b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ff8b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7ff8b-124">Accept</span></span>|<span data-ttu-id="7ff8b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ff8b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ff8b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7ff8b-126">Request body</span></span>
<span data-ttu-id="7ff8b-127">要求本文で、restrictedAppsViolation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-127">In the request body, supply a JSON representation for the restrictedAppsViolation object.</span></span>

<span data-ttu-id="7ff8b-128">次の表に、restrictedAppsViolation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-128">The following table shows the properties that are required when you create the restrictedAppsViolation.</span></span>

|<span data-ttu-id="7ff8b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7ff8b-129">Property</span></span>|<span data-ttu-id="7ff8b-130">型</span><span class="sxs-lookup"><span data-stu-id="7ff8b-130">Type</span></span>|<span data-ttu-id="7ff8b-131">説明</span><span class="sxs-lookup"><span data-stu-id="7ff8b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ff8b-132">id</span><span class="sxs-lookup"><span data-stu-id="7ff8b-132">id</span></span>|<span data-ttu-id="7ff8b-133">String</span><span class="sxs-lookup"><span data-stu-id="7ff8b-133">String</span></span>|<span data-ttu-id="7ff8b-134">オブジェクトの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-134">Unique identifier for the object.</span></span> <span data-ttu-id="7ff8b-135">accountId、deviceId、policyid、および userId から構成されます。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-135">Composed from accountId, deviceId, policyId and userId</span></span>|
|<span data-ttu-id="7ff8b-136">userId</span><span class="sxs-lookup"><span data-stu-id="7ff8b-136">userId</span></span>|<span data-ttu-id="7ff8b-137">String</span><span class="sxs-lookup"><span data-stu-id="7ff8b-137">String</span></span>|<span data-ttu-id="7ff8b-138">ユーザーの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="7ff8b-138">User unique identifier, must be Guid</span></span>|
|<span data-ttu-id="7ff8b-139">userName</span><span class="sxs-lookup"><span data-stu-id="7ff8b-139">userName</span></span>|<span data-ttu-id="7ff8b-140">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7ff8b-140">String</span></span>|<span data-ttu-id="7ff8b-141">ユーザー名</span><span class="sxs-lookup"><span data-stu-id="7ff8b-141">User name</span></span>|
|<span data-ttu-id="7ff8b-142">manageddeviceid</span><span class="sxs-lookup"><span data-stu-id="7ff8b-142">managedDeviceId</span></span>|<span data-ttu-id="7ff8b-143">String</span><span class="sxs-lookup"><span data-stu-id="7ff8b-143">String</span></span>|<span data-ttu-id="7ff8b-144">管理デバイスの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="7ff8b-144">Managed device unique identifier, must be Guid</span></span>|
|<span data-ttu-id="7ff8b-145">deviceName</span><span class="sxs-lookup"><span data-stu-id="7ff8b-145">deviceName</span></span>|<span data-ttu-id="7ff8b-146">String</span><span class="sxs-lookup"><span data-stu-id="7ff8b-146">String</span></span>|<span data-ttu-id="7ff8b-147">[デバイス名]</span><span class="sxs-lookup"><span data-stu-id="7ff8b-147">Device name</span></span>|
|<span data-ttu-id="7ff8b-148">deviceConfigurationId</span><span class="sxs-lookup"><span data-stu-id="7ff8b-148">deviceConfigurationId</span></span>|<span data-ttu-id="7ff8b-149">String</span><span class="sxs-lookup"><span data-stu-id="7ff8b-149">String</span></span>|<span data-ttu-id="7ff8b-150">デバイス構成プロファイルの一意識別子。 Guid である必要があります</span><span class="sxs-lookup"><span data-stu-id="7ff8b-150">Device configuration profile unique identifier, must be Guid</span></span>|
|<span data-ttu-id="7ff8b-151">deviceConfigurationName</span><span class="sxs-lookup"><span data-stu-id="7ff8b-151">deviceConfigurationName</span></span>|<span data-ttu-id="7ff8b-152">String</span><span class="sxs-lookup"><span data-stu-id="7ff8b-152">String</span></span>|<span data-ttu-id="7ff8b-153">デバイス構成プロファイル名</span><span class="sxs-lookup"><span data-stu-id="7ff8b-153">Device configuration profile name</span></span>|
|<span data-ttu-id="7ff8b-154">platformType</span><span class="sxs-lookup"><span data-stu-id="7ff8b-154">platformType</span></span>|[<span data-ttu-id="7ff8b-155">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="7ff8b-155">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="7ff8b-156">プラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-156">Platform type.</span></span> <span data-ttu-id="7ff8b-157">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="7ff8b-158">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="7ff8b-158">restrictedAppsState</span></span>|[<span data-ttu-id="7ff8b-159">restrictedAppsState</span><span class="sxs-lookup"><span data-stu-id="7ff8b-159">restrictedAppsState</span></span>](../resources/intune-deviceconfig-restrictedappsstate.md)|<span data-ttu-id="7ff8b-160">制限付きアプリの状態。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-160">Restricted apps state.</span></span> <span data-ttu-id="7ff8b-161">可能な値は、`prohibitedApps`、`notApprovedApps` です。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-161">Possible values are: `prohibitedApps`, `notApprovedApps`.</span></span>|
|<span data-ttu-id="7ff8b-162">restrictedApps</span><span class="sxs-lookup"><span data-stu-id="7ff8b-162">restrictedApps</span></span>|<span data-ttu-id="7ff8b-163">[manageddevicereportedapp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7ff8b-163">[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md) collection</span></span>|<span data-ttu-id="7ff8b-164">違反した制限付きアプリの一覧</span><span class="sxs-lookup"><span data-stu-id="7ff8b-164">List of violated restricted apps</span></span>|



## <a name="response"></a><span data-ttu-id="7ff8b-165">応答</span><span class="sxs-lookup"><span data-stu-id="7ff8b-165">Response</span></span>
<span data-ttu-id="7ff8b-166">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-166">If successful, this method returns a `201 Created` response code and a [restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ff8b-167">例</span><span class="sxs-lookup"><span data-stu-id="7ff8b-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ff8b-168">要求</span><span class="sxs-lookup"><span data-stu-id="7ff8b-168">Request</span></span>
<span data-ttu-id="7ff8b-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ff8b-170">応答</span><span class="sxs-lookup"><span data-stu-id="7ff8b-170">Response</span></span>
<span data-ttu-id="7ff8b-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7ff8b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





