---
title: deviceCompliancePolicyAssignment の削除
description: deviceCompliancePolicyAssignment を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ee781452d1163e5fb5efb5d5f3de635fe8d33c2
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264198"
---
# <a name="delete-devicecompliancepolicyassignment"></a><span data-ttu-id="c381a-103">deviceCompliancePolicyAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="c381a-103">Delete deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="c381a-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c381a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c381a-105">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="c381a-105">Deletes a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c381a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c381a-106">Prerequisites</span></span>
<span data-ttu-id="c381a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c381a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c381a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c381a-109">Permission type</span></span>|<span data-ttu-id="c381a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c381a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c381a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c381a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c381a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c381a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c381a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c381a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c381a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c381a-114">Not supported.</span></span>|
|<span data-ttu-id="c381a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c381a-115">Application</span></span>|<span data-ttu-id="c381a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c381a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c381a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c381a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c381a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c381a-118">Request headers</span></span>
|<span data-ttu-id="c381a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c381a-119">Header</span></span>|<span data-ttu-id="c381a-120">値</span><span class="sxs-lookup"><span data-stu-id="c381a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c381a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c381a-121">Authorization</span></span>|<span data-ttu-id="c381a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c381a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c381a-123">承諾</span><span class="sxs-lookup"><span data-stu-id="c381a-123">Accept</span></span>|<span data-ttu-id="c381a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c381a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c381a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c381a-125">Request body</span></span>
<span data-ttu-id="c381a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c381a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c381a-127">応答</span><span class="sxs-lookup"><span data-stu-id="c381a-127">Response</span></span>
<span data-ttu-id="c381a-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c381a-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c381a-129">例</span><span class="sxs-lookup"><span data-stu-id="c381a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="c381a-130">要求</span><span class="sxs-lookup"><span data-stu-id="c381a-130">Request</span></span>
<span data-ttu-id="c381a-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c381a-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="c381a-132">応答</span><span class="sxs-lookup"><span data-stu-id="c381a-132">Response</span></span>
<span data-ttu-id="c381a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c381a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



