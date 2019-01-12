---
title: Get windows10MobileCompliancePolicy
description: windows10MobileCompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d5542505906cc5d5e4599e0cb73c0df7f6445b62
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946470"
---
# <a name="get-windows10mobilecompliancepolicy"></a><span data-ttu-id="c7121-103">Get windows10MobileCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c7121-103">Get windows10MobileCompliancePolicy</span></span>

> <span data-ttu-id="c7121-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c7121-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c7121-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7121-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c7121-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7121-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c7121-107">[windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c7121-107">Read properties and relationships of the [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c7121-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c7121-108">Prerequisites</span></span>
<span data-ttu-id="c7121-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7121-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7121-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7121-111">Permission type</span></span>|<span data-ttu-id="c7121-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7121-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7121-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7121-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c7121-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7121-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c7121-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7121-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7121-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7121-116">Not supported.</span></span>|
|<span data-ttu-id="c7121-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7121-117">Application</span></span>|<span data-ttu-id="c7121-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7121-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7121-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7121-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7121-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c7121-120">Optional query parameters</span></span>
<span data-ttu-id="c7121-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c7121-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c7121-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7121-122">Request headers</span></span>
|<span data-ttu-id="c7121-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7121-123">Header</span></span>|<span data-ttu-id="c7121-124">値</span><span class="sxs-lookup"><span data-stu-id="c7121-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7121-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7121-125">Authorization</span></span>|<span data-ttu-id="c7121-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c7121-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7121-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c7121-127">Accept</span></span>|<span data-ttu-id="c7121-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c7121-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7121-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7121-129">Request body</span></span>
<span data-ttu-id="c7121-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c7121-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7121-131">応答</span><span class="sxs-lookup"><span data-stu-id="c7121-131">Response</span></span>
<span data-ttu-id="c7121-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c7121-132">If successful, this method returns a `200 OK` response code and [windows10MobileCompliancePolicy](../resources/intune-deviceconfig-windows10mobilecompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7121-133">例</span><span class="sxs-lookup"><span data-stu-id="c7121-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c7121-134">要求</span><span class="sxs-lookup"><span data-stu-id="c7121-134">Request</span></span>
<span data-ttu-id="c7121-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c7121-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="c7121-136">応答</span><span class="sxs-lookup"><span data-stu-id="c7121-136">Response</span></span>
<span data-ttu-id="c7121-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c7121-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





