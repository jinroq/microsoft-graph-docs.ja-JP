---
title: resourceOperation の作成
description: 新しい resourceOperation オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be287a5a7f87f38f39f55db7ec505b08b4c3624e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023791"
---
# <a name="create-resourceoperation"></a><span data-ttu-id="d3e7e-103">resourceOperation の作成</span><span class="sxs-lookup"><span data-stu-id="d3e7e-103">Create resourceOperation</span></span>

> <span data-ttu-id="d3e7e-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3e7e-105">新しい [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-105">Create a new [resourceOperation](../resources/intune-rbac-resourceoperation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3e7e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d3e7e-106">Prerequisites</span></span>
<span data-ttu-id="d3e7e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e7e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3e7e-109">Permission type</span></span>|<span data-ttu-id="d3e7e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3e7e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3e7e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3e7e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d3e7e-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e7e-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="d3e7e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3e7e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3e7e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-114">Not supported.</span></span>|
|<span data-ttu-id="d3e7e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3e7e-115">Application</span></span>|<span data-ttu-id="d3e7e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3e7e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3e7e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="d3e7e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3e7e-118">Request headers</span></span>
|<span data-ttu-id="d3e7e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3e7e-119">Header</span></span>|<span data-ttu-id="d3e7e-120">値</span><span class="sxs-lookup"><span data-stu-id="d3e7e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3e7e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3e7e-121">Authorization</span></span>|<span data-ttu-id="d3e7e-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3e7e-123">承諾</span><span class="sxs-lookup"><span data-stu-id="d3e7e-123">Accept</span></span>|<span data-ttu-id="d3e7e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d3e7e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3e7e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3e7e-125">Request body</span></span>
<span data-ttu-id="d3e7e-126">要求本文で、resourceOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-126">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="d3e7e-127">次の表に、resourceOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-127">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="d3e7e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3e7e-128">Property</span></span>|<span data-ttu-id="d3e7e-129">型</span><span class="sxs-lookup"><span data-stu-id="d3e7e-129">Type</span></span>|<span data-ttu-id="d3e7e-130">説明</span><span class="sxs-lookup"><span data-stu-id="d3e7e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3e7e-131">id</span><span class="sxs-lookup"><span data-stu-id="d3e7e-131">id</span></span>|<span data-ttu-id="d3e7e-132">String</span><span class="sxs-lookup"><span data-stu-id="d3e7e-132">String</span></span>|<span data-ttu-id="d3e7e-133">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-133">Key of the Resource Operation.</span></span> <span data-ttu-id="d3e7e-134">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-134">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="d3e7e-135">resourceName</span><span class="sxs-lookup"><span data-stu-id="d3e7e-135">resourceName</span></span>|<span data-ttu-id="d3e7e-136">String</span><span class="sxs-lookup"><span data-stu-id="d3e7e-136">String</span></span>|<span data-ttu-id="d3e7e-137">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-137">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="d3e7e-138">actionName</span><span class="sxs-lookup"><span data-stu-id="d3e7e-138">actionName</span></span>|<span data-ttu-id="d3e7e-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="d3e7e-139">String</span></span>|<span data-ttu-id="d3e7e-140">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-140">Type of action this operation is going to perform.</span></span> <span data-ttu-id="d3e7e-141">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-141">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="d3e7e-142">description</span><span class="sxs-lookup"><span data-stu-id="d3e7e-142">description</span></span>|<span data-ttu-id="d3e7e-143">String</span><span class="sxs-lookup"><span data-stu-id="d3e7e-143">String</span></span>|<span data-ttu-id="d3e7e-144">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-144">Description of the resource operation.</span></span> <span data-ttu-id="d3e7e-145">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-145">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="d3e7e-146">応答</span><span class="sxs-lookup"><span data-stu-id="d3e7e-146">Response</span></span>
<span data-ttu-id="d3e7e-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [resourceOperation](../resources/intune-rbac-resourceoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-147">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune-rbac-resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e7e-148">例</span><span class="sxs-lookup"><span data-stu-id="d3e7e-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3e7e-149">要求</span><span class="sxs-lookup"><span data-stu-id="d3e7e-149">Request</span></span>
<span data-ttu-id="d3e7e-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d3e7e-151">応答</span><span class="sxs-lookup"><span data-stu-id="d3e7e-151">Response</span></span>
<span data-ttu-id="d3e7e-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d3e7e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



