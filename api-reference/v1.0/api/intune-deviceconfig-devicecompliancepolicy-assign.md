---
title: assign アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: be4fd659bc6dea5c369e8181c071305f3c244f96
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980461"
---
# <a name="assign-action"></a><span data-ttu-id="4a2d6-103">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="4a2d6-103">assign action</span></span>

> <span data-ttu-id="4a2d6-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a2d6-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4a2d6-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a2d6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4a2d6-106">Prerequisites</span></span>
<span data-ttu-id="4a2d6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a2d6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a2d6-109">Permission type</span></span>|<span data-ttu-id="4a2d6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a2d6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a2d6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a2d6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4a2d6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a2d6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4a2d6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a2d6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a2d6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-114">Not supported.</span></span>|
|<span data-ttu-id="4a2d6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a2d6-115">Application</span></span>|<span data-ttu-id="4a2d6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a2d6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a2d6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4a2d6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a2d6-118">Request headers</span></span>
|<span data-ttu-id="4a2d6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a2d6-119">Header</span></span>|<span data-ttu-id="4a2d6-120">値</span><span class="sxs-lookup"><span data-stu-id="4a2d6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a2d6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a2d6-121">Authorization</span></span>|<span data-ttu-id="4a2d6-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a2d6-123">承諾</span><span class="sxs-lookup"><span data-stu-id="4a2d6-123">Accept</span></span>|<span data-ttu-id="4a2d6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4a2d6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a2d6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a2d6-125">Request body</span></span>
<span data-ttu-id="4a2d6-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4a2d6-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4a2d6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a2d6-128">Property</span></span>|<span data-ttu-id="4a2d6-129">型</span><span class="sxs-lookup"><span data-stu-id="4a2d6-129">Type</span></span>|<span data-ttu-id="4a2d6-130">説明</span><span class="sxs-lookup"><span data-stu-id="4a2d6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a2d6-131">assignments</span><span class="sxs-lookup"><span data-stu-id="4a2d6-131">assignments</span></span>|<span data-ttu-id="4a2d6-132">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4a2d6-132">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="4a2d6-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4a2d6-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4a2d6-134">応答</span><span class="sxs-lookup"><span data-stu-id="4a2d6-134">Response</span></span>
<span data-ttu-id="4a2d6-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-135">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a2d6-136">例</span><span class="sxs-lookup"><span data-stu-id="4a2d6-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a2d6-137">要求</span><span class="sxs-lookup"><span data-stu-id="4a2d6-137">Request</span></span>
<span data-ttu-id="4a2d6-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4a2d6-139">応答</span><span class="sxs-lookup"><span data-stu-id="4a2d6-139">Response</span></span>
<span data-ttu-id="4a2d6-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4a2d6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



