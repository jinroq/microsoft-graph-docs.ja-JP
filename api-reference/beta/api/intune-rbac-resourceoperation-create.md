---
title: resourceOperation の作成
description: 新しい resourceOperation オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b9825d344f51eb1945f5a261cc660e0234edef87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422573"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="9e220-103">resourceOperation の作成</span><span class="sxs-lookup"><span data-stu-id="9e220-103">Create resourceOperation</span></span>

> <span data-ttu-id="9e220-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e220-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e220-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e220-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e220-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e220-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e220-107">新しい [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9e220-107">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e220-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e220-108">Prerequisites</span></span>
<span data-ttu-id="9e220-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e220-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9e220-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e220-111">Permission type</span></span>|<span data-ttu-id="9e220-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e220-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e220-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e220-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e220-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e220-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="9e220-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e220-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e220-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e220-116">Not supported.</span></span>|
|<span data-ttu-id="9e220-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e220-117">Application</span></span>|<span data-ttu-id="9e220-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e220-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e220-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e220-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="9e220-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e220-120">Request headers</span></span>
|<span data-ttu-id="9e220-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e220-121">Header</span></span>|<span data-ttu-id="9e220-122">値</span><span class="sxs-lookup"><span data-stu-id="9e220-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e220-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e220-123">Authorization</span></span>|<span data-ttu-id="9e220-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9e220-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e220-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e220-125">Accept</span></span>|<span data-ttu-id="9e220-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e220-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e220-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e220-127">Request body</span></span>
<span data-ttu-id="9e220-128">要求本文で、resourceOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e220-128">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="9e220-129">次の表に、resourceOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9e220-129">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="9e220-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e220-130">Property</span></span>|<span data-ttu-id="9e220-131">型</span><span class="sxs-lookup"><span data-stu-id="9e220-131">Type</span></span>|<span data-ttu-id="9e220-132">説明</span><span class="sxs-lookup"><span data-stu-id="9e220-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e220-133">id</span><span class="sxs-lookup"><span data-stu-id="9e220-133">id</span></span>|<span data-ttu-id="9e220-134">String</span><span class="sxs-lookup"><span data-stu-id="9e220-134">String</span></span>|<span data-ttu-id="9e220-135">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="9e220-135">Key of the Resource Operation.</span></span> <span data-ttu-id="9e220-136">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="9e220-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="9e220-137">リソース</span><span class="sxs-lookup"><span data-stu-id="9e220-137">resource</span></span>|<span data-ttu-id="9e220-138">String</span><span class="sxs-lookup"><span data-stu-id="9e220-138">String</span></span>|<span data-ttu-id="9e220-139">この操作が所属しているリソースのカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="9e220-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="9e220-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="9e220-140">resourceName</span></span>|<span data-ttu-id="9e220-141">String</span><span class="sxs-lookup"><span data-stu-id="9e220-141">String</span></span>|<span data-ttu-id="9e220-142">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="9e220-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="9e220-143">actionName</span><span class="sxs-lookup"><span data-stu-id="9e220-143">actionName</span></span>|<span data-ttu-id="9e220-144">String</span><span class="sxs-lookup"><span data-stu-id="9e220-144">String</span></span>|<span data-ttu-id="9e220-145">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="9e220-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="9e220-146">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e220-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="9e220-147">説明</span><span class="sxs-lookup"><span data-stu-id="9e220-147">description</span></span>|<span data-ttu-id="9e220-148">String</span><span class="sxs-lookup"><span data-stu-id="9e220-148">String</span></span>|<span data-ttu-id="9e220-149">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="9e220-149">Description of the resource operation.</span></span> <span data-ttu-id="9e220-150">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="9e220-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="9e220-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="9e220-151">enabledForScopeValidation</span></span>|<span data-ttu-id="9e220-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e220-152">Boolean</span></span>|<span data-ttu-id="9e220-153">ロールの割り当てごとに定義されたスコープのアクセス許可を検証するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="9e220-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="9e220-154">応答</span><span class="sxs-lookup"><span data-stu-id="9e220-154">Response</span></span>
<span data-ttu-id="9e220-155">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9e220-155">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e220-156">例</span><span class="sxs-lookup"><span data-stu-id="9e220-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e220-157">要求</span><span class="sxs-lookup"><span data-stu-id="9e220-157">Request</span></span>
<span data-ttu-id="9e220-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e220-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9e220-159">応答</span><span class="sxs-lookup"><span data-stu-id="9e220-159">Response</span></span>
<span data-ttu-id="9e220-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e220-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




