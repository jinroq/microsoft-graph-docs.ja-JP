---
title: resourceOperation の更新
description: resourceOperation オブジェクトのプロパティを更新します。
ms.openlocfilehash: b89cfb962c6c7f573b4f7f7c6862edd9a66fa833
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073829"
---
# <a name="update-resourceoperation"></a><span data-ttu-id="aee14-103">resourceOperation の更新</span><span class="sxs-lookup"><span data-stu-id="aee14-103">Update resourceOperation</span></span>

> <span data-ttu-id="aee14-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aee14-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aee14-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aee14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="aee14-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aee14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aee14-107">[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aee14-107">Update the properties of a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aee14-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="aee14-108">Prerequisites</span></span>
<span data-ttu-id="aee14-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aee14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aee14-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aee14-111">Permission type</span></span>|<span data-ttu-id="aee14-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aee14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aee14-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aee14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="aee14-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aee14-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="aee14-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aee14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aee14-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aee14-116">Not supported.</span></span>|
|<span data-ttu-id="aee14-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aee14-117">Application</span></span>|<span data-ttu-id="aee14-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aee14-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aee14-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aee14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="aee14-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aee14-120">Request headers</span></span>
|<span data-ttu-id="aee14-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aee14-121">Header</span></span>|<span data-ttu-id="aee14-122">値</span><span class="sxs-lookup"><span data-stu-id="aee14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aee14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="aee14-123">Authorization</span></span>|<span data-ttu-id="aee14-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="aee14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aee14-125">Accept</span><span class="sxs-lookup"><span data-stu-id="aee14-125">Accept</span></span>|<span data-ttu-id="aee14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aee14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aee14-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="aee14-127">Request body</span></span>
<span data-ttu-id="aee14-128">要求本文で、[resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="aee14-128">In the request body, supply a JSON representation for the [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

<span data-ttu-id="aee14-129">次の表に、[resourceOperation](../resources/intune-rbac-resourceoperation.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="aee14-129">The following table shows the properties that are required when you create the [resourceOperation](../resources/intune-rbac-resourceoperation.md).</span></span>

|<span data-ttu-id="aee14-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aee14-130">Property</span></span>|<span data-ttu-id="aee14-131">型</span><span class="sxs-lookup"><span data-stu-id="aee14-131">Type</span></span>|<span data-ttu-id="aee14-132">説明</span><span class="sxs-lookup"><span data-stu-id="aee14-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aee14-133">id</span><span class="sxs-lookup"><span data-stu-id="aee14-133">id</span></span>|<span data-ttu-id="aee14-134">String</span><span class="sxs-lookup"><span data-stu-id="aee14-134">String</span></span>|<span data-ttu-id="aee14-135">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="aee14-135">Key of the Resource Operation.</span></span> <span data-ttu-id="aee14-136">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="aee14-136">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="aee14-137">resource</span><span class="sxs-lookup"><span data-stu-id="aee14-137">resource</span></span>|<span data-ttu-id="aee14-138">String</span><span class="sxs-lookup"><span data-stu-id="aee14-138">String</span></span>|<span data-ttu-id="aee14-139">この操作が所属しているリソースのカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="aee14-139">Resource category to which this Operation belongs.</span></span>|
|<span data-ttu-id="aee14-140">resourceName</span><span class="sxs-lookup"><span data-stu-id="aee14-140">resourceName</span></span>|<span data-ttu-id="aee14-141">String</span><span class="sxs-lookup"><span data-stu-id="aee14-141">String</span></span>|<span data-ttu-id="aee14-142">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="aee14-142">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="aee14-143">actionName</span><span class="sxs-lookup"><span data-stu-id="aee14-143">actionName</span></span>|<span data-ttu-id="aee14-144">String</span><span class="sxs-lookup"><span data-stu-id="aee14-144">String</span></span>|<span data-ttu-id="aee14-145">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="aee14-145">Type of action this operation is going to perform.</span></span> <span data-ttu-id="aee14-146">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="aee14-146">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="aee14-147">説明</span><span class="sxs-lookup"><span data-stu-id="aee14-147">description</span></span>|<span data-ttu-id="aee14-148">String</span><span class="sxs-lookup"><span data-stu-id="aee14-148">String</span></span>|<span data-ttu-id="aee14-149">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="aee14-149">Description of the resource operation.</span></span> <span data-ttu-id="aee14-150">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="aee14-150">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|
|<span data-ttu-id="aee14-151">enabledForScopeValidation</span><span class="sxs-lookup"><span data-stu-id="aee14-151">enabledForScopeValidation</span></span>|<span data-ttu-id="aee14-152">ブール値</span><span class="sxs-lookup"><span data-stu-id="aee14-152">Boolean</span></span>|<span data-ttu-id="aee14-153">ロールの割り当てごとに定義されたスコープのアクセス許可を検証するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="aee14-153">Determines whether the Permission is validated for Scopes defined per Role Assignment.</span></span>|



## <a name="response"></a><span data-ttu-id="aee14-154">応答</span><span class="sxs-lookup"><span data-stu-id="aee14-154">Response</span></span>
<span data-ttu-id="aee14-155">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="aee14-155">If successful, this method returns a `200 OK` response code and an updated [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aee14-156">例</span><span class="sxs-lookup"><span data-stu-id="aee14-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="aee14-157">要求</span><span class="sxs-lookup"><span data-stu-id="aee14-157">Request</span></span>
<span data-ttu-id="aee14-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aee14-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 193

{
  "resource": "Resource value",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value",
  "enabledForScopeValidation": true
}
```

### <a name="response"></a><span data-ttu-id="aee14-159">応答</span><span class="sxs-lookup"><span data-stu-id="aee14-159">Response</span></span>
<span data-ttu-id="aee14-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aee14-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





