---
title: depIOSEnrollmentProfile を取得する
description: depIOSEnrollmentProfile オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c685e06a24a0cd155dd5948018ffb3dd745d93e0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987042"
---
# <a name="get-depiosenrollmentprofile"></a><span data-ttu-id="17acf-103">depIOSEnrollmentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="17acf-103">Get depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="17acf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17acf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17acf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="17acf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17acf-106">[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="17acf-106">Read properties and relationships of the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="17acf-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="17acf-107">Prerequisites</span></span>
<span data-ttu-id="17acf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17acf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17acf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="17acf-110">Permission type</span></span>|<span data-ttu-id="17acf-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="17acf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="17acf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="17acf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="17acf-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="17acf-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="17acf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="17acf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="17acf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17acf-115">Not supported.</span></span>|
|<span data-ttu-id="17acf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="17acf-116">Application</span></span>|<span data-ttu-id="17acf-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17acf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="17acf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="17acf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="optional-query-parameters"></a><span data-ttu-id="17acf-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="17acf-119">Optional query parameters</span></span>
<span data-ttu-id="17acf-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="17acf-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="17acf-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17acf-121">Request headers</span></span>
|<span data-ttu-id="17acf-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17acf-122">Header</span></span>|<span data-ttu-id="17acf-123">値</span><span class="sxs-lookup"><span data-stu-id="17acf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="17acf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="17acf-124">Authorization</span></span>|<span data-ttu-id="17acf-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="17acf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="17acf-126">承諾</span><span class="sxs-lookup"><span data-stu-id="17acf-126">Accept</span></span>|<span data-ttu-id="17acf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="17acf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17acf-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="17acf-128">Request body</span></span>
<span data-ttu-id="17acf-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="17acf-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17acf-130">応答</span><span class="sxs-lookup"><span data-stu-id="17acf-130">Response</span></span>
<span data-ttu-id="17acf-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="17acf-131">If successful, this method returns a `200 OK` response code and [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17acf-132">例</span><span class="sxs-lookup"><span data-stu-id="17acf-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="17acf-133">要求</span><span class="sxs-lookup"><span data-stu-id="17acf-133">Request</span></span>
<span data-ttu-id="17acf-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="17acf-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="17acf-135">応答</span><span class="sxs-lookup"><span data-stu-id="17acf-135">Response</span></span>
<span data-ttu-id="17acf-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="17acf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1898

{
  "value": {
    "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
    "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
    "iTunesPairingMode": "allow",
    "managementCertificates": [
      {
        "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
        "thumbprint": "Thumbprint value",
        "certificate": "Certificate value"
      }
    ],
    "restoreFromAndroidDisabled": true,
    "awaitDeviceConfiguredConfirmation": true,
    "sharedIPadMaximumUserCount": 10,
    "enableSharedIPad": true,
    "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
    "enableSingleAppEnrollmentMode": true,
    "homeButtonScreenDisabled": true,
    "iMessageAndFaceTimeScreenDisabled": true,
    "onBoardingScreenDisabled": true,
    "screenTimeScreenDisabled": true,
    "simSetupScreenDisabled": true,
    "softwareUpdateScreenDisabled": true,
    "watchMigrationScreenDisabled": true
  }
}
```




