---
title: RoleScopeTag を作成します。
description: 新しい roleScopeTag オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 61476fa106661baa179ff5344b8e4ac891b5a3b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422195"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="f4fc9-103">RoleScopeTag を作成します。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-103">Create roleScopeTag</span></span>

> <span data-ttu-id="f4fc9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f4fc9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4fc9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f4fc9-107">新しい[roleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-107">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f4fc9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f4fc9-108">Prerequisites</span></span>
<span data-ttu-id="f4fc9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f4fc9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4fc9-111">Permission type</span></span>|<span data-ttu-id="f4fc9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4fc9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4fc9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4fc9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4fc9-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4fc9-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="f4fc9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4fc9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4fc9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-116">Not supported.</span></span>|
|<span data-ttu-id="f4fc9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4fc9-117">Application</span></span>|<span data-ttu-id="f4fc9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4fc9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4fc9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="f4fc9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4fc9-120">Request headers</span></span>
|<span data-ttu-id="f4fc9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4fc9-121">Header</span></span>|<span data-ttu-id="f4fc9-122">値</span><span class="sxs-lookup"><span data-stu-id="f4fc9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4fc9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4fc9-123">Authorization</span></span>|<span data-ttu-id="f4fc9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4fc9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4fc9-125">Accept</span></span>|<span data-ttu-id="f4fc9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4fc9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4fc9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4fc9-127">Request body</span></span>
<span data-ttu-id="f4fc9-128">要求の本文に roleScopeTag オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-128">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="f4fc9-129">次の表は、roleScopeTag を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-129">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="f4fc9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4fc9-130">Property</span></span>|<span data-ttu-id="f4fc9-131">型</span><span class="sxs-lookup"><span data-stu-id="f4fc9-131">Type</span></span>|<span data-ttu-id="f4fc9-132">説明</span><span class="sxs-lookup"><span data-stu-id="f4fc9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4fc9-133">id</span><span class="sxs-lookup"><span data-stu-id="f4fc9-133">id</span></span>|<span data-ttu-id="f4fc9-134">String</span><span class="sxs-lookup"><span data-stu-id="f4fc9-134">String</span></span>|<span data-ttu-id="f4fc9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-135">Key of the entity.</span></span> <span data-ttu-id="f4fc9-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="f4fc9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f4fc9-137">displayName</span></span>|<span data-ttu-id="f4fc9-138">String</span><span class="sxs-lookup"><span data-stu-id="f4fc9-138">String</span></span>|<span data-ttu-id="f4fc9-139">表示する、またはロールのスコープのタグの表示名。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="f4fc9-140">説明</span><span class="sxs-lookup"><span data-stu-id="f4fc9-140">description</span></span>|<span data-ttu-id="f4fc9-141">String</span><span class="sxs-lookup"><span data-stu-id="f4fc9-141">String</span></span>|<span data-ttu-id="f4fc9-142">ロールのスコープのタグの説明です。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="f4fc9-143">応答</span><span class="sxs-lookup"><span data-stu-id="f4fc9-143">Response</span></span>
<span data-ttu-id="f4fc9-144">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[roleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-144">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4fc9-145">例</span><span class="sxs-lookup"><span data-stu-id="f4fc9-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="f4fc9-146">要求</span><span class="sxs-lookup"><span data-stu-id="f4fc9-146">Request</span></span>
<span data-ttu-id="f4fc9-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="f4fc9-148">応答</span><span class="sxs-lookup"><span data-stu-id="f4fc9-148">Response</span></span>
<span data-ttu-id="f4fc9-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4fc9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```




