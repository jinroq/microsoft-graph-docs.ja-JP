---
title: deviceComplianceActionItems のリスト
description: deviceComplianceActionItem オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d9b5d154e345dd71a3fb9e34085c18b22f3ff46
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952259"
---
# <a name="list-devicecomplianceactionitems"></a><span data-ttu-id="d0a99-103">deviceComplianceActionItems のリスト</span><span class="sxs-lookup"><span data-stu-id="d0a99-103">List deviceComplianceActionItems</span></span>

> <span data-ttu-id="d0a99-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0a99-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0a99-105">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d0a99-105">List properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0a99-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d0a99-106">Prerequisites</span></span>
<span data-ttu-id="d0a99-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0a99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0a99-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0a99-109">Permission type</span></span>|<span data-ttu-id="d0a99-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0a99-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0a99-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0a99-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0a99-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0a99-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d0a99-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0a99-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0a99-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0a99-114">Not supported.</span></span>|
|<span data-ttu-id="d0a99-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0a99-115">Application</span></span>|<span data-ttu-id="d0a99-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0a99-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0a99-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0a99-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0a99-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0a99-118">Request headers</span></span>
|<span data-ttu-id="d0a99-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0a99-119">Header</span></span>|<span data-ttu-id="d0a99-120">値</span><span class="sxs-lookup"><span data-stu-id="d0a99-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0a99-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0a99-121">Authorization</span></span>|<span data-ttu-id="d0a99-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d0a99-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0a99-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d0a99-123">Accept</span></span>|<span data-ttu-id="d0a99-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d0a99-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0a99-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0a99-125">Request body</span></span>
<span data-ttu-id="d0a99-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d0a99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0a99-127">応答</span><span class="sxs-lookup"><span data-stu-id="d0a99-127">Response</span></span>
<span data-ttu-id="d0a99-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="d0a99-128">If successful, this method returns a `200 OK` response code and a collection of [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0a99-129">例</span><span class="sxs-lookup"><span data-stu-id="d0a99-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0a99-130">要求</span><span class="sxs-lookup"><span data-stu-id="d0a99-130">Request</span></span>
<span data-ttu-id="d0a99-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d0a99-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

### <a name="response"></a><span data-ttu-id="d0a99-132">応答</span><span class="sxs-lookup"><span data-stu-id="d0a99-132">Response</span></span>
<span data-ttu-id="d0a99-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d0a99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
      "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
      "gracePeriodHours": 0,
      "actionType": "notification",
      "notificationTemplateId": "Notification Template Id value",
      "notificationMessageCCList": [
        "Notification Message CCList value"
      ]
    }
  ]
}
```



