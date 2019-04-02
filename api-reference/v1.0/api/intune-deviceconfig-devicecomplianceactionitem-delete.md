---
title: Delete deviceComplianceActionItem
description: deviceComplianceActionItem を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 189152018478877b4ee61f437f1c160d0fad1234
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973965"
---
# <a name="delete-devicecomplianceactionitem"></a><span data-ttu-id="c2478-103">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="c2478-103">Delete deviceComplianceActionItem</span></span>

> <span data-ttu-id="c2478-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2478-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2478-105">[deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c2478-105">Deletes a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2478-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c2478-106">Prerequisites</span></span>
<span data-ttu-id="c2478-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2478-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2478-109">Permission type</span></span>|<span data-ttu-id="c2478-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2478-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2478-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2478-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c2478-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2478-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c2478-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2478-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2478-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2478-114">Not supported.</span></span>|
|<span data-ttu-id="c2478-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2478-115">Application</span></span>|<span data-ttu-id="c2478-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2478-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2478-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2478-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="c2478-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2478-118">Request headers</span></span>
|<span data-ttu-id="c2478-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2478-119">Header</span></span>|<span data-ttu-id="c2478-120">値</span><span class="sxs-lookup"><span data-stu-id="c2478-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2478-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2478-121">Authorization</span></span>|<span data-ttu-id="c2478-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c2478-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2478-123">承諾</span><span class="sxs-lookup"><span data-stu-id="c2478-123">Accept</span></span>|<span data-ttu-id="c2478-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c2478-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2478-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2478-125">Request body</span></span>
<span data-ttu-id="c2478-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c2478-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2478-127">応答</span><span class="sxs-lookup"><span data-stu-id="c2478-127">Response</span></span>
<span data-ttu-id="c2478-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c2478-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2478-129">例</span><span class="sxs-lookup"><span data-stu-id="c2478-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2478-130">要求</span><span class="sxs-lookup"><span data-stu-id="c2478-130">Request</span></span>
<span data-ttu-id="c2478-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c2478-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

### <a name="response"></a><span data-ttu-id="c2478-132">応答</span><span class="sxs-lookup"><span data-stu-id="c2478-132">Response</span></span>
<span data-ttu-id="c2478-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c2478-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



