---
title: windowsPhone81CompliancePolicies のリスト
description: windowsPhone81CompliancePolicy オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52a05f8fe8fc495364c4542a1c45e0269afa4650
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162686"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="96f91-103">windowsPhone81CompliancePolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="96f91-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="96f91-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96f91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96f91-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96f91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96f91-106">[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="96f91-106">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96f91-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="96f91-107">Prerequisites</span></span>
<span data-ttu-id="96f91-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96f91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="96f91-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96f91-110">Permission type</span></span>|<span data-ttu-id="96f91-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="96f91-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96f91-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96f91-112">Delegated (work or school account)</span></span>|<span data-ttu-id="96f91-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96f91-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="96f91-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96f91-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96f91-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96f91-115">Not supported.</span></span>|
|<span data-ttu-id="96f91-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96f91-116">Application</span></span>|<span data-ttu-id="96f91-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96f91-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96f91-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96f91-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="96f91-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96f91-119">Request headers</span></span>
|<span data-ttu-id="96f91-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96f91-120">Header</span></span>|<span data-ttu-id="96f91-121">値</span><span class="sxs-lookup"><span data-stu-id="96f91-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96f91-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="96f91-122">Authorization</span></span>|<span data-ttu-id="96f91-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="96f91-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96f91-124">承諾</span><span class="sxs-lookup"><span data-stu-id="96f91-124">Accept</span></span>|<span data-ttu-id="96f91-125">application/json</span><span class="sxs-lookup"><span data-stu-id="96f91-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96f91-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="96f91-126">Request body</span></span>
<span data-ttu-id="96f91-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="96f91-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96f91-128">応答</span><span class="sxs-lookup"><span data-stu-id="96f91-128">Response</span></span>
<span data-ttu-id="96f91-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="96f91-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96f91-130">例</span><span class="sxs-lookup"><span data-stu-id="96f91-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="96f91-131">要求</span><span class="sxs-lookup"><span data-stu-id="96f91-131">Request</span></span>
<span data-ttu-id="96f91-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96f91-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="96f91-133">応答</span><span class="sxs-lookup"><span data-stu-id="96f91-133">Response</span></span>
<span data-ttu-id="96f91-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="96f91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 958

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordMinimumCharacterSetCount": 0,
      "passwordRequiredType": "alphanumeric",
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "storageRequireEncryption": true
    }
  ]
}
```




