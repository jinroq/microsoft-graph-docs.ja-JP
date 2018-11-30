---
title: assign アクション
description: まだ文書化されていません
ms.openlocfilehash: 9cca8b47cd857bce017858d24375b77ea822980d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067587"
---
# <a name="assign-action"></a><span data-ttu-id="30301-103">assign アクション</span><span class="sxs-lookup"><span data-stu-id="30301-103">assign action</span></span>

> <span data-ttu-id="30301-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="30301-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30301-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30301-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30301-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="30301-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30301-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="30301-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30301-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="30301-108">Prerequisites</span></span>
<span data-ttu-id="30301-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30301-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30301-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="30301-111">Permission type</span></span>|<span data-ttu-id="30301-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="30301-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30301-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="30301-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30301-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30301-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="30301-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="30301-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30301-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30301-116">Not supported.</span></span>|
|<span data-ttu-id="30301-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="30301-117">Application</span></span>|<span data-ttu-id="30301-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30301-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30301-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="30301-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="30301-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30301-120">Request headers</span></span>
|<span data-ttu-id="30301-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30301-121">Header</span></span>|<span data-ttu-id="30301-122">値</span><span class="sxs-lookup"><span data-stu-id="30301-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30301-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="30301-123">Authorization</span></span>|<span data-ttu-id="30301-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="30301-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30301-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30301-125">Accept</span></span>|<span data-ttu-id="30301-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30301-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30301-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="30301-127">Request body</span></span>
<span data-ttu-id="30301-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="30301-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="30301-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="30301-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="30301-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30301-130">Property</span></span>|<span data-ttu-id="30301-131">型</span><span class="sxs-lookup"><span data-stu-id="30301-131">Type</span></span>|<span data-ttu-id="30301-132">説明</span><span class="sxs-lookup"><span data-stu-id="30301-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30301-133">assignments</span><span class="sxs-lookup"><span data-stu-id="30301-133">assignments</span></span>|<span data-ttu-id="30301-134">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="30301-134">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="30301-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="30301-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="30301-136">応答</span><span class="sxs-lookup"><span data-stu-id="30301-136">Response</span></span>
<span data-ttu-id="30301-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="30301-137">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30301-138">例</span><span class="sxs-lookup"><span data-stu-id="30301-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="30301-139">要求</span><span class="sxs-lookup"><span data-stu-id="30301-139">Request</span></span>
<span data-ttu-id="30301-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="30301-140">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="30301-141">応答</span><span class="sxs-lookup"><span data-stu-id="30301-141">Response</span></span>
<span data-ttu-id="30301-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="30301-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




