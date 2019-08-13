---
title: DepEnrollmentBaseProfile を取得する
description: DepEnrollmentBaseProfile オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 261717ffc78c3dbe731a15961c4d4f8c0d120ff2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348327"
---
# <a name="get-depenrollmentbaseprofile"></a><span data-ttu-id="d4895-103">DepEnrollmentBaseProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="d4895-103">Get depEnrollmentBaseProfile</span></span>

> <span data-ttu-id="d4895-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4895-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4895-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4895-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4895-106">[DepEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d4895-106">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4895-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4895-107">Prerequisites</span></span>
<span data-ttu-id="d4895-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4895-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4895-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4895-110">Permission type</span></span>|<span data-ttu-id="d4895-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4895-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4895-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4895-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4895-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4895-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d4895-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4895-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4895-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4895-115">Not supported.</span></span>|
|<span data-ttu-id="d4895-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4895-116">Application</span></span>|<span data-ttu-id="d4895-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4895-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4895-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4895-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d4895-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d4895-119">Optional query parameters</span></span>
<span data-ttu-id="d4895-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d4895-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4895-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4895-121">Request headers</span></span>
|<span data-ttu-id="d4895-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4895-122">Header</span></span>|<span data-ttu-id="d4895-123">値</span><span class="sxs-lookup"><span data-stu-id="d4895-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4895-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4895-124">Authorization</span></span>|<span data-ttu-id="d4895-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4895-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4895-126">承諾</span><span class="sxs-lookup"><span data-stu-id="d4895-126">Accept</span></span>|<span data-ttu-id="d4895-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d4895-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4895-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4895-128">Request body</span></span>
<span data-ttu-id="d4895-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d4895-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4895-130">応答</span><span class="sxs-lookup"><span data-stu-id="d4895-130">Response</span></span>
<span data-ttu-id="d4895-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d4895-131">If successful, this method returns a `200 OK` response code and [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4895-132">例</span><span class="sxs-lookup"><span data-stu-id="d4895-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4895-133">要求</span><span class="sxs-lookup"><span data-stu-id="d4895-133">Request</span></span>
<span data-ttu-id="d4895-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4895-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="d4895-135">応答</span><span class="sxs-lookup"><span data-stu-id="d4895-135">Response</span></span>
<span data-ttu-id="d4895-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4895-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1136

{
  "value": {
    "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
    "id": "db378868-8868-db37-6888-37db688837db",
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
    "deviceNameTemplate": "Device Name Template value"
  }
}
```






