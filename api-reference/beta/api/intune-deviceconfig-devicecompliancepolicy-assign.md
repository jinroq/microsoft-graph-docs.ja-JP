---
title: assign アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 34c16efb3a0454f760cf34b8914eadb61d3e4bba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949903"
---
# <a name="assign-action"></a><span data-ttu-id="5c4bf-103">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="5c4bf-103">assign action</span></span>

> <span data-ttu-id="5c4bf-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c4bf-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c4bf-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5c4bf-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c4bf-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5c4bf-107">Prerequisites</span></span>
<span data-ttu-id="5c4bf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c4bf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c4bf-110">Permission type</span></span>|<span data-ttu-id="5c4bf-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c4bf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c4bf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c4bf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5c4bf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c4bf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5c4bf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c4bf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c4bf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-115">Not supported.</span></span>|
|<span data-ttu-id="5c4bf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c4bf-116">Application</span></span>|<span data-ttu-id="5c4bf-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c4bf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c4bf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="5c4bf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c4bf-119">Request headers</span></span>
|<span data-ttu-id="5c4bf-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c4bf-120">Header</span></span>|<span data-ttu-id="5c4bf-121">値</span><span class="sxs-lookup"><span data-stu-id="5c4bf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c4bf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c4bf-122">Authorization</span></span>|<span data-ttu-id="5c4bf-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c4bf-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5c4bf-124">Accept</span></span>|<span data-ttu-id="5c4bf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5c4bf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c4bf-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c4bf-126">Request body</span></span>
<span data-ttu-id="5c4bf-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="5c4bf-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="5c4bf-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c4bf-129">Property</span></span>|<span data-ttu-id="5c4bf-130">型</span><span class="sxs-lookup"><span data-stu-id="5c4bf-130">Type</span></span>|<span data-ttu-id="5c4bf-131">説明</span><span class="sxs-lookup"><span data-stu-id="5c4bf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c4bf-132">assignments</span><span class="sxs-lookup"><span data-stu-id="5c4bf-132">assignments</span></span>|<span data-ttu-id="5c4bf-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5c4bf-133">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="5c4bf-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5c4bf-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="5c4bf-135">応答</span><span class="sxs-lookup"><span data-stu-id="5c4bf-135">Response</span></span>
<span data-ttu-id="5c4bf-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-136">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c4bf-137">例</span><span class="sxs-lookup"><span data-stu-id="5c4bf-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c4bf-138">要求</span><span class="sxs-lookup"><span data-stu-id="5c4bf-138">Request</span></span>
<span data-ttu-id="5c4bf-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

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

### <a name="response"></a><span data-ttu-id="5c4bf-140">応答</span><span class="sxs-lookup"><span data-stu-id="5c4bf-140">Response</span></span>
<span data-ttu-id="5c4bf-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5c4bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





