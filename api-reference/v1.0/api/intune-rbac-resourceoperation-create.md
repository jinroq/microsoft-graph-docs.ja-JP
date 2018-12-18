---
title: resourceOperation の作成
description: 新しい resourceOperation オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: f75cfee95b798a38942f70e313f4c18dda7aabe8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328708"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="4a2ab-103">resourceOperation の作成</span><span class="sxs-lookup"><span data-stu-id="4a2ab-103">Create resourceOperation</span></span>

> <span data-ttu-id="4a2ab-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a2ab-105">新しい [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-105">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a2ab-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4a2ab-106">Prerequisites</span></span>
<span data-ttu-id="4a2ab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a2ab-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a2ab-109">Permission type</span></span>|<span data-ttu-id="4a2ab-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a2ab-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a2ab-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a2ab-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4a2ab-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a2ab-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4a2ab-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a2ab-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a2ab-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-114">Not supported.</span></span>|
|<span data-ttu-id="4a2ab-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a2ab-115">Application</span></span>|<span data-ttu-id="4a2ab-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a2ab-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a2ab-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="4a2ab-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a2ab-118">Request headers</span></span>
|<span data-ttu-id="4a2ab-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a2ab-119">Header</span></span>|<span data-ttu-id="4a2ab-120">値</span><span class="sxs-lookup"><span data-stu-id="4a2ab-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a2ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a2ab-121">Authorization</span></span>|<span data-ttu-id="4a2ab-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a2ab-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4a2ab-123">Accept</span></span>|<span data-ttu-id="4a2ab-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4a2ab-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a2ab-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a2ab-125">Request body</span></span>
<span data-ttu-id="4a2ab-126">要求本文で、resourceOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-126">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="4a2ab-127">次の表に、resourceOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-127">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="4a2ab-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4a2ab-128">Property</span></span>|<span data-ttu-id="4a2ab-129">種類</span><span class="sxs-lookup"><span data-stu-id="4a2ab-129">Type</span></span>|<span data-ttu-id="4a2ab-130">説明</span><span class="sxs-lookup"><span data-stu-id="4a2ab-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a2ab-131">ID</span><span class="sxs-lookup"><span data-stu-id="4a2ab-131">id</span></span>|<span data-ttu-id="4a2ab-132">String</span><span class="sxs-lookup"><span data-stu-id="4a2ab-132">String</span></span>|<span data-ttu-id="4a2ab-133">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-133">Key of the Resource Operation.</span></span> <span data-ttu-id="4a2ab-134">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="4a2ab-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="4a2ab-135">resourceName</span></span>|<span data-ttu-id="4a2ab-136">String</span><span class="sxs-lookup"><span data-stu-id="4a2ab-136">String</span></span>|<span data-ttu-id="4a2ab-137">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="4a2ab-138">actionName</span><span class="sxs-lookup"><span data-stu-id="4a2ab-138">actionName</span></span>|<span data-ttu-id="4a2ab-139">String</span><span class="sxs-lookup"><span data-stu-id="4a2ab-139">String</span></span>|<span data-ttu-id="4a2ab-140">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="4a2ab-141">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="4a2ab-142">説明</span><span class="sxs-lookup"><span data-stu-id="4a2ab-142">description</span></span>|<span data-ttu-id="4a2ab-143">String</span><span class="sxs-lookup"><span data-stu-id="4a2ab-143">String</span></span>|<span data-ttu-id="4a2ab-144">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-144">Description of the resource operation.</span></span> <span data-ttu-id="4a2ab-145">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="4a2ab-146">応答</span><span class="sxs-lookup"><span data-stu-id="4a2ab-146">Response</span></span>
<span data-ttu-id="4a2ab-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-147">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a2ab-148">例</span><span class="sxs-lookup"><span data-stu-id="4a2ab-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a2ab-149">要求</span><span class="sxs-lookup"><span data-stu-id="4a2ab-149">Request</span></span>
<span data-ttu-id="4a2ab-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="4a2ab-151">応答</span><span class="sxs-lookup"><span data-stu-id="4a2ab-151">Response</span></span>
<span data-ttu-id="4a2ab-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4a2ab-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```



