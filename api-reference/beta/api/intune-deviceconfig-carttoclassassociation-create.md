---
title: CartToClassAssociation を作成します。
description: 新しい cartToClassAssociation オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 3ed7ef088acca7908ece1e0b5e61797bb54a2e9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330654"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="c6ff5-103">CartToClassAssociation を作成します。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="c6ff5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6ff5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6ff5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6ff5-107">新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6ff5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c6ff5-108">Prerequisites</span></span>
<span data-ttu-id="c6ff5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6ff5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c6ff5-111">Permission type</span></span>|<span data-ttu-id="c6ff5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c6ff5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6ff5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c6ff5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6ff5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6ff5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c6ff5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6ff5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6ff5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-116">Not supported.</span></span>|
|<span data-ttu-id="c6ff5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c6ff5-117">Application</span></span>|<span data-ttu-id="c6ff5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6ff5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6ff5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="c6ff5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6ff5-120">Request headers</span></span>
|<span data-ttu-id="c6ff5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6ff5-121">Header</span></span>|<span data-ttu-id="c6ff5-122">値</span><span class="sxs-lookup"><span data-stu-id="c6ff5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6ff5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6ff5-123">Authorization</span></span>|<span data-ttu-id="c6ff5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6ff5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c6ff5-125">Accept</span></span>|<span data-ttu-id="c6ff5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6ff5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6ff5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c6ff5-127">Request body</span></span>
<span data-ttu-id="c6ff5-128">要求の本文に cartToClassAssociation オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="c6ff5-129">次の表は、cartToClassAssociation を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="c6ff5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c6ff5-130">Property</span></span>|<span data-ttu-id="c6ff5-131">種類</span><span class="sxs-lookup"><span data-stu-id="c6ff5-131">Type</span></span>|<span data-ttu-id="c6ff5-132">説明</span><span class="sxs-lookup"><span data-stu-id="c6ff5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6ff5-133">ID</span><span class="sxs-lookup"><span data-stu-id="c6ff5-133">id</span></span>|<span data-ttu-id="c6ff5-134">String</span><span class="sxs-lookup"><span data-stu-id="c6ff5-134">String</span></span>|<span data-ttu-id="c6ff5-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-135">Key of the entity.</span></span>|
|<span data-ttu-id="c6ff5-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c6ff5-136">createdDateTime</span></span>|<span data-ttu-id="c6ff5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6ff5-137">DateTimeOffset</span></span>|<span data-ttu-id="c6ff5-138">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="c6ff5-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c6ff5-139">lastModifiedDateTime</span></span>|<span data-ttu-id="c6ff5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c6ff5-140">DateTimeOffset</span></span>|<span data-ttu-id="c6ff5-141">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c6ff5-142">version</span><span class="sxs-lookup"><span data-stu-id="c6ff5-142">version</span></span>|<span data-ttu-id="c6ff5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c6ff5-143">Int32</span></span>|<span data-ttu-id="c6ff5-144">CartToClassAssociation のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="c6ff5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c6ff5-145">displayName</span></span>|<span data-ttu-id="c6ff5-146">String</span><span class="sxs-lookup"><span data-stu-id="c6ff5-146">String</span></span>|<span data-ttu-id="c6ff5-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c6ff5-148">説明</span><span class="sxs-lookup"><span data-stu-id="c6ff5-148">description</span></span>|<span data-ttu-id="c6ff5-149">String</span><span class="sxs-lookup"><span data-stu-id="c6ff5-149">String</span></span>|<span data-ttu-id="c6ff5-150">管理者には、CartToClassAssociation の説明が用意されています。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="c6ff5-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="c6ff5-151">deviceCartIds</span></span>|<span data-ttu-id="c6ff5-152">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c6ff5-152">String collection</span></span>|<span data-ttu-id="c6ff5-153">クラスに関連するデバイスのカートの識別子です。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="c6ff5-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="c6ff5-154">classroomIds</span></span>|<span data-ttu-id="c6ff5-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c6ff5-155">String collection</span></span>|<span data-ttu-id="c6ff5-156">デバイスのカートに関連する教室の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="c6ff5-157">応答</span><span class="sxs-lookup"><span data-stu-id="c6ff5-157">Response</span></span>
<span data-ttu-id="c6ff5-158">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6ff5-159">例</span><span class="sxs-lookup"><span data-stu-id="c6ff5-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6ff5-160">要求</span><span class="sxs-lookup"><span data-stu-id="c6ff5-160">Request</span></span>
<span data-ttu-id="c6ff5-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="c6ff5-162">応答</span><span class="sxs-lookup"><span data-stu-id="c6ff5-162">Response</span></span>
<span data-ttu-id="c6ff5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c6ff5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```




