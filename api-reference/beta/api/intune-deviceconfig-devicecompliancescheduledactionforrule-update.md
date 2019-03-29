---
title: deviceComplianceScheduledActionForRule の更新
description: deviceComplianceScheduledActionForRule オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58d447558fd8ae6d7ce5748fad4bd912c71d93fd
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30972194"
---
# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="c3488-103">deviceComplianceScheduledActionForRule の更新</span><span class="sxs-lookup"><span data-stu-id="c3488-103">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="c3488-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3488-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3488-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3488-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3488-106">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c3488-106">Update the properties of a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3488-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3488-107">Prerequisites</span></span>
<span data-ttu-id="c3488-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3488-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3488-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3488-110">Permission type</span></span>|<span data-ttu-id="c3488-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3488-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3488-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3488-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c3488-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3488-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3488-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3488-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3488-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3488-115">Not supported.</span></span>|
|<span data-ttu-id="c3488-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3488-116">Application</span></span>|<span data-ttu-id="c3488-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3488-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3488-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3488-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="c3488-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3488-119">Request headers</span></span>
|<span data-ttu-id="c3488-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3488-120">Header</span></span>|<span data-ttu-id="c3488-121">値</span><span class="sxs-lookup"><span data-stu-id="c3488-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3488-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3488-122">Authorization</span></span>|<span data-ttu-id="c3488-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c3488-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3488-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c3488-124">Accept</span></span>|<span data-ttu-id="c3488-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c3488-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3488-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3488-126">Request body</span></span>
<span data-ttu-id="c3488-127">要求本文で、[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3488-127">In the request body, supply a JSON representation for the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="c3488-128">次の表に、[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c3488-128">The following table shows the properties that are required when you create the [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md).</span></span>

|<span data-ttu-id="c3488-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3488-129">Property</span></span>|<span data-ttu-id="c3488-130">型</span><span class="sxs-lookup"><span data-stu-id="c3488-130">Type</span></span>|<span data-ttu-id="c3488-131">説明</span><span class="sxs-lookup"><span data-stu-id="c3488-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3488-132">id</span><span class="sxs-lookup"><span data-stu-id="c3488-132">id</span></span>|<span data-ttu-id="c3488-133">String</span><span class="sxs-lookup"><span data-stu-id="c3488-133">String</span></span>|<span data-ttu-id="c3488-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c3488-134">Key of the entity.</span></span>|
|<span data-ttu-id="c3488-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="c3488-135">ruleName</span></span>|<span data-ttu-id="c3488-136">String</span><span class="sxs-lookup"><span data-stu-id="c3488-136">String</span></span>|<span data-ttu-id="c3488-137">このスケジュール済みのアクションが適用されるルールの名前です。</span><span class="sxs-lookup"><span data-stu-id="c3488-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="c3488-138">応答</span><span class="sxs-lookup"><span data-stu-id="c3488-138">Response</span></span>
<span data-ttu-id="c3488-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3488-139">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3488-140">例</span><span class="sxs-lookup"><span data-stu-id="c3488-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3488-141">要求</span><span class="sxs-lookup"><span data-stu-id="c3488-141">Request</span></span>
<span data-ttu-id="c3488-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3488-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="c3488-143">応答</span><span class="sxs-lookup"><span data-stu-id="c3488-143">Response</span></span>
<span data-ttu-id="c3488-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3488-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




