---
title: deviceCompliancePolicyAssignment の作成
description: 新しい deviceCompliancePolicyAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3c181e7362528fe0231e2e744f59ac82d7ee333e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847958"
---
# <a name="create-devicecompliancepolicyassignment"></a><span data-ttu-id="8ee22-103">deviceCompliancePolicyAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="8ee22-103">Create deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="8ee22-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ee22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ee22-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ee22-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ee22-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8ee22-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ee22-107">新しい [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8ee22-107">Create a new [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ee22-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8ee22-108">Prerequisites</span></span>
<span data-ttu-id="8ee22-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ee22-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ee22-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ee22-111">Permission type</span></span>|<span data-ttu-id="8ee22-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ee22-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ee22-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ee22-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ee22-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ee22-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8ee22-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ee22-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ee22-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ee22-116">Not supported.</span></span>|
|<span data-ttu-id="8ee22-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ee22-117">Application</span></span>|<span data-ttu-id="8ee22-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ee22-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ee22-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ee22-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8ee22-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ee22-120">Request headers</span></span>
|<span data-ttu-id="8ee22-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ee22-121">Header</span></span>|<span data-ttu-id="8ee22-122">値</span><span class="sxs-lookup"><span data-stu-id="8ee22-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ee22-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ee22-123">Authorization</span></span>|<span data-ttu-id="8ee22-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8ee22-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ee22-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ee22-125">Accept</span></span>|<span data-ttu-id="8ee22-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ee22-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ee22-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ee22-127">Request body</span></span>
<span data-ttu-id="8ee22-128">要求本文で、deviceCompliancePolicyAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8ee22-128">In the request body, supply a JSON representation for the deviceCompliancePolicyAssignment object.</span></span>

<span data-ttu-id="8ee22-129">次の表に、deviceCompliancePolicyAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8ee22-129">The following table shows the properties that are required when you create the deviceCompliancePolicyAssignment.</span></span>

|<span data-ttu-id="8ee22-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ee22-130">Property</span></span>|<span data-ttu-id="8ee22-131">種類</span><span class="sxs-lookup"><span data-stu-id="8ee22-131">Type</span></span>|<span data-ttu-id="8ee22-132">説明</span><span class="sxs-lookup"><span data-stu-id="8ee22-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ee22-133">ID</span><span class="sxs-lookup"><span data-stu-id="8ee22-133">id</span></span>|<span data-ttu-id="8ee22-134">String</span><span class="sxs-lookup"><span data-stu-id="8ee22-134">String</span></span>|<span data-ttu-id="8ee22-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8ee22-135">Key of the entity.</span></span>|
|<span data-ttu-id="8ee22-136">target</span><span class="sxs-lookup"><span data-stu-id="8ee22-136">target</span></span>|[<span data-ttu-id="8ee22-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8ee22-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8ee22-138">コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="8ee22-138">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="8ee22-139">応答</span><span class="sxs-lookup"><span data-stu-id="8ee22-139">Response</span></span>
<span data-ttu-id="8ee22-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8ee22-140">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ee22-141">例</span><span class="sxs-lookup"><span data-stu-id="8ee22-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ee22-142">要求</span><span class="sxs-lookup"><span data-stu-id="8ee22-142">Request</span></span>
<span data-ttu-id="8ee22-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8ee22-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="8ee22-144">応答</span><span class="sxs-lookup"><span data-stu-id="8ee22-144">Response</span></span>
<span data-ttu-id="8ee22-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8ee22-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





