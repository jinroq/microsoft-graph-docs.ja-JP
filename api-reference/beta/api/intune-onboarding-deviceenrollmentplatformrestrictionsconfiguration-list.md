---
title: deviceEnrollmentPlatformRestrictionsConfigurations のリスト
description: deviceEnrollmentPlatformRestrictionsConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4525cbb108cf6325aad28bd6298c0e5a24d6a764
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352925"
---
# <a name="list-deviceenrollmentplatformrestrictionsconfigurations"></a><span data-ttu-id="71290-103">deviceEnrollmentPlatformRestrictionsConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="71290-103">List deviceEnrollmentPlatformRestrictionsConfigurations</span></span>

> <span data-ttu-id="71290-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71290-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71290-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="71290-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71290-106">[deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="71290-106">List properties and relationships of the [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71290-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="71290-107">Prerequisites</span></span>
<span data-ttu-id="71290-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="71290-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71290-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="71290-110">Permission type</span></span>|<span data-ttu-id="71290-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="71290-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71290-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="71290-112">Delegated (work or school account)</span></span>|<span data-ttu-id="71290-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="71290-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="71290-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="71290-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71290-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="71290-115">Not supported.</span></span>|
|<span data-ttu-id="71290-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="71290-116">Application</span></span>|<span data-ttu-id="71290-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="71290-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="71290-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="71290-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="71290-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71290-119">Request headers</span></span>
|<span data-ttu-id="71290-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="71290-120">Header</span></span>|<span data-ttu-id="71290-121">値</span><span class="sxs-lookup"><span data-stu-id="71290-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71290-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71290-122">Authorization</span></span>|<span data-ttu-id="71290-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="71290-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71290-124">承諾</span><span class="sxs-lookup"><span data-stu-id="71290-124">Accept</span></span>|<span data-ttu-id="71290-125">application/json</span><span class="sxs-lookup"><span data-stu-id="71290-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71290-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="71290-126">Request body</span></span>
<span data-ttu-id="71290-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="71290-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71290-128">応答</span><span class="sxs-lookup"><span data-stu-id="71290-128">Response</span></span>
<span data-ttu-id="71290-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="71290-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentPlatformRestrictionsConfiguration](../resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71290-130">例</span><span class="sxs-lookup"><span data-stu-id="71290-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="71290-131">要求</span><span class="sxs-lookup"><span data-stu-id="71290-131">Request</span></span>
<span data-ttu-id="71290-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="71290-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="71290-133">応答</span><span class="sxs-lookup"><span data-stu-id="71290-133">Response</span></span>
<span data-ttu-id="71290-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="71290-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2664

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestrictionsConfiguration",
      "id": "3acb2d75-2d75-3acb-752d-cb3a752dcb3a",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "iosRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "windowsRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "windowsMobileRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "androidRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "androidForWorkRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "macRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      },
      "macOSRestriction": {
        "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction",
        "platformBlocked": true,
        "personalDeviceEnrollmentBlocked": true,
        "osMinimumVersion": "Os Minimum Version value",
        "osMaximumVersion": "Os Maximum Version value"
      }
    }
  ]
}
```






