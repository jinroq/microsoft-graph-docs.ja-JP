---
title: roleAssignment の作成
description: 新しい roleAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8bd191f52886d06ff2d059507227efdc826a7961
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023714"
---
# <a name="create-roleassignment"></a><span data-ttu-id="44a7d-103">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="44a7d-103">Create roleAssignment</span></span>

> <span data-ttu-id="44a7d-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="44a7d-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44a7d-105">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="44a7d-105">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44a7d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="44a7d-106">Prerequisites</span></span>
<span data-ttu-id="44a7d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44a7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44a7d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44a7d-109">Permission type</span></span>|<span data-ttu-id="44a7d-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="44a7d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44a7d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44a7d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="44a7d-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44a7d-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="44a7d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44a7d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44a7d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44a7d-114">Not supported.</span></span>|
|<span data-ttu-id="44a7d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44a7d-115">Application</span></span>|<span data-ttu-id="44a7d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44a7d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44a7d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44a7d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="44a7d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44a7d-118">Request headers</span></span>
|<span data-ttu-id="44a7d-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44a7d-119">Header</span></span>|<span data-ttu-id="44a7d-120">値</span><span class="sxs-lookup"><span data-stu-id="44a7d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44a7d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44a7d-121">Authorization</span></span>|<span data-ttu-id="44a7d-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="44a7d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44a7d-123">承諾</span><span class="sxs-lookup"><span data-stu-id="44a7d-123">Accept</span></span>|<span data-ttu-id="44a7d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="44a7d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44a7d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="44a7d-125">Request body</span></span>
<span data-ttu-id="44a7d-126">要求本文で、roleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="44a7d-126">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="44a7d-127">次の表に、roleAssignment の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="44a7d-127">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="44a7d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="44a7d-128">Property</span></span>|<span data-ttu-id="44a7d-129">型</span><span class="sxs-lookup"><span data-stu-id="44a7d-129">Type</span></span>|<span data-ttu-id="44a7d-130">説明</span><span class="sxs-lookup"><span data-stu-id="44a7d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44a7d-131">id</span><span class="sxs-lookup"><span data-stu-id="44a7d-131">id</span></span>|<span data-ttu-id="44a7d-132">文字列</span><span class="sxs-lookup"><span data-stu-id="44a7d-132">String</span></span>|<span data-ttu-id="44a7d-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="44a7d-133">Key of the entity.</span></span> <span data-ttu-id="44a7d-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="44a7d-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="44a7d-135">displayName</span><span class="sxs-lookup"><span data-stu-id="44a7d-135">displayName</span></span>|<span data-ttu-id="44a7d-136">String</span><span class="sxs-lookup"><span data-stu-id="44a7d-136">String</span></span>|<span data-ttu-id="44a7d-137">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="44a7d-137">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="44a7d-138">description</span><span class="sxs-lookup"><span data-stu-id="44a7d-138">description</span></span>|<span data-ttu-id="44a7d-139">String</span><span class="sxs-lookup"><span data-stu-id="44a7d-139">String</span></span>|<span data-ttu-id="44a7d-140">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="44a7d-140">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="44a7d-141">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="44a7d-141">resourceScopes</span></span>|<span data-ttu-id="44a7d-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="44a7d-142">String collection</span></span>|<span data-ttu-id="44a7d-143">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="44a7d-143">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="44a7d-144">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="44a7d-144">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="44a7d-145">応答</span><span class="sxs-lookup"><span data-stu-id="44a7d-145">Response</span></span>
<span data-ttu-id="44a7d-146">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="44a7d-146">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44a7d-147">例</span><span class="sxs-lookup"><span data-stu-id="44a7d-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="44a7d-148">要求</span><span class="sxs-lookup"><span data-stu-id="44a7d-148">Request</span></span>
<span data-ttu-id="44a7d-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44a7d-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="44a7d-150">応答</span><span class="sxs-lookup"><span data-stu-id="44a7d-150">Response</span></span>
<span data-ttu-id="44a7d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44a7d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



