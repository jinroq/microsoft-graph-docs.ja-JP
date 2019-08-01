---
title: deviceComplianceScheduledActionForRule の更新
description: deviceComplianceScheduledActionForRule オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4c90c450d4f9efc8147414582bb3e48d2e47bd35
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017715"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="a5337-103">deviceComplianceScheduledActionForRule の更新</span><span class="sxs-lookup"><span data-stu-id="a5337-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="a5337-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5337-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5337-105">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5337-105">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5337-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a5337-106">Prerequisites</span></span>
<span data-ttu-id="a5337-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5337-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5337-109">Permission type</span></span>|<span data-ttu-id="a5337-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5337-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5337-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5337-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a5337-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5337-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a5337-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5337-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5337-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5337-114">Not supported.</span></span>|
|<span data-ttu-id="a5337-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5337-115">Application</span></span>|<span data-ttu-id="a5337-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5337-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5337-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5337-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="a5337-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5337-118">Request headers</span></span>
|<span data-ttu-id="a5337-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5337-119">Header</span></span>|<span data-ttu-id="a5337-120">値</span><span class="sxs-lookup"><span data-stu-id="a5337-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5337-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5337-121">Authorization</span></span>|<span data-ttu-id="a5337-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5337-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5337-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a5337-123">Accept</span></span>|<span data-ttu-id="a5337-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a5337-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5337-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5337-125">Request body</span></span>
<span data-ttu-id="a5337-126">要求本文で、[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5337-126">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="a5337-127">次の表に、[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a5337-127">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="a5337-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5337-128">Property</span></span>|<span data-ttu-id="a5337-129">型</span><span class="sxs-lookup"><span data-stu-id="a5337-129">Type</span></span>|<span data-ttu-id="a5337-130">説明</span><span class="sxs-lookup"><span data-stu-id="a5337-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5337-131">id</span><span class="sxs-lookup"><span data-stu-id="a5337-131">id</span></span>|<span data-ttu-id="a5337-132">String</span><span class="sxs-lookup"><span data-stu-id="a5337-132">String</span></span>|<span data-ttu-id="a5337-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a5337-133">Key of the entity.</span></span>|
|<span data-ttu-id="a5337-134">ruleName</span><span class="sxs-lookup"><span data-stu-id="a5337-134">ruleName</span></span>|<span data-ttu-id="a5337-135">String</span><span class="sxs-lookup"><span data-stu-id="a5337-135">String</span></span>|<span data-ttu-id="a5337-136">このスケジュール済みのアクションが適用されるルールの名前です。</span><span class="sxs-lookup"><span data-stu-id="a5337-136">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="a5337-137">応答</span><span class="sxs-lookup"><span data-stu-id="a5337-137">Response</span></span>
<span data-ttu-id="a5337-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a5337-138">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5337-139">例</span><span class="sxs-lookup"><span data-stu-id="a5337-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5337-140">要求</span><span class="sxs-lookup"><span data-stu-id="a5337-140">Request</span></span>
<span data-ttu-id="a5337-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5337-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="a5337-142">応答</span><span class="sxs-lookup"><span data-stu-id="a5337-142">Response</span></span>
<span data-ttu-id="a5337-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5337-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



