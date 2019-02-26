---
title: deviceAndAppManagementRoleAssignment の更新
description: deviceAndAppManagementRoleAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 02574f1e6d8bc64dbc5f3415d5c102ed011f1c11
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263351"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="69ed0-103">deviceAndAppManagementRoleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="69ed0-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="69ed0-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="69ed0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69ed0-105">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="69ed0-105">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69ed0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="69ed0-106">Prerequisites</span></span>
<span data-ttu-id="69ed0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69ed0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="69ed0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69ed0-109">Permission type</span></span>|<span data-ttu-id="69ed0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="69ed0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69ed0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69ed0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69ed0-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69ed0-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="69ed0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69ed0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69ed0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69ed0-114">Not supported.</span></span>|
|<span data-ttu-id="69ed0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69ed0-115">Application</span></span>|<span data-ttu-id="69ed0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69ed0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69ed0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69ed0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="69ed0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69ed0-118">Request headers</span></span>
|<span data-ttu-id="69ed0-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69ed0-119">Header</span></span>|<span data-ttu-id="69ed0-120">値</span><span class="sxs-lookup"><span data-stu-id="69ed0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69ed0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69ed0-121">Authorization</span></span>|<span data-ttu-id="69ed0-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="69ed0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69ed0-123">承諾</span><span class="sxs-lookup"><span data-stu-id="69ed0-123">Accept</span></span>|<span data-ttu-id="69ed0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="69ed0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69ed0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="69ed0-125">Request body</span></span>
<span data-ttu-id="69ed0-126">要求本文で、[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="69ed0-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="69ed0-127">次の表に、[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="69ed0-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="69ed0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69ed0-128">Property</span></span>|<span data-ttu-id="69ed0-129">型</span><span class="sxs-lookup"><span data-stu-id="69ed0-129">Type</span></span>|<span data-ttu-id="69ed0-130">説明</span><span class="sxs-lookup"><span data-stu-id="69ed0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69ed0-131">id</span><span class="sxs-lookup"><span data-stu-id="69ed0-131">id</span></span>|<span data-ttu-id="69ed0-132">String</span><span class="sxs-lookup"><span data-stu-id="69ed0-132">String</span></span>|<span data-ttu-id="69ed0-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="69ed0-133">Key of the entity.</span></span> <span data-ttu-id="69ed0-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="69ed0-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="69ed0-135">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ed0-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="69ed0-136">displayName</span><span class="sxs-lookup"><span data-stu-id="69ed0-136">displayName</span></span>|<span data-ttu-id="69ed0-137">String</span><span class="sxs-lookup"><span data-stu-id="69ed0-137">String</span></span>|<span data-ttu-id="69ed0-138">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="69ed0-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="69ed0-139">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ed0-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="69ed0-140">説明</span><span class="sxs-lookup"><span data-stu-id="69ed0-140">description</span></span>|<span data-ttu-id="69ed0-141">String</span><span class="sxs-lookup"><span data-stu-id="69ed0-141">String</span></span>|<span data-ttu-id="69ed0-142">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="69ed0-142">Description of the Role Assignment.</span></span> <span data-ttu-id="69ed0-143">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ed0-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="69ed0-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="69ed0-144">resourceScopes</span></span>|<span data-ttu-id="69ed0-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="69ed0-145">String collection</span></span>|<span data-ttu-id="69ed0-146">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="69ed0-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="69ed0-147">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="69ed0-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="69ed0-148">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69ed0-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="69ed0-149">members</span><span class="sxs-lookup"><span data-stu-id="69ed0-149">members</span></span>|<span data-ttu-id="69ed0-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="69ed0-150">String collection</span></span>|<span data-ttu-id="69ed0-151">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="69ed0-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="69ed0-152">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="69ed0-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="69ed0-153">応答</span><span class="sxs-lookup"><span data-stu-id="69ed0-153">Response</span></span>
<span data-ttu-id="69ed0-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="69ed0-154">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69ed0-155">例</span><span class="sxs-lookup"><span data-stu-id="69ed0-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="69ed0-156">要求</span><span class="sxs-lookup"><span data-stu-id="69ed0-156">Request</span></span>
<span data-ttu-id="69ed0-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69ed0-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="69ed0-158">応答</span><span class="sxs-lookup"><span data-stu-id="69ed0-158">Response</span></span>
<span data-ttu-id="69ed0-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="69ed0-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



