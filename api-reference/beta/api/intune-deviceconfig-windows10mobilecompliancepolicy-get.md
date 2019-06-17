---
title: Get windows10MobileCompliancePolicy
description: windows10MobileCompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fe8ce01c5300c63b7bf43002b7dac22b9febaa5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962534"
---
# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="725fa-103">Get windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="725fa-103">Get windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="725fa-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="725fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="725fa-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="725fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="725fa-106">[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="725fa-106">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="725fa-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="725fa-107">Prerequisites</span></span>
<span data-ttu-id="725fa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="725fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="725fa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="725fa-110">Permission type</span></span>|<span data-ttu-id="725fa-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="725fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="725fa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="725fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="725fa-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="725fa-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="725fa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="725fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="725fa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="725fa-115">Not supported.</span></span>|
|<span data-ttu-id="725fa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="725fa-116">Application</span></span>|<span data-ttu-id="725fa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="725fa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="725fa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="725fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="725fa-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="725fa-119">Optional query parameters</span></span>
<span data-ttu-id="725fa-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="725fa-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="725fa-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="725fa-121">Request headers</span></span>
|<span data-ttu-id="725fa-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="725fa-122">Header</span></span>|<span data-ttu-id="725fa-123">値</span><span class="sxs-lookup"><span data-stu-id="725fa-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="725fa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="725fa-124">Authorization</span></span>|<span data-ttu-id="725fa-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="725fa-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="725fa-126">承諾</span><span class="sxs-lookup"><span data-stu-id="725fa-126">Accept</span></span>|<span data-ttu-id="725fa-127">application/json</span><span class="sxs-lookup"><span data-stu-id="725fa-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="725fa-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="725fa-128">Request body</span></span>
<span data-ttu-id="725fa-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="725fa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="725fa-130">応答</span><span class="sxs-lookup"><span data-stu-id="725fa-130">Response</span></span>
<span data-ttu-id="725fa-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="725fa-131">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="725fa-132">例</span><span class="sxs-lookup"><span data-stu-id="725fa-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="725fa-133">要求</span><span class="sxs-lookup"><span data-stu-id="725fa-133">Request</span></span>
<span data-ttu-id="725fa-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="725fa-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="725fa-135">応答</span><span class="sxs-lookup"><span data-stu-id="725fa-135">Response</span></span>
<span data-ttu-id="725fa-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="725fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1419

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10MobileCompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "3d4237b0-37b0-3d42-b037-423db037423d",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordMinimumLength": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "passwordExpirationDays": 6,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordRequireToUnlockFromIdle": true,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "earlyLaunchAntiMalwareDriverEnabled": true,
    "bitLockerEnabled": true,
    "secureBootEnabled": true,
    "codeIntegrityEnabled": true,
    "storageRequireEncryption": true,
    "activeFirewallRequired": true,
    "validOperatingSystemBuildRanges": [
      {
        "@odata.type": "microsoft.graph.operatingSystemVersionRange",
        "description": "Description value",
        "lowestVersion": "Lowest Version value",
        "highestVersion": "Highest Version value"
      }
    ]
  }
}
```





