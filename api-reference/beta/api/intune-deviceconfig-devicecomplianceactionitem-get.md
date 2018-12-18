---
title: Get deviceComplianceActionItem
description: deviceComplianceActionItem オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 2fd6762ca3f0d7128721eb240d7d00bcf1291da4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307953"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="dffdc-103">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="dffdc-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="dffdc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dffdc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dffdc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dffdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dffdc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dffdc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dffdc-107">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dffdc-107">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dffdc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="dffdc-108">Prerequisites</span></span>
<span data-ttu-id="dffdc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dffdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dffdc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dffdc-111">Permission type</span></span>|<span data-ttu-id="dffdc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dffdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dffdc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dffdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dffdc-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dffdc-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dffdc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dffdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dffdc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dffdc-116">Not supported.</span></span>|
|<span data-ttu-id="dffdc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dffdc-117">Application</span></span>|<span data-ttu-id="dffdc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dffdc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dffdc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dffdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dffdc-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dffdc-120">Optional query parameters</span></span>
<span data-ttu-id="dffdc-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dffdc-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="dffdc-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dffdc-122">Request headers</span></span>
|<span data-ttu-id="dffdc-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dffdc-123">Header</span></span>|<span data-ttu-id="dffdc-124">値</span><span class="sxs-lookup"><span data-stu-id="dffdc-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dffdc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="dffdc-125">Authorization</span></span>|<span data-ttu-id="dffdc-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dffdc-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dffdc-127">Accept</span><span class="sxs-lookup"><span data-stu-id="dffdc-127">Accept</span></span>|<span data-ttu-id="dffdc-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dffdc-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dffdc-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="dffdc-129">Request body</span></span>
<span data-ttu-id="dffdc-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dffdc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dffdc-131">応答</span><span class="sxs-lookup"><span data-stu-id="dffdc-131">Response</span></span>
<span data-ttu-id="dffdc-132">成功した場合、このメソッドは`200 OK`応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dffdc-132">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dffdc-133">例</span><span class="sxs-lookup"><span data-stu-id="dffdc-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="dffdc-134">要求</span><span class="sxs-lookup"><span data-stu-id="dffdc-134">Request</span></span>
<span data-ttu-id="dffdc-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dffdc-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="dffdc-136">応答</span><span class="sxs-lookup"><span data-stu-id="dffdc-136">Response</span></span>
<span data-ttu-id="dffdc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dffdc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
    "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
    "gracePeriodHours": 0,
    "actionType": "notification",
    "notificationTemplateId": "Notification Template Id value",
    "notificationMessageCCList": [
      "Notification Message CCList value"
    ]
  }
}
```





