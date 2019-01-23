---
title: deviceComplianceScheduledActionForRule の更新
description: deviceComplianceScheduledActionForRule オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d2ae868b5c11220423c4f1ee496c77f8cd0482c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414642"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="74156-103">deviceComplianceScheduledActionForRule の更新</span><span class="sxs-lookup"><span data-stu-id="74156-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="74156-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="74156-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="74156-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74156-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74156-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="74156-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74156-107">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="74156-107">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74156-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="74156-108">Prerequisites</span></span>
<span data-ttu-id="74156-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74156-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="74156-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74156-111">Permission type</span></span>|<span data-ttu-id="74156-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="74156-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74156-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74156-113">Delegated (work or school account)</span></span>|<span data-ttu-id="74156-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74156-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="74156-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74156-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74156-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74156-116">Not supported.</span></span>|
|<span data-ttu-id="74156-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74156-117">Application</span></span>|<span data-ttu-id="74156-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74156-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74156-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74156-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="74156-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74156-120">Request headers</span></span>
|<span data-ttu-id="74156-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74156-121">Header</span></span>|<span data-ttu-id="74156-122">値</span><span class="sxs-lookup"><span data-stu-id="74156-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74156-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="74156-123">Authorization</span></span>|<span data-ttu-id="74156-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="74156-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74156-125">Accept</span><span class="sxs-lookup"><span data-stu-id="74156-125">Accept</span></span>|<span data-ttu-id="74156-126">application/json</span><span class="sxs-lookup"><span data-stu-id="74156-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74156-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="74156-127">Request body</span></span>
<span data-ttu-id="74156-128">要求本文で、[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="74156-128">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="74156-129">次の表に、[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="74156-129">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="74156-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74156-130">Property</span></span>|<span data-ttu-id="74156-131">型</span><span class="sxs-lookup"><span data-stu-id="74156-131">Type</span></span>|<span data-ttu-id="74156-132">説明</span><span class="sxs-lookup"><span data-stu-id="74156-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74156-133">id</span><span class="sxs-lookup"><span data-stu-id="74156-133">id</span></span>|<span data-ttu-id="74156-134">String</span><span class="sxs-lookup"><span data-stu-id="74156-134">String</span></span>|<span data-ttu-id="74156-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="74156-135">Key of the entity.</span></span>|
|<span data-ttu-id="74156-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="74156-136">ruleName</span></span>|<span data-ttu-id="74156-137">String</span><span class="sxs-lookup"><span data-stu-id="74156-137">String</span></span>|<span data-ttu-id="74156-138">このスケジュール済みのアクションが適用されるルールの名前です。</span><span class="sxs-lookup"><span data-stu-id="74156-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="74156-139">応答</span><span class="sxs-lookup"><span data-stu-id="74156-139">Response</span></span>
<span data-ttu-id="74156-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74156-140">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74156-141">例</span><span class="sxs-lookup"><span data-stu-id="74156-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="74156-142">要求</span><span class="sxs-lookup"><span data-stu-id="74156-142">Request</span></span>
<span data-ttu-id="74156-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74156-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="74156-144">応答</span><span class="sxs-lookup"><span data-stu-id="74156-144">Response</span></span>
<span data-ttu-id="74156-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74156-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




