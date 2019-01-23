---
title: deviceComplianceScheduledActionForRule の作成
description: 新しい deviceComplianceScheduledActionForRule オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 561dda9270419fcb562f0ccdd8d3d0aa5d354261
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410582"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="a4de6-103">deviceComplianceScheduledActionForRule の作成</span><span class="sxs-lookup"><span data-stu-id="a4de6-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="a4de6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a4de6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a4de6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4de6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a4de6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4de6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4de6-107">新しい [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4de6-107">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4de6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a4de6-108">Prerequisites</span></span>
<span data-ttu-id="a4de6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4de6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a4de6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4de6-111">Permission type</span></span>|<span data-ttu-id="a4de6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4de6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4de6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4de6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a4de6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4de6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4de6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4de6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4de6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4de6-116">Not supported.</span></span>|
|<span data-ttu-id="a4de6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4de6-117">Application</span></span>|<span data-ttu-id="a4de6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4de6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4de6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4de6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="a4de6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4de6-120">Request headers</span></span>
|<span data-ttu-id="a4de6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4de6-121">Header</span></span>|<span data-ttu-id="a4de6-122">値</span><span class="sxs-lookup"><span data-stu-id="a4de6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4de6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4de6-123">Authorization</span></span>|<span data-ttu-id="a4de6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a4de6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4de6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a4de6-125">Accept</span></span>|<span data-ttu-id="a4de6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a4de6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4de6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4de6-127">Request body</span></span>
<span data-ttu-id="a4de6-128">要求本文で、deviceComplianceScheduledActionForRule オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4de6-128">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="a4de6-129">次の表に、deviceComplianceScheduledActionForRule の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a4de6-129">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="a4de6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4de6-130">Property</span></span>|<span data-ttu-id="a4de6-131">型</span><span class="sxs-lookup"><span data-stu-id="a4de6-131">Type</span></span>|<span data-ttu-id="a4de6-132">説明</span><span class="sxs-lookup"><span data-stu-id="a4de6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4de6-133">id</span><span class="sxs-lookup"><span data-stu-id="a4de6-133">id</span></span>|<span data-ttu-id="a4de6-134">String</span><span class="sxs-lookup"><span data-stu-id="a4de6-134">String</span></span>|<span data-ttu-id="a4de6-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a4de6-135">Key of the entity.</span></span>|
|<span data-ttu-id="a4de6-136">ruleName</span><span class="sxs-lookup"><span data-stu-id="a4de6-136">ruleName</span></span>|<span data-ttu-id="a4de6-137">String</span><span class="sxs-lookup"><span data-stu-id="a4de6-137">String</span></span>|<span data-ttu-id="a4de6-138">このスケジュール済みのアクションが適用されるルールの名前です。</span><span class="sxs-lookup"><span data-stu-id="a4de6-138">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="a4de6-139">応答</span><span class="sxs-lookup"><span data-stu-id="a4de6-139">Response</span></span>
<span data-ttu-id="a4de6-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4de6-140">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4de6-141">例</span><span class="sxs-lookup"><span data-stu-id="a4de6-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4de6-142">要求</span><span class="sxs-lookup"><span data-stu-id="a4de6-142">Request</span></span>
<span data-ttu-id="a4de6-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a4de6-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="a4de6-144">応答</span><span class="sxs-lookup"><span data-stu-id="a4de6-144">Response</span></span>
<span data-ttu-id="a4de6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a4de6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




