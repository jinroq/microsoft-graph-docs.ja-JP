---
title: deviceComplianceScheduledActionForRule の作成
description: 新しい deviceComplianceScheduledActionForRule オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 2bf76bc65fe139d41364c9fc1a162d2eadaedec4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327084"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="a6b17-103">deviceComplianceScheduledActionForRule の作成</span><span class="sxs-lookup"><span data-stu-id="a6b17-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="a6b17-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6b17-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6b17-105">新しい [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a6b17-105">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6b17-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a6b17-106">Prerequisites</span></span>
<span data-ttu-id="a6b17-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6b17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6b17-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6b17-109">Permission type</span></span>|<span data-ttu-id="a6b17-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6b17-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6b17-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6b17-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a6b17-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6b17-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6b17-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6b17-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6b17-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6b17-114">Not supported.</span></span>|
|<span data-ttu-id="a6b17-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6b17-115">Application</span></span>|<span data-ttu-id="a6b17-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6b17-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6b17-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6b17-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="a6b17-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6b17-118">Request headers</span></span>
|<span data-ttu-id="a6b17-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6b17-119">Header</span></span>|<span data-ttu-id="a6b17-120">値</span><span class="sxs-lookup"><span data-stu-id="a6b17-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6b17-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6b17-121">Authorization</span></span>|<span data-ttu-id="a6b17-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a6b17-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6b17-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a6b17-123">Accept</span></span>|<span data-ttu-id="a6b17-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a6b17-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6b17-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6b17-125">Request body</span></span>
<span data-ttu-id="a6b17-126">要求本文で、deviceComplianceScheduledActionForRule オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6b17-126">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="a6b17-127">次の表に、deviceComplianceScheduledActionForRule の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a6b17-127">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="a6b17-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6b17-128">Property</span></span>|<span data-ttu-id="a6b17-129">種類</span><span class="sxs-lookup"><span data-stu-id="a6b17-129">Type</span></span>|<span data-ttu-id="a6b17-130">説明</span><span class="sxs-lookup"><span data-stu-id="a6b17-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b17-131">ID</span><span class="sxs-lookup"><span data-stu-id="a6b17-131">id</span></span>|<span data-ttu-id="a6b17-132">String</span><span class="sxs-lookup"><span data-stu-id="a6b17-132">String</span></span>|<span data-ttu-id="a6b17-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a6b17-133">Key of the entity.</span></span>|
|<span data-ttu-id="a6b17-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="a6b17-134">ruleName</span></span>|<span data-ttu-id="a6b17-135">String</span><span class="sxs-lookup"><span data-stu-id="a6b17-135">String</span></span>|<span data-ttu-id="a6b17-136">このスケジュール済みのアクションが適用されるルールの名前です。</span><span class="sxs-lookup"><span data-stu-id="a6b17-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="a6b17-137">応答</span><span class="sxs-lookup"><span data-stu-id="a6b17-137">Response</span></span>
<span data-ttu-id="a6b17-138">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a6b17-138">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6b17-139">例</span><span class="sxs-lookup"><span data-stu-id="a6b17-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6b17-140">要求</span><span class="sxs-lookup"><span data-stu-id="a6b17-140">Request</span></span>
<span data-ttu-id="a6b17-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6b17-141">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="a6b17-142">応答</span><span class="sxs-lookup"><span data-stu-id="a6b17-142">Response</span></span>
<span data-ttu-id="a6b17-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6b17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```



