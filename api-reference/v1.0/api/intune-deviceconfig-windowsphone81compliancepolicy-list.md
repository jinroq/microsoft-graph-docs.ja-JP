---
title: windowsPhone81CompliancePolicies のリスト
description: windowsPhone81CompliancePolicy オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: c29426788d8ad045b31364de55880a24c47f6eed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332754"
---
# <a name="list-windowsphone81compliancepolicies"></a><span data-ttu-id="3d57d-103">windowsPhone81CompliancePolicies のリスト</span><span class="sxs-lookup"><span data-stu-id="3d57d-103">List windowsPhone81CompliancePolicies</span></span>

> <span data-ttu-id="3d57d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d57d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d57d-105">[windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3d57d-105">List properties and relationships of the [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3d57d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3d57d-106">Prerequisites</span></span>
<span data-ttu-id="3d57d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d57d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d57d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d57d-109">Permission type</span></span>|<span data-ttu-id="3d57d-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d57d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d57d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d57d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3d57d-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d57d-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="3d57d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d57d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d57d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d57d-114">Not supported.</span></span>|
|<span data-ttu-id="3d57d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d57d-115">Application</span></span>|<span data-ttu-id="3d57d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d57d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d57d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d57d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3d57d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d57d-118">Request headers</span></span>
|<span data-ttu-id="3d57d-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d57d-119">Header</span></span>|<span data-ttu-id="3d57d-120">値</span><span class="sxs-lookup"><span data-stu-id="3d57d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d57d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d57d-121">Authorization</span></span>|<span data-ttu-id="3d57d-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3d57d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d57d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="3d57d-123">Accept</span></span>|<span data-ttu-id="3d57d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3d57d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d57d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d57d-125">Request body</span></span>
<span data-ttu-id="3d57d-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3d57d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d57d-127">応答</span><span class="sxs-lookup"><span data-stu-id="3d57d-127">Response</span></span>
<span data-ttu-id="3d57d-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="3d57d-128">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81CompliancePolicy](../resources/intune-deviceconfig-windowsphone81compliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d57d-129">例</span><span class="sxs-lookup"><span data-stu-id="3d57d-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="3d57d-130">要求</span><span class="sxs-lookup"><span data-stu-id="3d57d-130">Request</span></span>
<span data-ttu-id="3d57d-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3d57d-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="3d57d-132">応答</span><span class="sxs-lookup"><span data-stu-id="3d57d-132">Response</span></span>
<span data-ttu-id="3d57d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3d57d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 884

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
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



