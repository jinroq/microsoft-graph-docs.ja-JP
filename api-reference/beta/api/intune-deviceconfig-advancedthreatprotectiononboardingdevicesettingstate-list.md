---
title: リスト advancedThreatProtectionOnboardingDeviceSettingStates
description: AdvancedThreatProtectionOnboardingDeviceSettingState オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d238b10cc9b40a6ae590617213521f067c3acc4b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854615"
---
# <a name="list-advancedthreatprotectiononboardingdevicesettingstates"></a><span data-ttu-id="da443-103">リスト advancedThreatProtectionOnboardingDeviceSettingStates</span><span class="sxs-lookup"><span data-stu-id="da443-103">List advancedThreatProtectionOnboardingDeviceSettingStates</span></span>

> <span data-ttu-id="da443-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="da443-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da443-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da443-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da443-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="da443-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da443-107">[AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="da443-107">List properties and relationships of the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da443-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="da443-108">Prerequisites</span></span>
<span data-ttu-id="da443-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da443-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da443-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da443-111">Permission type</span></span>|<span data-ttu-id="da443-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="da443-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da443-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da443-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da443-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="da443-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="da443-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da443-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da443-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da443-116">Not supported.</span></span>|
|<span data-ttu-id="da443-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da443-117">Application</span></span>|<span data-ttu-id="da443-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da443-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da443-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da443-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="da443-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da443-120">Request headers</span></span>
|<span data-ttu-id="da443-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da443-121">Header</span></span>|<span data-ttu-id="da443-122">値</span><span class="sxs-lookup"><span data-stu-id="da443-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da443-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da443-123">Authorization</span></span>|<span data-ttu-id="da443-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="da443-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da443-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da443-125">Accept</span></span>|<span data-ttu-id="da443-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da443-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da443-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="da443-127">Request body</span></span>
<span data-ttu-id="da443-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="da443-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da443-129">応答</span><span class="sxs-lookup"><span data-stu-id="da443-129">Response</span></span>
<span data-ttu-id="da443-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="da443-130">If successful, this method returns a `200 OK` response code and a collection of [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da443-131">例</span><span class="sxs-lookup"><span data-stu-id="da443-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="da443-132">要求</span><span class="sxs-lookup"><span data-stu-id="da443-132">Request</span></span>
<span data-ttu-id="da443-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da443-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

### <a name="response"></a><span data-ttu-id="da443-134">応答</span><span class="sxs-lookup"><span data-stu-id="da443-134">Response</span></span>
<span data-ttu-id="da443-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="da443-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 711

{
  "value": [
    {
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
  ]
}
```





