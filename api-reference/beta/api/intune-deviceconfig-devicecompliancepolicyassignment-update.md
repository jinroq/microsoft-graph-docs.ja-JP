---
title: deviceCompliancePolicyAssignment の更新
description: deviceCompliancePolicyAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 79849e7ba9efc1223c1069b2d0771335bea65f04
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949777"
---
# <a name="update-devicecompliancepolicyassignment"></a><span data-ttu-id="62b4f-103">deviceCompliancePolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="62b4f-103">Update deviceCompliancePolicyAssignment</span></span>

> <span data-ttu-id="62b4f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62b4f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62b4f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62b4f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62b4f-106">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="62b4f-106">Update the properties of a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62b4f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="62b4f-107">Prerequisites</span></span>
<span data-ttu-id="62b4f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62b4f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62b4f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62b4f-110">Permission type</span></span>|<span data-ttu-id="62b4f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="62b4f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62b4f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62b4f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62b4f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62b4f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62b4f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62b4f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62b4f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62b4f-115">Not supported.</span></span>|
|<span data-ttu-id="62b4f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62b4f-116">Application</span></span>|<span data-ttu-id="62b4f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62b4f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62b4f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62b4f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="62b4f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62b4f-119">Request headers</span></span>
|<span data-ttu-id="62b4f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62b4f-120">Header</span></span>|<span data-ttu-id="62b4f-121">値</span><span class="sxs-lookup"><span data-stu-id="62b4f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62b4f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62b4f-122">Authorization</span></span>|<span data-ttu-id="62b4f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="62b4f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62b4f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="62b4f-124">Accept</span></span>|<span data-ttu-id="62b4f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62b4f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62b4f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="62b4f-126">Request body</span></span>
<span data-ttu-id="62b4f-127">要求本文で、[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="62b4f-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object.</span></span>

<span data-ttu-id="62b4f-128">次の表に、[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="62b4f-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span></span>

|<span data-ttu-id="62b4f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62b4f-129">Property</span></span>|<span data-ttu-id="62b4f-130">型</span><span class="sxs-lookup"><span data-stu-id="62b4f-130">Type</span></span>|<span data-ttu-id="62b4f-131">説明</span><span class="sxs-lookup"><span data-stu-id="62b4f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62b4f-132">id</span><span class="sxs-lookup"><span data-stu-id="62b4f-132">id</span></span>|<span data-ttu-id="62b4f-133">String</span><span class="sxs-lookup"><span data-stu-id="62b4f-133">String</span></span>|<span data-ttu-id="62b4f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="62b4f-134">Key of the entity.</span></span>|
|<span data-ttu-id="62b4f-135">target</span><span class="sxs-lookup"><span data-stu-id="62b4f-135">target</span></span>|[<span data-ttu-id="62b4f-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="62b4f-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="62b4f-137">コンプライアンス ポリシーの割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="62b4f-137">Target for the compliance policy assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="62b4f-138">応答</span><span class="sxs-lookup"><span data-stu-id="62b4f-138">Response</span></span>
<span data-ttu-id="62b4f-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="62b4f-139">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62b4f-140">例</span><span class="sxs-lookup"><span data-stu-id="62b4f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="62b4f-141">要求</span><span class="sxs-lookup"><span data-stu-id="62b4f-141">Request</span></span>
<span data-ttu-id="62b4f-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="62b4f-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments/{deviceCompliancePolicyAssignmentId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="62b4f-143">応答</span><span class="sxs-lookup"><span data-stu-id="62b4f-143">Response</span></span>
<span data-ttu-id="62b4f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="62b4f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





