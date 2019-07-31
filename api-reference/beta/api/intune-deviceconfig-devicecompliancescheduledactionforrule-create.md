---
title: deviceComplianceScheduledActionForRule の作成
description: 新しい deviceComplianceScheduledActionForRule オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 59e19e57de47bfa3e2ad4322b09129d07546317d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949658"
---
# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="4ae82-103">deviceComplianceScheduledActionForRule の作成</span><span class="sxs-lookup"><span data-stu-id="4ae82-103">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="4ae82-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ae82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ae82-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4ae82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ae82-106">新しい [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4ae82-106">Create a new [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ae82-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4ae82-107">Prerequisites</span></span>
<span data-ttu-id="4ae82-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4ae82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ae82-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4ae82-110">Permission type</span></span>|<span data-ttu-id="4ae82-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4ae82-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ae82-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4ae82-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ae82-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae82-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ae82-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4ae82-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ae82-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ae82-115">Not supported.</span></span>|
|<span data-ttu-id="4ae82-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4ae82-116">Application</span></span>|<span data-ttu-id="4ae82-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ae82-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ae82-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4ae82-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="4ae82-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ae82-119">Request headers</span></span>
|<span data-ttu-id="4ae82-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4ae82-120">Header</span></span>|<span data-ttu-id="4ae82-121">値</span><span class="sxs-lookup"><span data-stu-id="4ae82-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ae82-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ae82-122">Authorization</span></span>|<span data-ttu-id="4ae82-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4ae82-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ae82-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4ae82-124">Accept</span></span>|<span data-ttu-id="4ae82-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ae82-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ae82-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4ae82-126">Request body</span></span>
<span data-ttu-id="4ae82-127">要求本文で、deviceComplianceScheduledActionForRule オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4ae82-127">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="4ae82-128">次の表に、deviceComplianceScheduledActionForRule の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4ae82-128">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="4ae82-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4ae82-129">Property</span></span>|<span data-ttu-id="4ae82-130">型</span><span class="sxs-lookup"><span data-stu-id="4ae82-130">Type</span></span>|<span data-ttu-id="4ae82-131">説明</span><span class="sxs-lookup"><span data-stu-id="4ae82-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ae82-132">id</span><span class="sxs-lookup"><span data-stu-id="4ae82-132">id</span></span>|<span data-ttu-id="4ae82-133">String</span><span class="sxs-lookup"><span data-stu-id="4ae82-133">String</span></span>|<span data-ttu-id="4ae82-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4ae82-134">Key of the entity.</span></span>|
|<span data-ttu-id="4ae82-135">ruleName</span><span class="sxs-lookup"><span data-stu-id="4ae82-135">ruleName</span></span>|<span data-ttu-id="4ae82-136">String</span><span class="sxs-lookup"><span data-stu-id="4ae82-136">String</span></span>|<span data-ttu-id="4ae82-137">このスケジュール済みのアクションが適用されるルールの名前です。</span><span class="sxs-lookup"><span data-stu-id="4ae82-137">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="4ae82-138">応答</span><span class="sxs-lookup"><span data-stu-id="4ae82-138">Response</span></span>
<span data-ttu-id="4ae82-139">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4ae82-139">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ae82-140">例</span><span class="sxs-lookup"><span data-stu-id="4ae82-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ae82-141">要求</span><span class="sxs-lookup"><span data-stu-id="4ae82-141">Request</span></span>
<span data-ttu-id="4ae82-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4ae82-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="4ae82-143">応答</span><span class="sxs-lookup"><span data-stu-id="4ae82-143">Response</span></span>
<span data-ttu-id="4ae82-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4ae82-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





