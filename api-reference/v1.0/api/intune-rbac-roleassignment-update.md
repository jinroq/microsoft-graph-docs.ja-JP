---
title: roleAssignment の更新
description: roleAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 705ab4e06774f81ed47353e15af870af5f437a0b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328505"
---
# <a name="update-roleassignment"></a><span data-ttu-id="7f067-103">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="7f067-103">Update roleAssignment</span></span>

> <span data-ttu-id="7f067-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f067-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f067-105">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f067-105">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f067-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f067-106">Prerequisites</span></span>
<span data-ttu-id="7f067-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f067-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f067-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f067-109">Permission type</span></span>|<span data-ttu-id="7f067-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f067-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f067-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f067-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7f067-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f067-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="7f067-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f067-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f067-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f067-114">Not supported.</span></span>|
|<span data-ttu-id="7f067-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f067-115">Application</span></span>|<span data-ttu-id="7f067-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f067-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f067-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f067-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="7f067-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f067-118">Request headers</span></span>
|<span data-ttu-id="7f067-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f067-119">Header</span></span>|<span data-ttu-id="7f067-120">値</span><span class="sxs-lookup"><span data-stu-id="7f067-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f067-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f067-121">Authorization</span></span>|<span data-ttu-id="7f067-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7f067-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f067-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7f067-123">Accept</span></span>|<span data-ttu-id="7f067-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7f067-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f067-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f067-125">Request body</span></span>
<span data-ttu-id="7f067-126">要求本文で、[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f067-126">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="7f067-127">次の表に、[roleAssignment](../resources/intune-rbac-roleassignment.md) の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f067-127">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="7f067-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f067-128">Property</span></span>|<span data-ttu-id="7f067-129">種類</span><span class="sxs-lookup"><span data-stu-id="7f067-129">Type</span></span>|<span data-ttu-id="7f067-130">説明</span><span class="sxs-lookup"><span data-stu-id="7f067-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f067-131">ID</span><span class="sxs-lookup"><span data-stu-id="7f067-131">id</span></span>|<span data-ttu-id="7f067-132">String</span><span class="sxs-lookup"><span data-stu-id="7f067-132">String</span></span>|<span data-ttu-id="7f067-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7f067-133">Key of the entity.</span></span> <span data-ttu-id="7f067-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="7f067-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="7f067-135">displayName</span><span class="sxs-lookup"><span data-stu-id="7f067-135">displayName</span></span>|<span data-ttu-id="7f067-136">String</span><span class="sxs-lookup"><span data-stu-id="7f067-136">String</span></span>|<span data-ttu-id="7f067-137">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="7f067-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="7f067-138">説明</span><span class="sxs-lookup"><span data-stu-id="7f067-138">description</span></span>|<span data-ttu-id="7f067-139">String</span><span class="sxs-lookup"><span data-stu-id="7f067-139">String</span></span>|<span data-ttu-id="7f067-140">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="7f067-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="7f067-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="7f067-141">resourceScopes</span></span>|<span data-ttu-id="7f067-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7f067-142">String collection</span></span>|<span data-ttu-id="7f067-143">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="7f067-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="7f067-144">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="7f067-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="7f067-145">応答</span><span class="sxs-lookup"><span data-stu-id="7f067-145">Response</span></span>
<span data-ttu-id="7f067-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f067-146">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f067-147">例</span><span class="sxs-lookup"><span data-stu-id="7f067-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f067-148">要求</span><span class="sxs-lookup"><span data-stu-id="7f067-148">Request</span></span>
<span data-ttu-id="7f067-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f067-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="7f067-150">応答</span><span class="sxs-lookup"><span data-stu-id="7f067-150">Response</span></span>
<span data-ttu-id="7f067-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f067-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```



