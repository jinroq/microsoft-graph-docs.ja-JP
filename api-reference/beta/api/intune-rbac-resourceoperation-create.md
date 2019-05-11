---
title: resourceOperation の作成
description: 新しい resourceOperation オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01fb01eda7710abaa080fca559047022d87fa6f6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899537"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="0c11f-103">resourceOperation の作成</span><span class="sxs-lookup"><span data-stu-id="0c11f-103">Create resourceOperation</span></span>

> <span data-ttu-id="0c11f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c11f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c11f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c11f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c11f-106">新しい [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0c11f-106">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c11f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0c11f-107">Prerequisites</span></span>
<span data-ttu-id="0c11f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c11f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c11f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c11f-110">Permission type</span></span>|<span data-ttu-id="0c11f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c11f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c11f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c11f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c11f-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c11f-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0c11f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c11f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c11f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c11f-115">Not supported.</span></span>|
|<span data-ttu-id="0c11f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c11f-116">Application</span></span>|<span data-ttu-id="0c11f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c11f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c11f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c11f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="0c11f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c11f-119">Request headers</span></span>
|<span data-ttu-id="0c11f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c11f-120">Header</span></span>|<span data-ttu-id="0c11f-121">値</span><span class="sxs-lookup"><span data-stu-id="0c11f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c11f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c11f-122">Authorization</span></span>|<span data-ttu-id="0c11f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c11f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c11f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0c11f-124">Accept</span></span>|<span data-ttu-id="0c11f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c11f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c11f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c11f-126">Request body</span></span>
<span data-ttu-id="0c11f-127">要求本文で、resourceOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c11f-127">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="0c11f-128">次の表に、resourceOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0c11f-128">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="0c11f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c11f-129">Property</span></span>|<span data-ttu-id="0c11f-130">型</span><span class="sxs-lookup"><span data-stu-id="0c11f-130">Type</span></span>|<span data-ttu-id="0c11f-131">説明</span><span class="sxs-lookup"><span data-stu-id="0c11f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c11f-132">id</span><span class="sxs-lookup"><span data-stu-id="0c11f-132">id</span></span>|<span data-ttu-id="0c11f-133">String</span><span class="sxs-lookup"><span data-stu-id="0c11f-133">String</span></span>|<span data-ttu-id="0c11f-134">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="0c11f-134">Key of the Resource Operation.</span></span> <span data-ttu-id="0c11f-135">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="0c11f-135">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="0c11f-136">リソース</span><span class="sxs-lookup"><span data-stu-id="0c11f-136">resource</span></span>|<span data-ttu-id="0c11f-137">String</span><span class="sxs-lookup"><span data-stu-id="0c11f-137">String</span></span>|<span data-ttu-id="0c11f-138">この操作が属するリソースカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="0c11f-138">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="0c11f-139">resourceName</span><span class="sxs-lookup"><span data-stu-id="0c11f-139">resourceName</span></span>|<span data-ttu-id="0c11f-140">String</span><span class="sxs-lookup"><span data-stu-id="0c11f-140">String</span></span>|<span data-ttu-id="0c11f-141">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="0c11f-141">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="0c11f-142">actionName</span><span class="sxs-lookup"><span data-stu-id="0c11f-142">actionName</span></span>|<span data-ttu-id="0c11f-143">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0c11f-143">String</span></span>|<span data-ttu-id="0c11f-144">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="0c11f-144">Type of action this operation is going to perform.</span></span> <span data-ttu-id="0c11f-145">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c11f-145">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="0c11f-146">description</span><span class="sxs-lookup"><span data-stu-id="0c11f-146">description</span></span>|<span data-ttu-id="0c11f-147">String</span><span class="sxs-lookup"><span data-stu-id="0c11f-147">String</span></span>|<span data-ttu-id="0c11f-148">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="0c11f-148">Description of the resource operation.</span></span> <span data-ttu-id="0c11f-149">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="0c11f-149">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="0c11f-150">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="0c11f-150">enabledForScopeValidation</span></span>|<span data-ttu-id="0c11f-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="0c11f-151">Boolean</span></span>|<span data-ttu-id="0c11f-152">権限が役割の割り当てごとに定義されたスコープに対して検証されているかどうかを判断します。</span><span class="sxs-lookup"><span data-stu-id="0c11f-152">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="0c11f-153">応答</span><span class="sxs-lookup"><span data-stu-id="0c11f-153">Response</span></span>
<span data-ttu-id="0c11f-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0c11f-154">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c11f-155">例</span><span class="sxs-lookup"><span data-stu-id="0c11f-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c11f-156">要求</span><span class="sxs-lookup"><span data-stu-id="0c11f-156">Request</span></span>
<span data-ttu-id="0c11f-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c11f-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 249

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```

### <a name="response"></a><span data-ttu-id="0c11f-158">応答</span><span class="sxs-lookup"><span data-stu-id="0c11f-158">Response</span></span>
<span data-ttu-id="0c11f-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c11f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 298

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```




