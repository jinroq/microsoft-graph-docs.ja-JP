---
title: deviceEnrollmentWindowsHelloForBusinessConfigurations のリスト
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 07cefeabf922b7b45ec75ee787feebb0eb9655c2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31794856"
---
# <a name="list-deviceenrollmentwindowshelloforbusinessconfigurations"></a><span data-ttu-id="95682-103">deviceEnrollmentWindowsHelloForBusinessConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="95682-103">List deviceEnrollmentWindowsHelloForBusinessConfigurations</span></span>

> <span data-ttu-id="95682-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95682-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95682-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95682-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95682-106">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="95682-106">List properties and relationships of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95682-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="95682-107">Prerequisites</span></span>
<span data-ttu-id="95682-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95682-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95682-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95682-110">Permission type</span></span>|<span data-ttu-id="95682-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95682-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95682-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95682-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95682-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="95682-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="95682-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95682-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95682-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95682-115">Not supported.</span></span>|
|<span data-ttu-id="95682-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95682-116">Application</span></span>|<span data-ttu-id="95682-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95682-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95682-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95682-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="95682-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95682-119">Request headers</span></span>
|<span data-ttu-id="95682-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95682-120">Header</span></span>|<span data-ttu-id="95682-121">値</span><span class="sxs-lookup"><span data-stu-id="95682-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95682-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95682-122">Authorization</span></span>|<span data-ttu-id="95682-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="95682-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95682-124">承諾</span><span class="sxs-lookup"><span data-stu-id="95682-124">Accept</span></span>|<span data-ttu-id="95682-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95682-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95682-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="95682-126">Request body</span></span>
<span data-ttu-id="95682-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95682-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95682-128">応答</span><span class="sxs-lookup"><span data-stu-id="95682-128">Response</span></span>
<span data-ttu-id="95682-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="95682-129">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95682-130">例</span><span class="sxs-lookup"><span data-stu-id="95682-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="95682-131">要求</span><span class="sxs-lookup"><span data-stu-id="95682-131">Request</span></span>
<span data-ttu-id="95682-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95682-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="95682-133">応答</span><span class="sxs-lookup"><span data-stu-id="95682-133">Response</span></span>
<span data-ttu-id="95682-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95682-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 914

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
      "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "pinMinimumLength": 0,
      "pinMaximumLength": 0,
      "pinUppercaseCharactersUsage": "required",
      "pinLowercaseCharactersUsage": "required",
      "pinSpecialCharactersUsage": "required",
      "state": "enabled",
      "securityDeviceRequired": true,
      "unlockWithBiometricsEnabled": true,
      "remotePassportEnabled": true,
      "pinPreviousBlockCount": 5,
      "pinExpirationInDays": 3,
      "enhancedBiometricsState": "enabled"
    }
  ]
}
```





