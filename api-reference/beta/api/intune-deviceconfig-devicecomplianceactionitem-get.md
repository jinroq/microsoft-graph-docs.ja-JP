---
title: Get deviceComplianceActionItem
description: deviceComplianceActionItem オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 824fbde162998ca4749e500d836c5b4f7dd58c89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950043"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="6f2d1-103">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="6f2d1-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="6f2d1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f2d1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f2d1-106">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-106">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f2d1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6f2d1-107">Prerequisites</span></span>
<span data-ttu-id="6f2d1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f2d1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f2d1-110">Permission type</span></span>|<span data-ttu-id="6f2d1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f2d1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f2d1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f2d1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6f2d1-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f2d1-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6f2d1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f2d1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f2d1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-115">Not supported.</span></span>|
|<span data-ttu-id="6f2d1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f2d1-116">Application</span></span>|<span data-ttu-id="6f2d1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f2d1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f2d1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6f2d1-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6f2d1-119">Optional query parameters</span></span>
<span data-ttu-id="6f2d1-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6f2d1-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f2d1-121">Request headers</span></span>
|<span data-ttu-id="6f2d1-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6f2d1-122">Header</span></span>|<span data-ttu-id="6f2d1-123">値</span><span class="sxs-lookup"><span data-stu-id="6f2d1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f2d1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f2d1-124">Authorization</span></span>|<span data-ttu-id="6f2d1-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f2d1-126">承諾</span><span class="sxs-lookup"><span data-stu-id="6f2d1-126">Accept</span></span>|<span data-ttu-id="6f2d1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="6f2d1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f2d1-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f2d1-128">Request body</span></span>
<span data-ttu-id="6f2d1-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f2d1-130">応答</span><span class="sxs-lookup"><span data-stu-id="6f2d1-130">Response</span></span>
<span data-ttu-id="6f2d1-131">成功した場合、このメソッドは`200 OK`応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-131">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f2d1-132">例</span><span class="sxs-lookup"><span data-stu-id="6f2d1-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f2d1-133">要求</span><span class="sxs-lookup"><span data-stu-id="6f2d1-133">Request</span></span>
<span data-ttu-id="6f2d1-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="6f2d1-135">応答</span><span class="sxs-lookup"><span data-stu-id="6f2d1-135">Response</span></span>
<span data-ttu-id="6f2d1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6f2d1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





