---
title: リスト depEnrollmentProfiles
description: depEnrollmentProfile オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 382ec08d6a876fc16f1a32b554152f7c22219c69
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775150"
---
# <a name="list-depenrollmentprofiles"></a><span data-ttu-id="e43a7-103">リスト depEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="e43a7-103">List depEnrollmentProfiles</span></span>

> <span data-ttu-id="e43a7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e43a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e43a7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e43a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e43a7-106">[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e43a7-106">List properties and relationships of the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e43a7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e43a7-107">Prerequisites</span></span>
<span data-ttu-id="e43a7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e43a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e43a7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e43a7-110">Permission type</span></span>|<span data-ttu-id="e43a7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e43a7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e43a7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e43a7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e43a7-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="e43a7-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="e43a7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e43a7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e43a7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e43a7-115">Not supported.</span></span>|
|<span data-ttu-id="e43a7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e43a7-116">Application</span></span>|<span data-ttu-id="e43a7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e43a7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e43a7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e43a7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e43a7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e43a7-119">Request headers</span></span>
|<span data-ttu-id="e43a7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e43a7-120">Header</span></span>|<span data-ttu-id="e43a7-121">値</span><span class="sxs-lookup"><span data-stu-id="e43a7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e43a7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e43a7-122">Authorization</span></span>|<span data-ttu-id="e43a7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e43a7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e43a7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e43a7-124">Accept</span></span>|<span data-ttu-id="e43a7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e43a7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e43a7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e43a7-126">Request body</span></span>
<span data-ttu-id="e43a7-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e43a7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e43a7-128">応答</span><span class="sxs-lookup"><span data-stu-id="e43a7-128">Response</span></span>
<span data-ttu-id="e43a7-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e43a7-129">If successful, this method returns a `200 OK` response code and a collection of [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e43a7-130">例</span><span class="sxs-lookup"><span data-stu-id="e43a7-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e43a7-131">要求</span><span class="sxs-lookup"><span data-stu-id="e43a7-131">Request</span></span>
<span data-ttu-id="e43a7-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e43a7-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="e43a7-133">応答</span><span class="sxs-lookup"><span data-stu-id="e43a7-133">Response</span></span>
<span data-ttu-id="e43a7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e43a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1588

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.depEnrollmentProfile",
      "id": "3d4534f7-34f7-3d45-f734-453df734453d",
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
      "iTunesPairingMode": "allow",
      "profileRemovalDisabled": true,
      "managementCertificates": [
        {
          "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
          "thumbprint": "Thumbprint value",
          "certificate": "Certificate value"
        }
      ],
      "restoreBlocked": true,
      "restoreFromAndroidDisabled": true,
      "appleIdDisabled": true,
      "termsAndConditionsDisabled": true,
      "touchIdDisabled": true,
      "applePayDisabled": true,
      "zoomDisabled": true,
      "siriDisabled": true,
      "diagnosticsDisabled": true,
      "macOSRegistrationDisabled": true,
      "macOSFileVaultDisabled": true,
      "awaitDeviceConfiguredConfirmation": true,
      "sharedIPadMaximumUserCount": 10,
      "enableSharedIPad": true
    }
  ]
}
```





