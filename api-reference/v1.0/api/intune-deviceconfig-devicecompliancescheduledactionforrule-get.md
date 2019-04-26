---
title: Get deviceComplianceScheduledActionForRule
description: deviceComplianceScheduledActionForRule オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1317927a45310400bd9fa464a56ac7df968d2e59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580877"
---
# <a name="get-devicecompliancescheduledactionforrule"></a><span data-ttu-id="596dd-103">Get deviceComplianceScheduledActionForRule</span><span class="sxs-lookup"><span data-stu-id="596dd-103">Get deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="596dd-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="596dd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="596dd-105">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="596dd-105">Read properties and relationships of the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="596dd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="596dd-106">Prerequisites</span></span>
<span data-ttu-id="596dd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="596dd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="596dd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="596dd-109">Permission type</span></span>|<span data-ttu-id="596dd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="596dd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="596dd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="596dd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="596dd-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="596dd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="596dd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="596dd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="596dd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="596dd-114">Not supported.</span></span>|
|<span data-ttu-id="596dd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="596dd-115">Application</span></span>|<span data-ttu-id="596dd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="596dd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="596dd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="596dd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="596dd-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="596dd-118">Optional query parameters</span></span>
<span data-ttu-id="596dd-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="596dd-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="596dd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="596dd-120">Request headers</span></span>
|<span data-ttu-id="596dd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="596dd-121">Header</span></span>|<span data-ttu-id="596dd-122">値</span><span class="sxs-lookup"><span data-stu-id="596dd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="596dd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="596dd-123">Authorization</span></span>|<span data-ttu-id="596dd-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="596dd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="596dd-125">承諾</span><span class="sxs-lookup"><span data-stu-id="596dd-125">Accept</span></span>|<span data-ttu-id="596dd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="596dd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="596dd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="596dd-127">Request body</span></span>
<span data-ttu-id="596dd-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="596dd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="596dd-129">応答</span><span class="sxs-lookup"><span data-stu-id="596dd-129">Response</span></span>
<span data-ttu-id="596dd-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="596dd-130">If successful, this method returns a `200 OK` response code and [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="596dd-131">例</span><span class="sxs-lookup"><span data-stu-id="596dd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="596dd-132">要求</span><span class="sxs-lookup"><span data-stu-id="596dd-132">Request</span></span>
<span data-ttu-id="596dd-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="596dd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

### <a name="response"></a><span data-ttu-id="596dd-134">応答</span><span class="sxs-lookup"><span data-stu-id="596dd-134">Response</span></span>
<span data-ttu-id="596dd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="596dd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 188

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
    "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
    "ruleName": "Rule Name value"
  }
}
```



