---
title: deviceAndAppManagementRoleAssignment の作成
description: 新しい deviceAndAppManagementRoleAssignment オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: dc2227837d1652e32353df6aaba96596276ce8c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305657"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="f95df-103">deviceAndAppManagementRoleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="f95df-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="f95df-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f95df-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f95df-105">新しい [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f95df-105">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f95df-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f95df-106">Prerequisites</span></span>
<span data-ttu-id="f95df-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f95df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f95df-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f95df-109">Permission type</span></span>|<span data-ttu-id="f95df-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f95df-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f95df-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f95df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f95df-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95df-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f95df-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f95df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f95df-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f95df-114">Not supported.</span></span>|
|<span data-ttu-id="f95df-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f95df-115">Application</span></span>|<span data-ttu-id="f95df-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f95df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f95df-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f95df-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="f95df-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f95df-118">Request headers</span></span>
|<span data-ttu-id="f95df-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f95df-119">Header</span></span>|<span data-ttu-id="f95df-120">値</span><span class="sxs-lookup"><span data-stu-id="f95df-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f95df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f95df-121">Authorization</span></span>|<span data-ttu-id="f95df-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f95df-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f95df-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f95df-123">Accept</span></span>|<span data-ttu-id="f95df-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f95df-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f95df-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f95df-125">Request body</span></span>
<span data-ttu-id="f95df-126">要求本文で、deviceAndAppManagementRoleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f95df-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="f95df-127">次の表に、deviceAndAppManagementRoleAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f95df-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="f95df-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f95df-128">Property</span></span>|<span data-ttu-id="f95df-129">種類</span><span class="sxs-lookup"><span data-stu-id="f95df-129">Type</span></span>|<span data-ttu-id="f95df-130">説明</span><span class="sxs-lookup"><span data-stu-id="f95df-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f95df-131">ID</span><span class="sxs-lookup"><span data-stu-id="f95df-131">id</span></span>|<span data-ttu-id="f95df-132">String</span><span class="sxs-lookup"><span data-stu-id="f95df-132">String</span></span>|<span data-ttu-id="f95df-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f95df-133">Key of the entity.</span></span> <span data-ttu-id="f95df-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="f95df-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="f95df-135">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f95df-135">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f95df-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f95df-136">displayName</span></span>|<span data-ttu-id="f95df-137">String</span><span class="sxs-lookup"><span data-stu-id="f95df-137">String</span></span>|<span data-ttu-id="f95df-138">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="f95df-138">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="f95df-139">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f95df-139">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f95df-140">説明</span><span class="sxs-lookup"><span data-stu-id="f95df-140">description</span></span>|<span data-ttu-id="f95df-141">String</span><span class="sxs-lookup"><span data-stu-id="f95df-141">String</span></span>|<span data-ttu-id="f95df-142">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="f95df-142">Description of the Role Assignment.</span></span> <span data-ttu-id="f95df-143">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f95df-143">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f95df-144">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="f95df-144">resourceScopes</span></span>|<span data-ttu-id="f95df-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f95df-145">String collection</span></span>|<span data-ttu-id="f95df-146">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="f95df-146">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="f95df-147">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="f95df-147">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="f95df-148">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f95df-148">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="f95df-149">members</span><span class="sxs-lookup"><span data-stu-id="f95df-149">members</span></span>|<span data-ttu-id="f95df-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f95df-150">String collection</span></span>|<span data-ttu-id="f95df-151">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="f95df-151">The list of ids of role member security groups.</span></span> <span data-ttu-id="f95df-152">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="f95df-152">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="f95df-153">応答</span><span class="sxs-lookup"><span data-stu-id="f95df-153">Response</span></span>
<span data-ttu-id="f95df-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f95df-154">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f95df-155">例</span><span class="sxs-lookup"><span data-stu-id="f95df-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="f95df-156">要求</span><span class="sxs-lookup"><span data-stu-id="f95df-156">Request</span></span>
<span data-ttu-id="f95df-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f95df-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
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

### <a name="response"></a><span data-ttu-id="f95df-158">応答</span><span class="sxs-lookup"><span data-stu-id="f95df-158">Response</span></span>
<span data-ttu-id="f95df-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f95df-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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


