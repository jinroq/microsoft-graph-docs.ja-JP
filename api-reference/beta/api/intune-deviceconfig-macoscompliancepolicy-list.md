---
title: macOSCompliancePolicies のリスト
description: macOSCompliancePolicy オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8faa8629989d074d60c493c8f9e575e81ab01a38
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338897"
---
# <a name="list-macoscompliancepolicies"></a><span data-ttu-id="a08a4-103">macOSCompliancePolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="a08a4-103">List macOSCompliancePolicies</span></span>

> <span data-ttu-id="a08a4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a08a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a08a4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a08a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a08a4-106">[macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a08a4-106">List properties and relationships of the [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a08a4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a08a4-107">Prerequisites</span></span>
<span data-ttu-id="a08a4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a08a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a08a4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a08a4-110">Permission type</span></span>|<span data-ttu-id="a08a4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a08a4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a08a4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a08a4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a08a4-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a08a4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a08a4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a08a4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a08a4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a08a4-115">Not supported.</span></span>|
|<span data-ttu-id="a08a4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a08a4-116">Application</span></span>|<span data-ttu-id="a08a4-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a08a4-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a08a4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a08a4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a08a4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a08a4-119">Request headers</span></span>
|<span data-ttu-id="a08a4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a08a4-120">Header</span></span>|<span data-ttu-id="a08a4-121">値</span><span class="sxs-lookup"><span data-stu-id="a08a4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a08a4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a08a4-122">Authorization</span></span>|<span data-ttu-id="a08a4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a08a4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a08a4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a08a4-124">Accept</span></span>|<span data-ttu-id="a08a4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a08a4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a08a4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a08a4-126">Request body</span></span>
<span data-ttu-id="a08a4-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a08a4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a08a4-128">応答</span><span class="sxs-lookup"><span data-stu-id="a08a4-128">Response</span></span>
<span data-ttu-id="a08a4-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a08a4-129">If successful, this method returns a `200 OK` response code and a collection of [macOSCompliancePolicy](../resources/intune-deviceconfig-macoscompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a08a4-130">例</span><span class="sxs-lookup"><span data-stu-id="a08a4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="a08a4-131">要求</span><span class="sxs-lookup"><span data-stu-id="a08a4-131">Request</span></span>
<span data-ttu-id="a08a4-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a08a4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="a08a4-133">応答</span><span class="sxs-lookup"><span data-stu-id="a08a4-133">Response</span></span>
<span data-ttu-id="a08a4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a08a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1408

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
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
      "osMinimumBuildVersion": "Os Minimum Build Version value",
      "osMaximumBuildVersion": "Os Maximum Build Version value",
      "systemIntegrityProtectionEnabled": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "storageRequireEncryption": true,
      "gatekeeperAllowedAppSource": "macAppStore",
      "firewallEnabled": true,
      "firewallBlockAllIncoming": true,
      "firewallEnableStealthMode": true
    }
  ]
}
```






