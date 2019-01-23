---
title: CartToClassAssociation を作成します。
description: 新しい cartToClassAssociation オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e2368507adbf7e0065b10d4c0c93353d81d5d936
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423672"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="bf8bd-103">CartToClassAssociation を作成します。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="bf8bd-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf8bd-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf8bd-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf8bd-107">新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bf8bd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bf8bd-108">Prerequisites</span></span>
<span data-ttu-id="bf8bd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="bf8bd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bf8bd-111">Permission type</span></span>|<span data-ttu-id="bf8bd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bf8bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf8bd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bf8bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bf8bd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf8bd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="bf8bd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bf8bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf8bd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-116">Not supported.</span></span>|
|<span data-ttu-id="bf8bd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bf8bd-117">Application</span></span>|<span data-ttu-id="bf8bd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bf8bd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bf8bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="bf8bd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf8bd-120">Request headers</span></span>
|<span data-ttu-id="bf8bd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bf8bd-121">Header</span></span>|<span data-ttu-id="bf8bd-122">値</span><span class="sxs-lookup"><span data-stu-id="bf8bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bf8bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf8bd-123">Authorization</span></span>|<span data-ttu-id="bf8bd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bf8bd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="bf8bd-125">Accept</span></span>|<span data-ttu-id="bf8bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf8bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf8bd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="bf8bd-127">Request body</span></span>
<span data-ttu-id="bf8bd-128">要求の本文に cartToClassAssociation オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="bf8bd-129">次の表は、cartToClassAssociation を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="bf8bd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf8bd-130">Property</span></span>|<span data-ttu-id="bf8bd-131">型</span><span class="sxs-lookup"><span data-stu-id="bf8bd-131">Type</span></span>|<span data-ttu-id="bf8bd-132">説明</span><span class="sxs-lookup"><span data-stu-id="bf8bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf8bd-133">id</span><span class="sxs-lookup"><span data-stu-id="bf8bd-133">id</span></span>|<span data-ttu-id="bf8bd-134">String</span><span class="sxs-lookup"><span data-stu-id="bf8bd-134">String</span></span>|<span data-ttu-id="bf8bd-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-135">Key of the entity.</span></span>|
|<span data-ttu-id="bf8bd-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bf8bd-136">createdDateTime</span></span>|<span data-ttu-id="bf8bd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf8bd-137">DateTimeOffset</span></span>|<span data-ttu-id="bf8bd-138">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="bf8bd-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bf8bd-139">lastModifiedDateTime</span></span>|<span data-ttu-id="bf8bd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf8bd-140">DateTimeOffset</span></span>|<span data-ttu-id="bf8bd-141">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="bf8bd-142">version</span><span class="sxs-lookup"><span data-stu-id="bf8bd-142">version</span></span>|<span data-ttu-id="bf8bd-143">Int32</span><span class="sxs-lookup"><span data-stu-id="bf8bd-143">Int32</span></span>|<span data-ttu-id="bf8bd-144">CartToClassAssociation のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="bf8bd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bf8bd-145">displayName</span></span>|<span data-ttu-id="bf8bd-146">String</span><span class="sxs-lookup"><span data-stu-id="bf8bd-146">String</span></span>|<span data-ttu-id="bf8bd-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="bf8bd-148">説明</span><span class="sxs-lookup"><span data-stu-id="bf8bd-148">description</span></span>|<span data-ttu-id="bf8bd-149">String</span><span class="sxs-lookup"><span data-stu-id="bf8bd-149">String</span></span>|<span data-ttu-id="bf8bd-150">管理者には、CartToClassAssociation の説明が用意されています。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="bf8bd-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="bf8bd-151">deviceCartIds</span></span>|<span data-ttu-id="bf8bd-152">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bf8bd-152">String collection</span></span>|<span data-ttu-id="bf8bd-153">クラスに関連するデバイスのカートの識別子です。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="bf8bd-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="bf8bd-154">classroomIds</span></span>|<span data-ttu-id="bf8bd-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bf8bd-155">String collection</span></span>|<span data-ttu-id="bf8bd-156">デバイスのカートに関連する教室の識別子です。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="bf8bd-157">応答</span><span class="sxs-lookup"><span data-stu-id="bf8bd-157">Response</span></span>
<span data-ttu-id="bf8bd-158">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf8bd-159">例</span><span class="sxs-lookup"><span data-stu-id="bf8bd-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf8bd-160">要求</span><span class="sxs-lookup"><span data-stu-id="bf8bd-160">Request</span></span>
<span data-ttu-id="bf8bd-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
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

### <a name="response"></a><span data-ttu-id="bf8bd-162">応答</span><span class="sxs-lookup"><span data-stu-id="bf8bd-162">Response</span></span>
<span data-ttu-id="bf8bd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bf8bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




