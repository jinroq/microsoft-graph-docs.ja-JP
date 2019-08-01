---
title: deviceAndAppManagementRoleAssignment の更新
description: deviceAndAppManagementRoleAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9ac6c2d4d2c25122f5f6d766e06d907301a08b17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023875"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="07cd6-103">deviceAndAppManagementRoleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="07cd6-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="07cd6-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="07cd6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07cd6-105">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="07cd6-105">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07cd6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="07cd6-106">Prerequisites</span></span>
<span data-ttu-id="07cd6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07cd6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07cd6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07cd6-109">Permission type</span></span>|<span data-ttu-id="07cd6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="07cd6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07cd6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07cd6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="07cd6-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07cd6-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="07cd6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07cd6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07cd6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07cd6-114">Not supported.</span></span>|
|<span data-ttu-id="07cd6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07cd6-115">Application</span></span>|<span data-ttu-id="07cd6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07cd6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07cd6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07cd6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="07cd6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07cd6-118">Request headers</span></span>
|<span data-ttu-id="07cd6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07cd6-119">Header</span></span>|<span data-ttu-id="07cd6-120">値</span><span class="sxs-lookup"><span data-stu-id="07cd6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07cd6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="07cd6-121">Authorization</span></span>|<span data-ttu-id="07cd6-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="07cd6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07cd6-123">承諾</span><span class="sxs-lookup"><span data-stu-id="07cd6-123">Accept</span></span>|<span data-ttu-id="07cd6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="07cd6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07cd6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="07cd6-125">Request body</span></span>
<span data-ttu-id="07cd6-126">要求本文で、[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="07cd6-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="07cd6-127">次の表に、[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="07cd6-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="07cd6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07cd6-128">Property</span></span>|<span data-ttu-id="07cd6-129">型</span><span class="sxs-lookup"><span data-stu-id="07cd6-129">Type</span></span>|<span data-ttu-id="07cd6-130">説明</span><span class="sxs-lookup"><span data-stu-id="07cd6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07cd6-131">id</span><span class="sxs-lookup"><span data-stu-id="07cd6-131">id</span></span>|<span data-ttu-id="07cd6-132">文字列</span><span class="sxs-lookup"><span data-stu-id="07cd6-132">String</span></span>|<span data-ttu-id="07cd6-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="07cd6-133">Key of the entity.</span></span> <span data-ttu-id="07cd6-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="07cd6-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="07cd6-135">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07cd6-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="07cd6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="07cd6-136">displayName</span></span>|<span data-ttu-id="07cd6-137">String</span><span class="sxs-lookup"><span data-stu-id="07cd6-137">String</span></span>|<span data-ttu-id="07cd6-138">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="07cd6-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="07cd6-139">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07cd6-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="07cd6-140">description</span><span class="sxs-lookup"><span data-stu-id="07cd6-140">description</span></span>|<span data-ttu-id="07cd6-141">String</span><span class="sxs-lookup"><span data-stu-id="07cd6-141">String</span></span>|<span data-ttu-id="07cd6-142">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="07cd6-142">Description of the Role Assignment.</span></span> <span data-ttu-id="07cd6-143">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07cd6-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="07cd6-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="07cd6-144">resourceScopes</span></span>|<span data-ttu-id="07cd6-145">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="07cd6-145">String collection</span></span>|<span data-ttu-id="07cd6-146">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="07cd6-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="07cd6-147">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="07cd6-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="07cd6-148">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="07cd6-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="07cd6-149">members</span><span class="sxs-lookup"><span data-stu-id="07cd6-149">members</span></span>|<span data-ttu-id="07cd6-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="07cd6-150">String collection</span></span>|<span data-ttu-id="07cd6-151">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="07cd6-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="07cd6-152">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="07cd6-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="07cd6-153">応答</span><span class="sxs-lookup"><span data-stu-id="07cd6-153">Response</span></span>
<span data-ttu-id="07cd6-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="07cd6-154">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07cd6-155">例</span><span class="sxs-lookup"><span data-stu-id="07cd6-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="07cd6-156">要求</span><span class="sxs-lookup"><span data-stu-id="07cd6-156">Request</span></span>
<span data-ttu-id="07cd6-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="07cd6-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="07cd6-158">応答</span><span class="sxs-lookup"><span data-stu-id="07cd6-158">Response</span></span>
<span data-ttu-id="07cd6-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07cd6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



