---
title: iosCompliancePolicies のリスト
description: iosCompliancePolicy オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 959947928959efc8f9c8b8f0641d92a6d7a28719
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017344"
---
# <a name="list-ioscompliancepolicies"></a><span data-ttu-id="6330f-103">iosCompliancePolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="6330f-103">List iosCompliancePolicies</span></span>

> <span data-ttu-id="6330f-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6330f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6330f-105">[iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6330f-105">List properties and relationships of the [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6330f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6330f-106">Prerequisites</span></span>
<span data-ttu-id="6330f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6330f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6330f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6330f-109">Permission type</span></span>|<span data-ttu-id="6330f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6330f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6330f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6330f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6330f-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6330f-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6330f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6330f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6330f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6330f-114">Not supported.</span></span>|
|<span data-ttu-id="6330f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6330f-115">Application</span></span>|<span data-ttu-id="6330f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6330f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6330f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6330f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6330f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6330f-118">Request headers</span></span>
|<span data-ttu-id="6330f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6330f-119">Header</span></span>|<span data-ttu-id="6330f-120">値</span><span class="sxs-lookup"><span data-stu-id="6330f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6330f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6330f-121">Authorization</span></span>|<span data-ttu-id="6330f-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6330f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6330f-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6330f-123">Accept</span></span>|<span data-ttu-id="6330f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6330f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6330f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6330f-125">Request body</span></span>
<span data-ttu-id="6330f-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6330f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6330f-127">応答</span><span class="sxs-lookup"><span data-stu-id="6330f-127">Response</span></span>
<span data-ttu-id="6330f-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6330f-128">If successful, this method returns a `200 OK` response code and a collection of [iosCompliancePolicy](../resources/intune-deviceconfig-ioscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6330f-129">例</span><span class="sxs-lookup"><span data-stu-id="6330f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6330f-130">要求</span><span class="sxs-lookup"><span data-stu-id="6330f-130">Request</span></span>
<span data-ttu-id="6330f-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6330f-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="6330f-132">応答</span><span class="sxs-lookup"><span data-stu-id="6330f-132">Response</span></span>
<span data-ttu-id="6330f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6330f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1034

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosCompliancePolicy",
      "id": "4f501351-1351-4f50-5113-504f5113504f",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passcodeBlockSimple": true,
      "passcodeExpirationDays": 6,
      "passcodeMinimumLength": 5,
      "passcodeMinutesOfInactivityBeforeLock": 5,
      "passcodePreviousPasscodeBlockCount": 2,
      "passcodeMinimumCharacterSetCount": 0,
      "passcodeRequiredType": "alphanumeric",
      "passcodeRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "securityBlockJailbrokenDevices": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "managedEmailProfileRequired": true
    }
  ]
}
```



