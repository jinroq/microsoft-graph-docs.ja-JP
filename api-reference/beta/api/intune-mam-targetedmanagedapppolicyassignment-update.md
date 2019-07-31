---
title: targetedManagedAppPolicyAssignment の更新
description: targetedManagedAppPolicyAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a3a64b18da8b93d17920b015ce80b3e65ca99c3d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35994391"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="57913-103">targetedManagedAppPolicyAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="57913-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="57913-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57913-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57913-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="57913-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57913-106">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="57913-106">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57913-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="57913-107">Prerequisites</span></span>
<span data-ttu-id="57913-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57913-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57913-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="57913-110">Permission type</span></span>|<span data-ttu-id="57913-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="57913-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57913-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57913-112">Delegated (work or school account)</span></span>|<span data-ttu-id="57913-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57913-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="57913-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57913-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57913-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57913-115">Not supported.</span></span>|
|<span data-ttu-id="57913-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57913-116">Application</span></span>|<span data-ttu-id="57913-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57913-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="57913-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57913-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="57913-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57913-119">Request headers</span></span>
|<span data-ttu-id="57913-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57913-120">Header</span></span>|<span data-ttu-id="57913-121">値</span><span class="sxs-lookup"><span data-stu-id="57913-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57913-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="57913-122">Authorization</span></span>|<span data-ttu-id="57913-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="57913-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57913-124">承諾</span><span class="sxs-lookup"><span data-stu-id="57913-124">Accept</span></span>|<span data-ttu-id="57913-125">application/json</span><span class="sxs-lookup"><span data-stu-id="57913-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57913-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="57913-126">Request body</span></span>
<span data-ttu-id="57913-127">要求本文で、[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="57913-127">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="57913-128">次の表に、[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="57913-128">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="57913-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57913-129">Property</span></span>|<span data-ttu-id="57913-130">型</span><span class="sxs-lookup"><span data-stu-id="57913-130">Type</span></span>|<span data-ttu-id="57913-131">説明</span><span class="sxs-lookup"><span data-stu-id="57913-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57913-132">id</span><span class="sxs-lookup"><span data-stu-id="57913-132">id</span></span>|<span data-ttu-id="57913-133">String</span><span class="sxs-lookup"><span data-stu-id="57913-133">String</span></span>|<span data-ttu-id="57913-134">ID</span><span class="sxs-lookup"><span data-stu-id="57913-134">Id</span></span>|
|<span data-ttu-id="57913-135">target</span><span class="sxs-lookup"><span data-stu-id="57913-135">target</span></span>|[<span data-ttu-id="57913-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="57913-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="57913-137">グループまたはアプリの展開の識別子</span><span class="sxs-lookup"><span data-stu-id="57913-137">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="57913-138">応答</span><span class="sxs-lookup"><span data-stu-id="57913-138">Response</span></span>
<span data-ttu-id="57913-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="57913-139">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57913-140">例</span><span class="sxs-lookup"><span data-stu-id="57913-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="57913-141">要求</span><span class="sxs-lookup"><span data-stu-id="57913-141">Request</span></span>
<span data-ttu-id="57913-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="57913-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="57913-143">応答</span><span class="sxs-lookup"><span data-stu-id="57913-143">Response</span></span>
<span data-ttu-id="57913-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="57913-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





