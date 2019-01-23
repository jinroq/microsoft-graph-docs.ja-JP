---
title: resourceOperation の更新
description: resourceOperation オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 266d45150c5633a66c5996b5cb9285f97ecaf6bb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411142"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="bde2a-103">resourceOperation の更新</span><span class="sxs-lookup"><span data-stu-id="bde2a-103">Update resourceOperation</span></span>

> <span data-ttu-id="bde2a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bde2a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bde2a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bde2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bde2a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bde2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bde2a-107">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bde2a-107">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bde2a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bde2a-108">Prerequisites</span></span>
<span data-ttu-id="bde2a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bde2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bde2a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bde2a-111">Permission type</span></span>|<span data-ttu-id="bde2a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bde2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bde2a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bde2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bde2a-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bde2a-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="bde2a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bde2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bde2a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bde2a-116">Not supported.</span></span>|
|<span data-ttu-id="bde2a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bde2a-117">Application</span></span>|<span data-ttu-id="bde2a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bde2a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bde2a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bde2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="bde2a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bde2a-120">Request headers</span></span>
|<span data-ttu-id="bde2a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bde2a-121">Header</span></span>|<span data-ttu-id="bde2a-122">値</span><span class="sxs-lookup"><span data-stu-id="bde2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bde2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bde2a-123">Authorization</span></span>|<span data-ttu-id="bde2a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bde2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bde2a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bde2a-125">Accept</span></span>|<span data-ttu-id="bde2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bde2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bde2a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bde2a-127">Request body</span></span>
<span data-ttu-id="bde2a-128">要求本文で、[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bde2a-128">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="bde2a-129">次の表に、[resourceOperation](../resources/intune-rbac-resourceoperation.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bde2a-129">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="bde2a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bde2a-130">Property</span></span>|<span data-ttu-id="bde2a-131">型</span><span class="sxs-lookup"><span data-stu-id="bde2a-131">Type</span></span>|<span data-ttu-id="bde2a-132">説明</span><span class="sxs-lookup"><span data-stu-id="bde2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bde2a-133">id</span><span class="sxs-lookup"><span data-stu-id="bde2a-133">id</span></span>|<span data-ttu-id="bde2a-134">String</span><span class="sxs-lookup"><span data-stu-id="bde2a-134">String</span></span>|<span data-ttu-id="bde2a-135">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="bde2a-135">Key of the Resource Operation.</span></span> <span data-ttu-id="bde2a-136">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="bde2a-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="bde2a-137">リソース</span><span class="sxs-lookup"><span data-stu-id="bde2a-137">resource</span></span>|<span data-ttu-id="bde2a-138">String</span><span class="sxs-lookup"><span data-stu-id="bde2a-138">String</span></span>|<span data-ttu-id="bde2a-139">この操作が所属しているリソースのカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="bde2a-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="bde2a-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="bde2a-140">resourceName</span></span>|<span data-ttu-id="bde2a-141">String</span><span class="sxs-lookup"><span data-stu-id="bde2a-141">String</span></span>|<span data-ttu-id="bde2a-142">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="bde2a-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="bde2a-143">actionName</span><span class="sxs-lookup"><span data-stu-id="bde2a-143">actionName</span></span>|<span data-ttu-id="bde2a-144">String</span><span class="sxs-lookup"><span data-stu-id="bde2a-144">String</span></span>|<span data-ttu-id="bde2a-145">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="bde2a-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="bde2a-146">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="bde2a-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="bde2a-147">説明</span><span class="sxs-lookup"><span data-stu-id="bde2a-147">description</span></span>|<span data-ttu-id="bde2a-148">String</span><span class="sxs-lookup"><span data-stu-id="bde2a-148">String</span></span>|<span data-ttu-id="bde2a-149">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="bde2a-149">Description of the resource operation.</span></span> <span data-ttu-id="bde2a-150">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="bde2a-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="bde2a-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="bde2a-151">enabledForScopeValidation</span></span>|<span data-ttu-id="bde2a-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="bde2a-152">Boolean</span></span>|<span data-ttu-id="bde2a-153">ロールの割り当てごとに定義されたスコープのアクセス許可を検証するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bde2a-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="bde2a-154">応答</span><span class="sxs-lookup"><span data-stu-id="bde2a-154">Response</span></span>
<span data-ttu-id="bde2a-155">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="bde2a-155">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bde2a-156">例</span><span class="sxs-lookup"><span data-stu-id="bde2a-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="bde2a-157">要求</span><span class="sxs-lookup"><span data-stu-id="bde2a-157">Request</span></span>
<span data-ttu-id="bde2a-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bde2a-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
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

### <a name="response"></a><span data-ttu-id="bde2a-159">応答</span><span class="sxs-lookup"><span data-stu-id="bde2a-159">Response</span></span>
<span data-ttu-id="bde2a-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bde2a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




