---
title: Get deviceComplianceActionItem
description: deviceComplianceActionItem オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe8b9022b0e3f2121dd7059664b704e76489afd1
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968512"
---
# <a name="get-devicecomplianceactionitem"></a><span data-ttu-id="88fa7-103">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="88fa7-103">Get deviceComplianceActionItem</span></span>

> <span data-ttu-id="88fa7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88fa7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88fa7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88fa7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88fa7-106">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="88fa7-106">Read properties and relationships of the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88fa7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="88fa7-107">Prerequisites</span></span>
<span data-ttu-id="88fa7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88fa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88fa7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="88fa7-110">Permission type</span></span>|<span data-ttu-id="88fa7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="88fa7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88fa7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88fa7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="88fa7-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88fa7-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="88fa7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88fa7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88fa7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88fa7-115">Not supported.</span></span>|
|<span data-ttu-id="88fa7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88fa7-116">Application</span></span>|<span data-ttu-id="88fa7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88fa7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88fa7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88fa7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="88fa7-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="88fa7-119">Optional query parameters</span></span>
<span data-ttu-id="88fa7-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="88fa7-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="88fa7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88fa7-121">Request headers</span></span>
|<span data-ttu-id="88fa7-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88fa7-122">Header</span></span>|<span data-ttu-id="88fa7-123">値</span><span class="sxs-lookup"><span data-stu-id="88fa7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88fa7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="88fa7-124">Authorization</span></span>|<span data-ttu-id="88fa7-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="88fa7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88fa7-126">承諾</span><span class="sxs-lookup"><span data-stu-id="88fa7-126">Accept</span></span>|<span data-ttu-id="88fa7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="88fa7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88fa7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="88fa7-128">Request body</span></span>
<span data-ttu-id="88fa7-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="88fa7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88fa7-130">応答</span><span class="sxs-lookup"><span data-stu-id="88fa7-130">Response</span></span>
<span data-ttu-id="88fa7-131">成功した場合、このメソッドは`200 OK`応答コードと、応答本文で [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="88fa7-131">If successful, this method returns a `200 OK` response code and [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88fa7-132">例</span><span class="sxs-lookup"><span data-stu-id="88fa7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="88fa7-133">要求</span><span class="sxs-lookup"><span data-stu-id="88fa7-133">Request</span></span>
<span data-ttu-id="88fa7-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="88fa7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="88fa7-135">応答</span><span class="sxs-lookup"><span data-stu-id="88fa7-135">Response</span></span>
<span data-ttu-id="88fa7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="88fa7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




