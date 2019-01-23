---
title: CartToClassAssociation を更新します。
description: CartToClassAssociation オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8da37fa694c0352ade04c1ae9ce9bca926bc126
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396799"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="5233b-103">CartToClassAssociation を更新します。</span><span class="sxs-lookup"><span data-stu-id="5233b-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="5233b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5233b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5233b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5233b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5233b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5233b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5233b-107">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5233b-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5233b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5233b-108">Prerequisites</span></span>
<span data-ttu-id="5233b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5233b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5233b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5233b-111">Permission type</span></span>|<span data-ttu-id="5233b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5233b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5233b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5233b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5233b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5233b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5233b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5233b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5233b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5233b-116">Not supported.</span></span>|
|<span data-ttu-id="5233b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5233b-117">Application</span></span>|<span data-ttu-id="5233b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5233b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5233b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5233b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="5233b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5233b-120">Request headers</span></span>
|<span data-ttu-id="5233b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5233b-121">Header</span></span>|<span data-ttu-id="5233b-122">値</span><span class="sxs-lookup"><span data-stu-id="5233b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5233b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5233b-123">Authorization</span></span>|<span data-ttu-id="5233b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5233b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5233b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5233b-125">Accept</span></span>|<span data-ttu-id="5233b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5233b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5233b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5233b-127">Request body</span></span>
<span data-ttu-id="5233b-128">要求の本文に[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="5233b-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="5233b-129">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="5233b-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="5233b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5233b-130">Property</span></span>|<span data-ttu-id="5233b-131">型</span><span class="sxs-lookup"><span data-stu-id="5233b-131">Type</span></span>|<span data-ttu-id="5233b-132">説明</span><span class="sxs-lookup"><span data-stu-id="5233b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5233b-133">id</span><span class="sxs-lookup"><span data-stu-id="5233b-133">id</span></span>|<span data-ttu-id="5233b-134">String</span><span class="sxs-lookup"><span data-stu-id="5233b-134">String</span></span>|<span data-ttu-id="5233b-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5233b-135">Key of the entity.</span></span>|
|<span data-ttu-id="5233b-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5233b-136">createdDateTime</span></span>|<span data-ttu-id="5233b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5233b-137">DateTimeOffset</span></span>|<span data-ttu-id="5233b-138">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5233b-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="5233b-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5233b-139">lastModifiedDateTime</span></span>|<span data-ttu-id="5233b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5233b-140">DateTimeOffset</span></span>|<span data-ttu-id="5233b-141">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5233b-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5233b-142">version</span><span class="sxs-lookup"><span data-stu-id="5233b-142">version</span></span>|<span data-ttu-id="5233b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5233b-143">Int32</span></span>|<span data-ttu-id="5233b-144">CartToClassAssociation のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="5233b-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="5233b-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5233b-145">displayName</span></span>|<span data-ttu-id="5233b-146">String</span><span class="sxs-lookup"><span data-stu-id="5233b-146">String</span></span>|<span data-ttu-id="5233b-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="5233b-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="5233b-148">説明</span><span class="sxs-lookup"><span data-stu-id="5233b-148">description</span></span>|<span data-ttu-id="5233b-149">String</span><span class="sxs-lookup"><span data-stu-id="5233b-149">String</span></span>|<span data-ttu-id="5233b-150">管理者には、CartToClassAssociation の説明が用意されています。</span><span class="sxs-lookup"><span data-stu-id="5233b-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="5233b-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="5233b-151">deviceCartIds</span></span>|<span data-ttu-id="5233b-152">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5233b-152">String collection</span></span>|<span data-ttu-id="5233b-153">クラスに関連するデバイスのカートの識別子です。</span><span class="sxs-lookup"><span data-stu-id="5233b-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="5233b-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="5233b-154">classroomIds</span></span>|<span data-ttu-id="5233b-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5233b-155">String collection</span></span>|<span data-ttu-id="5233b-156">デバイスのカートに関連する教室の識別子です。</span><span class="sxs-lookup"><span data-stu-id="5233b-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="5233b-157">応答</span><span class="sxs-lookup"><span data-stu-id="5233b-157">Response</span></span>
<span data-ttu-id="5233b-158">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="5233b-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5233b-159">例</span><span class="sxs-lookup"><span data-stu-id="5233b-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="5233b-160">要求</span><span class="sxs-lookup"><span data-stu-id="5233b-160">Request</span></span>
<span data-ttu-id="5233b-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5233b-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
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

### <a name="response"></a><span data-ttu-id="5233b-162">応答</span><span class="sxs-lookup"><span data-stu-id="5233b-162">Response</span></span>
<span data-ttu-id="5233b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5233b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




