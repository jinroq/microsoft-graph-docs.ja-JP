---
title: deviceCompliancePolicyAssignment の更新
description: deviceCompliancePolicyAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 31fb66288f2c7706115b9d1ab52efa652b0b98ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968646"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="56e9c-103">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="56e9c-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="56e9c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="56e9c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56e9c-105">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="56e9c-105">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56e9c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="56e9c-106">Prerequisites</span></span>
<span data-ttu-id="56e9c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56e9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56e9c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56e9c-109">Permission type</span></span>|<span data-ttu-id="56e9c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="56e9c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56e9c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56e9c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="56e9c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56e9c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="56e9c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56e9c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56e9c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56e9c-114">Not supported.</span></span>|
|<span data-ttu-id="56e9c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56e9c-115">Application</span></span>|<span data-ttu-id="56e9c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56e9c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56e9c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56e9c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="56e9c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56e9c-118">Request headers</span></span>
|<span data-ttu-id="56e9c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56e9c-119">Header</span></span>|<span data-ttu-id="56e9c-120">値</span><span class="sxs-lookup"><span data-stu-id="56e9c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56e9c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="56e9c-121">Authorization</span></span>|<span data-ttu-id="56e9c-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="56e9c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56e9c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="56e9c-123">Accept</span></span>|<span data-ttu-id="56e9c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="56e9c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56e9c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="56e9c-125">Request body</span></span>
<span data-ttu-id="56e9c-126">要求本文で、[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56e9c-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="56e9c-127">次の表に、[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="56e9c-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="56e9c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56e9c-128">Property</span></span>|<span data-ttu-id="56e9c-129">種類</span><span class="sxs-lookup"><span data-stu-id="56e9c-129">Type</span></span>|<span data-ttu-id="56e9c-130">説明</span><span class="sxs-lookup"><span data-stu-id="56e9c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56e9c-131">ID</span><span class="sxs-lookup"><span data-stu-id="56e9c-131">id</span></span>|<span data-ttu-id="56e9c-132">String</span><span class="sxs-lookup"><span data-stu-id="56e9c-132">String</span></span>|<span data-ttu-id="56e9c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="56e9c-133">Key of the entity.</span></span>|
|<span data-ttu-id="56e9c-134">target</span><span class="sxs-lookup"><span data-stu-id="56e9c-134">target</span></span>|[<span data-ttu-id="56e9c-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="56e9c-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="56e9c-136">コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="56e9c-136">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="56e9c-137">応答</span><span class="sxs-lookup"><span data-stu-id="56e9c-137">Response</span></span>
<span data-ttu-id="56e9c-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56e9c-138">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56e9c-139">例</span><span class="sxs-lookup"><span data-stu-id="56e9c-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="56e9c-140">要求</span><span class="sxs-lookup"><span data-stu-id="56e9c-140">Request</span></span>
<span data-ttu-id="56e9c-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56e9c-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="56e9c-142">応答</span><span class="sxs-lookup"><span data-stu-id="56e9c-142">Response</span></span>
<span data-ttu-id="56e9c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56e9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



