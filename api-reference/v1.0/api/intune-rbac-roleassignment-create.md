---
title: roleAssignment の作成
description: 新しい roleAssignment オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: ac3a8ee5b007c918a9b655cb2f396c872f9f2d92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27362238"
---
# <a name="create-roleassignment"></a><span data-ttu-id="00cac-103">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="00cac-103">Create roleAssignment</span></span>

> <span data-ttu-id="00cac-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="00cac-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00cac-105">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="00cac-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00cac-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="00cac-106">Prerequisites</span></span>
<span data-ttu-id="00cac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00cac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00cac-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00cac-109">Permission type</span></span>|<span data-ttu-id="00cac-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="00cac-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00cac-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00cac-111">Delegated (work or school account)</span></span>|<span data-ttu-id="00cac-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00cac-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="00cac-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00cac-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00cac-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00cac-114">Not supported.</span></span>|
|<span data-ttu-id="00cac-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00cac-115">Application</span></span>|<span data-ttu-id="00cac-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00cac-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00cac-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00cac-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="00cac-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00cac-118">Request headers</span></span>
|<span data-ttu-id="00cac-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00cac-119">Header</span></span>|<span data-ttu-id="00cac-120">値</span><span class="sxs-lookup"><span data-stu-id="00cac-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00cac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="00cac-121">Authorization</span></span>|<span data-ttu-id="00cac-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="00cac-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00cac-123">Accept</span><span class="sxs-lookup"><span data-stu-id="00cac-123">Accept</span></span>|<span data-ttu-id="00cac-124">application/json</span><span class="sxs-lookup"><span data-stu-id="00cac-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00cac-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="00cac-125">Request body</span></span>
<span data-ttu-id="00cac-126">要求本文で、roleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="00cac-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="00cac-127">次の表に、roleAssignment の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="00cac-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="00cac-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="00cac-128">Property</span></span>|<span data-ttu-id="00cac-129">種類</span><span class="sxs-lookup"><span data-stu-id="00cac-129">Type</span></span>|<span data-ttu-id="00cac-130">説明</span><span class="sxs-lookup"><span data-stu-id="00cac-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00cac-131">ID</span><span class="sxs-lookup"><span data-stu-id="00cac-131">id</span></span>|<span data-ttu-id="00cac-132">String</span><span class="sxs-lookup"><span data-stu-id="00cac-132">String</span></span>|<span data-ttu-id="00cac-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="00cac-133">Key of the entity.</span></span> <span data-ttu-id="00cac-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="00cac-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="00cac-135">displayName</span><span class="sxs-lookup"><span data-stu-id="00cac-135">displayName</span></span>|<span data-ttu-id="00cac-136">String</span><span class="sxs-lookup"><span data-stu-id="00cac-136">String</span></span>|<span data-ttu-id="00cac-137">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="00cac-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="00cac-138">説明</span><span class="sxs-lookup"><span data-stu-id="00cac-138">description</span></span>|<span data-ttu-id="00cac-139">String</span><span class="sxs-lookup"><span data-stu-id="00cac-139">String</span></span>|<span data-ttu-id="00cac-140">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="00cac-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="00cac-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="00cac-141">resourceScopes</span></span>|<span data-ttu-id="00cac-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="00cac-142">String collection</span></span>|<span data-ttu-id="00cac-143">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="00cac-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="00cac-144">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="00cac-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="00cac-145">応答</span><span class="sxs-lookup"><span data-stu-id="00cac-145">Response</span></span>
<span data-ttu-id="00cac-146">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="00cac-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00cac-147">例</span><span class="sxs-lookup"><span data-stu-id="00cac-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="00cac-148">要求</span><span class="sxs-lookup"><span data-stu-id="00cac-148">Request</span></span>
<span data-ttu-id="00cac-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00cac-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
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

### <a name="response"></a><span data-ttu-id="00cac-150">応答</span><span class="sxs-lookup"><span data-stu-id="00cac-150">Response</span></span>
<span data-ttu-id="00cac-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="00cac-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



