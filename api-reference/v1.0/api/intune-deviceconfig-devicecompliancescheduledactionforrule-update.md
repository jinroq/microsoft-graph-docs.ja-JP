---
title: deviceComplianceScheduledActionForRule の更新
description: deviceComplianceScheduledActionForRule オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: e63602cf39aa89bfdcda2db900d993d8e0a56d9d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301660"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="9e2cc-103">deviceComplianceScheduledActionForRule の更新</span><span class="sxs-lookup"><span data-stu-id="9e2cc-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="9e2cc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e2cc-105">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e2cc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e2cc-106">Prerequisites</span></span>
<span data-ttu-id="9e2cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e2cc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e2cc-109">Permission type</span></span>|<span data-ttu-id="9e2cc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e2cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e2cc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e2cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9e2cc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e2cc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e2cc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e2cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e2cc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-114">Not supported.</span></span>|
|<span data-ttu-id="9e2cc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e2cc-115">Application</span></span>|<span data-ttu-id="9e2cc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e2cc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e2cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="9e2cc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e2cc-118">Request headers</span></span>
|<span data-ttu-id="9e2cc-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e2cc-119">Header</span></span>|<span data-ttu-id="9e2cc-120">値</span><span class="sxs-lookup"><span data-stu-id="9e2cc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e2cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e2cc-121">Authorization</span></span>|<span data-ttu-id="9e2cc-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e2cc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9e2cc-123">Accept</span></span>|<span data-ttu-id="9e2cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9e2cc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e2cc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e2cc-125">Request body</span></span>
<span data-ttu-id="9e2cc-126">要求本文で、[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="9e2cc-127">次の表に、[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="9e2cc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e2cc-128">Property</span></span>|<span data-ttu-id="9e2cc-129">種類</span><span class="sxs-lookup"><span data-stu-id="9e2cc-129">Type</span></span>|<span data-ttu-id="9e2cc-130">説明</span><span class="sxs-lookup"><span data-stu-id="9e2cc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e2cc-131">ID</span><span class="sxs-lookup"><span data-stu-id="9e2cc-131">id</span></span>|<span data-ttu-id="9e2cc-132">String</span><span class="sxs-lookup"><span data-stu-id="9e2cc-132">String</span></span>|<span data-ttu-id="9e2cc-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-133">Key of the entity.</span></span>|
|<span data-ttu-id="9e2cc-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="9e2cc-134">ruleName</span></span>|<span data-ttu-id="9e2cc-135">String</span><span class="sxs-lookup"><span data-stu-id="9e2cc-135">String</span></span>|<span data-ttu-id="9e2cc-136">このスケジュール済みのアクションが適用されるルールの名前です。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="9e2cc-137">応答</span><span class="sxs-lookup"><span data-stu-id="9e2cc-137">Response</span></span>
<span data-ttu-id="9e2cc-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e2cc-139">例</span><span class="sxs-lookup"><span data-stu-id="9e2cc-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e2cc-140">要求</span><span class="sxs-lookup"><span data-stu-id="9e2cc-140">Request</span></span>
<span data-ttu-id="9e2cc-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="9e2cc-142">応答</span><span class="sxs-lookup"><span data-stu-id="9e2cc-142">Response</span></span>
<span data-ttu-id="9e2cc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e2cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```


