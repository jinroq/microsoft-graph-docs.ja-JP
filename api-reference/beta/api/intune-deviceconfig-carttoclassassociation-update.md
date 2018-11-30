---
title: CartToClassAssociation を更新します。
description: CartToClassAssociation オブジェクトのプロパティを更新します。
ms.openlocfilehash: ecdfdca855920c26e607f24771e41392f74d7095
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071616"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="32def-103">CartToClassAssociation を更新します。</span><span class="sxs-lookup"><span data-stu-id="32def-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="32def-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32def-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32def-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32def-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32def-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="32def-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="32def-107">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="32def-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="32def-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="32def-108">Prerequisites</span></span>
<span data-ttu-id="32def-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32def-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32def-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32def-111">Permission type</span></span>|<span data-ttu-id="32def-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="32def-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32def-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32def-113">Delegated (work or school account)</span></span>|<span data-ttu-id="32def-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32def-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32def-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32def-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32def-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32def-116">Not supported.</span></span>|
|<span data-ttu-id="32def-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32def-117">Application</span></span>|<span data-ttu-id="32def-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32def-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32def-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32def-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="32def-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32def-120">Request headers</span></span>
|<span data-ttu-id="32def-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32def-121">Header</span></span>|<span data-ttu-id="32def-122">値</span><span class="sxs-lookup"><span data-stu-id="32def-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32def-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="32def-123">Authorization</span></span>|<span data-ttu-id="32def-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="32def-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32def-125">Accept</span><span class="sxs-lookup"><span data-stu-id="32def-125">Accept</span></span>|<span data-ttu-id="32def-126">application/json</span><span class="sxs-lookup"><span data-stu-id="32def-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32def-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="32def-127">Request body</span></span>
<span data-ttu-id="32def-128">要求の本文に[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="32def-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="32def-129">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="32def-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="32def-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32def-130">Property</span></span>|<span data-ttu-id="32def-131">型</span><span class="sxs-lookup"><span data-stu-id="32def-131">Type</span></span>|<span data-ttu-id="32def-132">説明</span><span class="sxs-lookup"><span data-stu-id="32def-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32def-133">id</span><span class="sxs-lookup"><span data-stu-id="32def-133">id</span></span>|<span data-ttu-id="32def-134">String</span><span class="sxs-lookup"><span data-stu-id="32def-134">String</span></span>|<span data-ttu-id="32def-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="32def-135">Key of the entity.</span></span>|
|<span data-ttu-id="32def-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32def-136">createdDateTime</span></span>|<span data-ttu-id="32def-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32def-137">DateTimeOffset</span></span>|<span data-ttu-id="32def-138">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="32def-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="32def-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32def-139">lastModifiedDateTime</span></span>|<span data-ttu-id="32def-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32def-140">DateTimeOffset</span></span>|<span data-ttu-id="32def-141">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="32def-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="32def-142">version</span><span class="sxs-lookup"><span data-stu-id="32def-142">version</span></span>|<span data-ttu-id="32def-143">Int32</span><span class="sxs-lookup"><span data-stu-id="32def-143">Int32</span></span>|<span data-ttu-id="32def-144">CartToClassAssociation のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="32def-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="32def-145">displayName</span><span class="sxs-lookup"><span data-stu-id="32def-145">displayName</span></span>|<span data-ttu-id="32def-146">String</span><span class="sxs-lookup"><span data-stu-id="32def-146">String</span></span>|<span data-ttu-id="32def-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="32def-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="32def-148">説明</span><span class="sxs-lookup"><span data-stu-id="32def-148">description</span></span>|<span data-ttu-id="32def-149">String</span><span class="sxs-lookup"><span data-stu-id="32def-149">String</span></span>|<span data-ttu-id="32def-150">管理者には、CartToClassAssociation の説明が用意されています。</span><span class="sxs-lookup"><span data-stu-id="32def-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="32def-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="32def-151">deviceCartIds</span></span>|<span data-ttu-id="32def-152">String コレクション</span><span class="sxs-lookup"><span data-stu-id="32def-152">String collection</span></span>|<span data-ttu-id="32def-153">クラスに関連するデバイスのカートの識別子です。</span><span class="sxs-lookup"><span data-stu-id="32def-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="32def-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="32def-154">classroomIds</span></span>|<span data-ttu-id="32def-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="32def-155">String collection</span></span>|<span data-ttu-id="32def-156">デバイスのカートに関連する教室の識別子です。</span><span class="sxs-lookup"><span data-stu-id="32def-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="32def-157">応答</span><span class="sxs-lookup"><span data-stu-id="32def-157">Response</span></span>
<span data-ttu-id="32def-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="32def-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32def-159">例</span><span class="sxs-lookup"><span data-stu-id="32def-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="32def-160">要求</span><span class="sxs-lookup"><span data-stu-id="32def-160">Request</span></span>
<span data-ttu-id="32def-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32def-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
Content-type: application/json
Content-length: 274

{
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

### <a name="response"></a><span data-ttu-id="32def-162">応答</span><span class="sxs-lookup"><span data-stu-id="32def-162">Response</span></span>
<span data-ttu-id="32def-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32def-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





