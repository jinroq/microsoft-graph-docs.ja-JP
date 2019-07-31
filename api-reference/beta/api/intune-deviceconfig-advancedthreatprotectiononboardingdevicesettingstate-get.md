---
title: AdvancedThreatProtectionOnboardingDeviceSettingState を取得する
description: AdvancedThreatProtectionOnboardingDeviceSettingState オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e3a41906bf812cc9a133f9b0ba19a9bb3b6674e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958415"
---
# <a name="get-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="33217-103">AdvancedThreatProtectionOnboardingDeviceSettingState を取得する</span><span class="sxs-lookup"><span data-stu-id="33217-103">Get advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="33217-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33217-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="33217-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="33217-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33217-106">[AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="33217-106">Read properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="33217-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="33217-107">Prerequisites</span></span>
<span data-ttu-id="33217-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33217-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33217-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33217-110">Permission type</span></span>|<span data-ttu-id="33217-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="33217-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33217-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33217-112">Delegated (work or school account)</span></span>|<span data-ttu-id="33217-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="33217-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="33217-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33217-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33217-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33217-115">Not supported.</span></span>|
|<span data-ttu-id="33217-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33217-116">Application</span></span>|<span data-ttu-id="33217-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33217-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33217-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33217-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33217-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="33217-119">Optional query parameters</span></span>
<span data-ttu-id="33217-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="33217-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33217-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33217-121">Request headers</span></span>
|<span data-ttu-id="33217-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33217-122">Header</span></span>|<span data-ttu-id="33217-123">値</span><span class="sxs-lookup"><span data-stu-id="33217-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33217-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="33217-124">Authorization</span></span>|<span data-ttu-id="33217-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="33217-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33217-126">承諾</span><span class="sxs-lookup"><span data-stu-id="33217-126">Accept</span></span>|<span data-ttu-id="33217-127">application/json</span><span class="sxs-lookup"><span data-stu-id="33217-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33217-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="33217-128">Request body</span></span>
<span data-ttu-id="33217-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="33217-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33217-130">応答</span><span class="sxs-lookup"><span data-stu-id="33217-130">Response</span></span>
<span data-ttu-id="33217-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="33217-131">If successful, this method returns a `200 OK` response code and [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33217-132">例</span><span class="sxs-lookup"><span data-stu-id="33217-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="33217-133">要求</span><span class="sxs-lookup"><span data-stu-id="33217-133">Request</span></span>
<span data-ttu-id="33217-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33217-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="33217-135">応答</span><span class="sxs-lookup"><span data-stu-id="33217-135">Response</span></span>
<span data-ttu-id="33217-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="33217-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 669

{
  "value": {
    "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
    "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
    "platformType": "windowsRT",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "deviceId": "Device Id value",
    "deviceName": "Device Name value",
    "userId": "User Id value",
    "userEmail": "User Email value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "deviceModel": "Device Model value",
    "state": "notApplicable",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
  }
}
```





