---
title: targetedManagedAppPolicyAssignment の更新
description: targetedManagedAppPolicyAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 642ab5f52a91830bffb3c0e456a69e8f281135ce
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254402"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="e3062-103">targetedManagedAppPolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="e3062-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="e3062-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3062-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3062-105">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3062-105">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3062-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3062-106">Prerequisites</span></span>
<span data-ttu-id="e3062-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3062-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3062-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3062-109">Permission type</span></span>|<span data-ttu-id="e3062-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3062-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3062-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3062-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3062-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3062-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3062-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3062-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3062-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3062-114">Not supported.</span></span>|
|<span data-ttu-id="e3062-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3062-115">Application</span></span>|<span data-ttu-id="e3062-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3062-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3062-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3062-117">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="e3062-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3062-118">Request headers</span></span>
|<span data-ttu-id="e3062-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3062-119">Header</span></span>|<span data-ttu-id="e3062-120">値</span><span class="sxs-lookup"><span data-stu-id="e3062-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3062-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3062-121">Authorization</span></span>|<span data-ttu-id="e3062-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e3062-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3062-123">承諾</span><span class="sxs-lookup"><span data-stu-id="e3062-123">Accept</span></span>|<span data-ttu-id="e3062-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e3062-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3062-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3062-125">Request body</span></span>
<span data-ttu-id="e3062-126">要求本文で、[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3062-126">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="e3062-127">次の表に、[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e3062-127">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="e3062-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3062-128">Property</span></span>|<span data-ttu-id="e3062-129">型</span><span class="sxs-lookup"><span data-stu-id="e3062-129">Type</span></span>|<span data-ttu-id="e3062-130">説明</span><span class="sxs-lookup"><span data-stu-id="e3062-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3062-131">id</span><span class="sxs-lookup"><span data-stu-id="e3062-131">id</span></span>|<span data-ttu-id="e3062-132">String</span><span class="sxs-lookup"><span data-stu-id="e3062-132">String</span></span>|<span data-ttu-id="e3062-133">ID</span><span class="sxs-lookup"><span data-stu-id="e3062-133">Id</span></span>|
|<span data-ttu-id="e3062-134">target</span><span class="sxs-lookup"><span data-stu-id="e3062-134">target</span></span>|[<span data-ttu-id="e3062-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e3062-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e3062-136">グループまたはアプリの展開の識別子</span><span class="sxs-lookup"><span data-stu-id="e3062-136">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="e3062-137">応答</span><span class="sxs-lookup"><span data-stu-id="e3062-137">Response</span></span>
<span data-ttu-id="e3062-138">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3062-138">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3062-139">例</span><span class="sxs-lookup"><span data-stu-id="e3062-139">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3062-140">要求</span><span class="sxs-lookup"><span data-stu-id="e3062-140">Request</span></span>
<span data-ttu-id="e3062-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3062-141">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 174

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e3062-142">応答</span><span class="sxs-lookup"><span data-stu-id="e3062-142">Response</span></span>
<span data-ttu-id="e3062-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3062-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



