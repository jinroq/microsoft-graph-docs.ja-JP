---
title: リスト depMacOSEnrollmentProfiles
description: depMacOSEnrollmentProfile オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e8cf635bb2108238f372a4434a88432831faa9c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801695"
---
# <a name="list-depmacosenrollmentprofiles"></a><span data-ttu-id="09713-103">リスト depMacOSEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="09713-103">List depMacOSEnrollmentProfiles</span></span>

> <span data-ttu-id="09713-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09713-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09713-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09713-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09713-106">[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="09713-106">List properties and relationships of the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09713-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="09713-107">Prerequisites</span></span>
<span data-ttu-id="09713-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09713-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09713-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09713-110">Permission type</span></span>|<span data-ttu-id="09713-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="09713-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09713-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09713-112">Delegated (work or school account)</span></span>|<span data-ttu-id="09713-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="09713-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="09713-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09713-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09713-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09713-115">Not supported.</span></span>|
|<span data-ttu-id="09713-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09713-116">Application</span></span>|<span data-ttu-id="09713-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09713-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09713-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09713-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="09713-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09713-119">Request headers</span></span>
|<span data-ttu-id="09713-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09713-120">Header</span></span>|<span data-ttu-id="09713-121">値</span><span class="sxs-lookup"><span data-stu-id="09713-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09713-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="09713-122">Authorization</span></span>|<span data-ttu-id="09713-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="09713-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09713-124">承諾</span><span class="sxs-lookup"><span data-stu-id="09713-124">Accept</span></span>|<span data-ttu-id="09713-125">application/json</span><span class="sxs-lookup"><span data-stu-id="09713-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09713-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="09713-126">Request body</span></span>
<span data-ttu-id="09713-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="09713-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09713-128">応答</span><span class="sxs-lookup"><span data-stu-id="09713-128">Response</span></span>
<span data-ttu-id="09713-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="09713-129">If successful, this method returns a `200 OK` response code and a collection of [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09713-130">例</span><span class="sxs-lookup"><span data-stu-id="09713-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="09713-131">要求</span><span class="sxs-lookup"><span data-stu-id="09713-131">Request</span></span>
<span data-ttu-id="09713-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09713-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="09713-133">応答</span><span class="sxs-lookup"><span data-stu-id="09713-133">Response</span></span>
<span data-ttu-id="09713-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09713-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
      "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
      "displayName": "Display Name value",
      "description": "Description value",
      "requiresUserAuthentication": true,
      "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
      "enableAuthenticationViaCompanyPortal": true,
      "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
      "isDefault": true,
      "supervisedModeEnabled": true,
      "supportDepartment": "Support Department value",
      "passCodeDisabled": true,
      "isMandatory": true,
      "locationDisabled": true,
      "supportPhoneNumber": "Support Phone Number value",
      "profileRemovalDisabled": true,
      "restoreBlocked": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true,
      "displayToneSetupDisabled": true,
      "privacyPaneDisabled": true,
      "deviceNameTemplate": "Device Name Template value",
      "registrationDisabled": true,
      "fileVaultDisabled": true,
      "iCloudDiagnosticsDisabled": true,
      "iCloudStorageDisabled": true,
      "chooseYourLockScreenDisabled": true
    }
  ]
}
```





