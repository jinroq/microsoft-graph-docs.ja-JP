---
title: scheduleActionsForRules アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ced79558b7a106e57468cacd7db2e2bd5ae97bc5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32459914"
---
# <a name="scheduleactionsforrules-action"></a><span data-ttu-id="8bbc2-103">scheduleActionsForRules アクション</span><span class="sxs-lookup"><span data-stu-id="8bbc2-103">scheduleActionsForRules action</span></span>

> <span data-ttu-id="8bbc2-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8bbc2-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8bbc2-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8bbc2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8bbc2-106">Prerequisites</span></span>
<span data-ttu-id="8bbc2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bbc2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8bbc2-109">Permission type</span></span>|<span data-ttu-id="8bbc2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8bbc2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8bbc2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bbc2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8bbc2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8bbc2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8bbc2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-114">Not supported.</span></span>|
|<span data-ttu-id="8bbc2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8bbc2-115">Application</span></span>|<span data-ttu-id="8bbc2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8bbc2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8bbc2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules
```

## <a name="request-headers"></a><span data-ttu-id="8bbc2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bbc2-118">Request headers</span></span>
|<span data-ttu-id="8bbc2-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8bbc2-119">Header</span></span>|<span data-ttu-id="8bbc2-120">値</span><span class="sxs-lookup"><span data-stu-id="8bbc2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8bbc2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bbc2-121">Authorization</span></span>|<span data-ttu-id="8bbc2-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8bbc2-123">承諾</span><span class="sxs-lookup"><span data-stu-id="8bbc2-123">Accept</span></span>|<span data-ttu-id="8bbc2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8bbc2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8bbc2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8bbc2-125">Request body</span></span>
<span data-ttu-id="8bbc2-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8bbc2-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8bbc2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8bbc2-128">Property</span></span>|<span data-ttu-id="8bbc2-129">型</span><span class="sxs-lookup"><span data-stu-id="8bbc2-129">Type</span></span>|<span data-ttu-id="8bbc2-130">説明</span><span class="sxs-lookup"><span data-stu-id="8bbc2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bbc2-131">deviceComplianceScheduledActionForRules</span><span class="sxs-lookup"><span data-stu-id="8bbc2-131">deviceComplianceScheduledActionForRules</span></span>|<span data-ttu-id="8bbc2-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8bbc2-132">[deviceComplianceScheduledActionForRule](../resources/intune-deviceconfig-devicecompliancescheduledactionforrule.md) collection</span></span>|<span data-ttu-id="8bbc2-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8bbc2-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="8bbc2-134">応答</span><span class="sxs-lookup"><span data-stu-id="8bbc2-134">Response</span></span>
<span data-ttu-id="8bbc2-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8bbc2-136">例</span><span class="sxs-lookup"><span data-stu-id="8bbc2-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bbc2-137">要求</span><span class="sxs-lookup"><span data-stu-id="8bbc2-137">Request</span></span>
<span data-ttu-id="8bbc2-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduleActionsForRules

Content-type: application/json
Content-length: 242

{
  "deviceComplianceScheduledActionForRules": [
    {
      "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
      "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
      "ruleName": "Rule Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="8bbc2-139">応答</span><span class="sxs-lookup"><span data-stu-id="8bbc2-139">Response</span></span>
<span data-ttu-id="8bbc2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8bbc2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



