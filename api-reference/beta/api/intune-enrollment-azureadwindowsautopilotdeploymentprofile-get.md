---
title: azureADWindowsAutopilotDeploymentProfile を取得する
description: azureADWindowsAutopilotDeploymentProfile オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2a05530caf4b5967f7b0a6ce0c0a8ee4e362fa9
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30969009"
---
# <a name="get-azureadwindowsautopilotdeploymentprofile"></a><span data-ttu-id="3087b-103">azureADWindowsAutopilotDeploymentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="3087b-103">Get azureADWindowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="3087b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3087b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3087b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3087b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3087b-106">[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3087b-106">Read properties and relationships of the [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3087b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3087b-107">Prerequisites</span></span>
<span data-ttu-id="3087b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3087b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3087b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3087b-110">Permission type</span></span>|<span data-ttu-id="3087b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3087b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3087b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3087b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3087b-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="3087b-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="3087b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3087b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3087b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3087b-115">Not supported.</span></span>|
|<span data-ttu-id="3087b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3087b-116">Application</span></span>|<span data-ttu-id="3087b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3087b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3087b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3087b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3087b-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3087b-119">Optional query parameters</span></span>
<span data-ttu-id="3087b-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3087b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3087b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3087b-121">Request headers</span></span>
|<span data-ttu-id="3087b-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3087b-122">Header</span></span>|<span data-ttu-id="3087b-123">値</span><span class="sxs-lookup"><span data-stu-id="3087b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3087b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3087b-124">Authorization</span></span>|<span data-ttu-id="3087b-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3087b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3087b-126">承諾</span><span class="sxs-lookup"><span data-stu-id="3087b-126">Accept</span></span>|<span data-ttu-id="3087b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3087b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3087b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3087b-128">Request body</span></span>
<span data-ttu-id="3087b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3087b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3087b-130">応答</span><span class="sxs-lookup"><span data-stu-id="3087b-130">Response</span></span>
<span data-ttu-id="3087b-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3087b-131">If successful, this method returns a `200 OK` response code and [azureADWindowsAutopilotDeploymentProfile](../resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3087b-132">例</span><span class="sxs-lookup"><span data-stu-id="3087b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3087b-133">要求</span><span class="sxs-lookup"><span data-stu-id="3087b-133">Request</span></span>
<span data-ttu-id="3087b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3087b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="3087b-135">応答</span><span class="sxs-lookup"><span data-stu-id="3087b-135">Response</span></span>
<span data-ttu-id="3087b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3087b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1348

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
    "enableWhiteGlove": true
  }
}
```




