---
title: deviceCompliancePolicyAssignment の更新
description: deviceCompliancePolicyAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b86a3e338574aa97f463a9c7a52b41a5fea1e4b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868797"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="4bcb3-103">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="4bcb3-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="4bcb3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bcb3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4bcb3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bcb3-107">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-107">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4bcb3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4bcb3-108">Prerequisites</span></span>
<span data-ttu-id="4bcb3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4bcb3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4bcb3-111">Permission type</span></span>|<span data-ttu-id="4bcb3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4bcb3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bcb3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4bcb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4bcb3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4bcb3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4bcb3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4bcb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bcb3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-116">Not supported.</span></span>|
|<span data-ttu-id="4bcb3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4bcb3-117">Application</span></span>|<span data-ttu-id="4bcb3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bcb3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4bcb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4bcb3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4bcb3-120">Request headers</span></span>
|<span data-ttu-id="4bcb3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4bcb3-121">Header</span></span>|<span data-ttu-id="4bcb3-122">値</span><span class="sxs-lookup"><span data-stu-id="4bcb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bcb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4bcb3-123">Authorization</span></span>|<span data-ttu-id="4bcb3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bcb3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4bcb3-125">Accept</span></span>|<span data-ttu-id="4bcb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4bcb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bcb3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4bcb3-127">Request body</span></span>
<span data-ttu-id="4bcb3-128">要求本文で、[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="4bcb3-129">次の表に、[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="4bcb3-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bcb3-130">Property</span></span>|<span data-ttu-id="4bcb3-131">種類</span><span class="sxs-lookup"><span data-stu-id="4bcb3-131">Type</span></span>|<span data-ttu-id="4bcb3-132">説明</span><span class="sxs-lookup"><span data-stu-id="4bcb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bcb3-133">ID</span><span class="sxs-lookup"><span data-stu-id="4bcb3-133">id</span></span>|<span data-ttu-id="4bcb3-134">String</span><span class="sxs-lookup"><span data-stu-id="4bcb3-134">String</span></span>|<span data-ttu-id="4bcb3-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-135">Key of the entity.</span></span>|
|<span data-ttu-id="4bcb3-136">target</span><span class="sxs-lookup"><span data-stu-id="4bcb3-136">target</span></span>|[<span data-ttu-id="4bcb3-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4bcb3-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="4bcb3-138">コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="4bcb3-139">応答</span><span class="sxs-lookup"><span data-stu-id="4bcb3-139">Response</span></span>
<span data-ttu-id="4bcb3-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-140">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bcb3-141">例</span><span class="sxs-lookup"><span data-stu-id="4bcb3-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bcb3-142">要求</span><span class="sxs-lookup"><span data-stu-id="4bcb3-142">Request</span></span>
<span data-ttu-id="4bcb3-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="4bcb3-144">応答</span><span class="sxs-lookup"><span data-stu-id="4bcb3-144">Response</span></span>
<span data-ttu-id="4bcb3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4bcb3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





