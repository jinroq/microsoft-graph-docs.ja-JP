---
title: AzureADWindowsAutopilotDeploymentProfile を取得する
description: AzureADWindowsAutopilotDeploymentProfile オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8e93664b3d601119405c4c4172ee337d60eadec7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35985604"
---
# <a name="get-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="0c029-103">AzureADWindowsAutopilotDeploymentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="0c029-103">Get azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="0c029-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c029-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c029-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c029-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c029-106">[AzureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0c029-106">Read properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c029-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0c029-107">Prerequisites</span></span>
<span data-ttu-id="0c029-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c029-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c029-110">Permission type</span></span>|<span data-ttu-id="0c029-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c029-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c029-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c029-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c029-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0c029-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0c029-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c029-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c029-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c029-115">Not supported.</span></span>|
|<span data-ttu-id="0c029-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c029-116">Application</span></span>|<span data-ttu-id="0c029-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c029-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c029-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c029-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c029-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0c029-119">Optional query parameters</span></span>
<span data-ttu-id="0c029-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0c029-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c029-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c029-121">Request headers</span></span>
|<span data-ttu-id="0c029-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c029-122">Header</span></span>|<span data-ttu-id="0c029-123">値</span><span class="sxs-lookup"><span data-stu-id="0c029-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c029-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c029-124">Authorization</span></span>|<span data-ttu-id="0c029-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c029-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c029-126">承諾</span><span class="sxs-lookup"><span data-stu-id="0c029-126">Accept</span></span>|<span data-ttu-id="0c029-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0c029-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c029-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c029-128">Request body</span></span>
<span data-ttu-id="0c029-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0c029-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c029-130">応答</span><span class="sxs-lookup"><span data-stu-id="0c029-130">Response</span></span>
<span data-ttu-id="0c029-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0c029-131">If successful, this method returns a `200 OK` response code and [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c029-132">例</span><span class="sxs-lookup"><span data-stu-id="0c029-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c029-133">要求</span><span class="sxs-lookup"><span data-stu-id="0c029-133">Request</span></span>
<span data-ttu-id="0c029-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c029-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="0c029-135">応答</span><span class="sxs-lookup"><span data-stu-id="0c029-135">Response</span></span>
<span data-ttu-id="0c029-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c029-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1416

{
  "value": {
    "@odata.type": "#microsoft.graph.azureADWindowsAutopilotDeploymentProfile",
    "id": "e2ec4e69-4e69-e2ec-694e-ece2694eece2",
    "displayName": "Display Name value",
    "description": "Description value",
    "language": "Language value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "outOfBoxExperienceSettings": {
      "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
      "hidePrivacySettings": true,
      "hideEULA": true,
      "userType": "standard",
      "deviceUsageType": "shared",
      "skipKeyboardSelectionPage": true,
      "hideEscapeLink": true
    },
    "enrollmentStatusScreenSettings": {
      "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
      "hideInstallationProgress": true,
      "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
      "blockDeviceSetupRetryByUser": true,
      "allowLogCollectionOnInstallFailure": true,
      "customErrorMessage": "Custom Error Message value",
      "installProgressTimeoutInMinutes": 15,
      "allowDeviceUseOnInstallFailure": true
    },
    "extractHardwareHash": true,
    "deviceNameTemplate": "Device Name Template value",
    "deviceType": "surfaceHub2",
    "enableWhiteGlove": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```





