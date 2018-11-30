---
title: macOSCompliancePolicies のリスト
description: macOSCompliancePolicy オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 70ef7d53822953c7469490f9e23873b4b2219c39
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023172"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="4eed8-103">macOSCompliancePolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="4eed8-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="4eed8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4eed8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4eed8-105">[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4eed8-105">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4eed8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4eed8-106">Prerequisites</span></span>
<span data-ttu-id="4eed8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4eed8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4eed8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4eed8-109">Permission type</span></span>|<span data-ttu-id="4eed8-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4eed8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eed8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4eed8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4eed8-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4eed8-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4eed8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4eed8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eed8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4eed8-114">Not supported.</span></span>|
|<span data-ttu-id="4eed8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4eed8-115">Application</span></span>|<span data-ttu-id="4eed8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4eed8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eed8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4eed8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="4eed8-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4eed8-118">Request headers</span></span>
|<span data-ttu-id="4eed8-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4eed8-119">Header</span></span>|<span data-ttu-id="4eed8-120">値</span><span class="sxs-lookup"><span data-stu-id="4eed8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eed8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eed8-121">Authorization</span></span>|<span data-ttu-id="4eed8-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4eed8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eed8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4eed8-123">Accept</span></span>|<span data-ttu-id="4eed8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4eed8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eed8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4eed8-125">Request body</span></span>
<span data-ttu-id="4eed8-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4eed8-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4eed8-127">応答</span><span class="sxs-lookup"><span data-stu-id="4eed8-127">Response</span></span>
<span data-ttu-id="4eed8-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4eed8-128">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eed8-129">例</span><span class="sxs-lookup"><span data-stu-id="4eed8-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4eed8-130">要求</span><span class="sxs-lookup"><span data-stu-id="4eed8-130">Request</span></span>
<span data-ttu-id="4eed8-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4eed8-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="4eed8-132">応答</span><span class="sxs-lookup"><span data-stu-id="4eed8-132">Response</span></span>
<span data-ttu-id="4eed8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4eed8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1150

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
      "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "systemIntegrityProtectionEnabled": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "storageRequireEncryption": true,
      "firewallEnabled": true,
      "firewallBlockAllIncoming": true,
      "firewallEnableStealthMode": true
    }
  ]
}
```



