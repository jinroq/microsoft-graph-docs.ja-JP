---
title: WindowsAutopilotDeploymentProfile を取得します。
description: WindowsAutopilotDeploymentProfile オブジェクトのプロパティと関係を参照してください。
author: tfitzmac
ms.openlocfilehash: e913aeac27a66ea5b139cb5ec4f03e24055e7c49
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344577"
---
# <a name="get-windowsautopilotdeploymentprofile"></a><span data-ttu-id="2b21d-103">WindowsAutopilotDeploymentProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b21d-103">Get windowsAutopilotDeploymentProfile</span></span>

> <span data-ttu-id="2b21d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b21d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b21d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b21d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b21d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b21d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b21d-107">[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b21d-107">Read properties and relationships of the [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b21d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2b21d-108">Prerequisites</span></span>
<span data-ttu-id="2b21d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b21d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b21d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b21d-111">Permission type</span></span>|<span data-ttu-id="2b21d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b21d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b21d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b21d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b21d-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b21d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2b21d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b21d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b21d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b21d-116">Not supported.</span></span>|
|<span data-ttu-id="2b21d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b21d-117">Application</span></span>|<span data-ttu-id="2b21d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b21d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b21d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b21d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/intendedDeploymentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2b21d-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2b21d-120">Optional query parameters</span></span>
<span data-ttu-id="2b21d-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b21d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2b21d-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b21d-122">Request headers</span></span>
|<span data-ttu-id="2b21d-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b21d-123">Header</span></span>|<span data-ttu-id="2b21d-124">値</span><span class="sxs-lookup"><span data-stu-id="2b21d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b21d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b21d-125">Authorization</span></span>|<span data-ttu-id="2b21d-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2b21d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b21d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="2b21d-127">Accept</span></span>|<span data-ttu-id="2b21d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2b21d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b21d-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b21d-129">Request body</span></span>
<span data-ttu-id="2b21d-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2b21d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b21d-131">応答</span><span class="sxs-lookup"><span data-stu-id="2b21d-131">Response</span></span>
<span data-ttu-id="2b21d-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2b21d-132">If successful, this method returns a `200 OK` response code and [windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b21d-133">例</span><span class="sxs-lookup"><span data-stu-id="2b21d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b21d-134">要求</span><span class="sxs-lookup"><span data-stu-id="2b21d-134">Request</span></span>
<span data-ttu-id="2b21d-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b21d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}
```

### <a name="response"></a><span data-ttu-id="2b21d-136">応答</span><span class="sxs-lookup"><span data-stu-id="2b21d-136">Response</span></span>
<span data-ttu-id="2b21d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2b21d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1276

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
    "id": "9d6394a9-94a9-9d63-a994-639da994639d",
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
    "deviceNameTemplate": "Device Name Template value"
  }
}
```





