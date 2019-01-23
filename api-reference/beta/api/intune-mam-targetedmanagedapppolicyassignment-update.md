---
title: targetedManagedAppPolicyAssignment の更新
description: targetedManagedAppPolicyAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: da22dcaa56691e3e248664ca32941e29eaa9100a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401496"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="aaeff-103">targetedManagedAppPolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="aaeff-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="aaeff-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aaeff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="aaeff-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaeff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aaeff-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aaeff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaeff-107">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aaeff-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaeff-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="aaeff-108">Prerequisites</span></span>
<span data-ttu-id="aaeff-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aaeff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aaeff-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aaeff-111">Permission type</span></span>|<span data-ttu-id="aaeff-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aaeff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaeff-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aaeff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aaeff-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aaeff-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="aaeff-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aaeff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaeff-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaeff-116">Not supported.</span></span>|
|<span data-ttu-id="aaeff-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aaeff-117">Application</span></span>|<span data-ttu-id="aaeff-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaeff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaeff-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aaeff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="aaeff-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aaeff-120">Request headers</span></span>
|<span data-ttu-id="aaeff-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aaeff-121">Header</span></span>|<span data-ttu-id="aaeff-122">値</span><span class="sxs-lookup"><span data-stu-id="aaeff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaeff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaeff-123">Authorization</span></span>|<span data-ttu-id="aaeff-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="aaeff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaeff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aaeff-125">Accept</span></span>|<span data-ttu-id="aaeff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aaeff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaeff-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="aaeff-127">Request body</span></span>
<span data-ttu-id="aaeff-128">要求本文で、[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="aaeff-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="aaeff-129">次の表に、[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="aaeff-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="aaeff-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aaeff-130">Property</span></span>|<span data-ttu-id="aaeff-131">型</span><span class="sxs-lookup"><span data-stu-id="aaeff-131">Type</span></span>|<span data-ttu-id="aaeff-132">説明</span><span class="sxs-lookup"><span data-stu-id="aaeff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aaeff-133">id</span><span class="sxs-lookup"><span data-stu-id="aaeff-133">id</span></span>|<span data-ttu-id="aaeff-134">String</span><span class="sxs-lookup"><span data-stu-id="aaeff-134">String</span></span>|<span data-ttu-id="aaeff-135">ID</span><span class="sxs-lookup"><span data-stu-id="aaeff-135">Id</span></span>|
|<span data-ttu-id="aaeff-136">target</span><span class="sxs-lookup"><span data-stu-id="aaeff-136">target</span></span>|[<span data-ttu-id="aaeff-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="aaeff-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="aaeff-138">グループまたはアプリの展開の識別子</span><span class="sxs-lookup"><span data-stu-id="aaeff-138">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="aaeff-139">応答</span><span class="sxs-lookup"><span data-stu-id="aaeff-139">Response</span></span>
<span data-ttu-id="aaeff-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aaeff-140">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaeff-141">例</span><span class="sxs-lookup"><span data-stu-id="aaeff-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaeff-142">要求</span><span class="sxs-lookup"><span data-stu-id="aaeff-142">Request</span></span>
<span data-ttu-id="aaeff-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aaeff-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="aaeff-144">応答</span><span class="sxs-lookup"><span data-stu-id="aaeff-144">Response</span></span>
<span data-ttu-id="aaeff-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aaeff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




