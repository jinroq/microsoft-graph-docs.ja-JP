---
title: cartToClassAssociation の更新
description: cartToClassAssociation オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09e83b523145f79d610b1299d61fafc5d0a03b02
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30964480"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="4e192-103">cartToClassAssociation の更新</span><span class="sxs-lookup"><span data-stu-id="4e192-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="4e192-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e192-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4e192-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e192-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e192-106">[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4e192-106">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e192-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4e192-107">Prerequisites</span></span>
<span data-ttu-id="4e192-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e192-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e192-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e192-110">Permission type</span></span>|<span data-ttu-id="4e192-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e192-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e192-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e192-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4e192-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e192-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4e192-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e192-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e192-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e192-115">Not supported.</span></span>|
|<span data-ttu-id="4e192-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e192-116">Application</span></span>|<span data-ttu-id="4e192-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e192-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e192-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e192-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="4e192-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e192-119">Request headers</span></span>
|<span data-ttu-id="4e192-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e192-120">Header</span></span>|<span data-ttu-id="4e192-121">値</span><span class="sxs-lookup"><span data-stu-id="4e192-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e192-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e192-122">Authorization</span></span>|<span data-ttu-id="4e192-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e192-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e192-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4e192-124">Accept</span></span>|<span data-ttu-id="4e192-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4e192-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e192-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e192-126">Request body</span></span>
<span data-ttu-id="4e192-127">要求本文で、 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e192-127">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="4e192-128">次の表に、 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4e192-128">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="4e192-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e192-129">Property</span></span>|<span data-ttu-id="4e192-130">型</span><span class="sxs-lookup"><span data-stu-id="4e192-130">Type</span></span>|<span data-ttu-id="4e192-131">説明</span><span class="sxs-lookup"><span data-stu-id="4e192-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e192-132">id</span><span class="sxs-lookup"><span data-stu-id="4e192-132">id</span></span>|<span data-ttu-id="4e192-133">String</span><span class="sxs-lookup"><span data-stu-id="4e192-133">String</span></span>|<span data-ttu-id="4e192-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4e192-134">Key of the entity.</span></span>|
|<span data-ttu-id="4e192-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4e192-135">createdDateTime</span></span>|<span data-ttu-id="4e192-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e192-136">DateTimeOffset</span></span>|<span data-ttu-id="4e192-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4e192-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="4e192-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4e192-138">lastModifiedDateTime</span></span>|<span data-ttu-id="4e192-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4e192-139">DateTimeOffset</span></span>|<span data-ttu-id="4e192-140">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="4e192-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="4e192-141">version</span><span class="sxs-lookup"><span data-stu-id="4e192-141">version</span></span>|<span data-ttu-id="4e192-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4e192-142">Int32</span></span>|<span data-ttu-id="4e192-143">CartToClassAssociation のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4e192-143">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="4e192-144">displayName</span><span class="sxs-lookup"><span data-stu-id="4e192-144">displayName</span></span>|<span data-ttu-id="4e192-145">String</span><span class="sxs-lookup"><span data-stu-id="4e192-145">String</span></span>|<span data-ttu-id="4e192-146">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="4e192-146">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="4e192-147">description</span><span class="sxs-lookup"><span data-stu-id="4e192-147">description</span></span>|<span data-ttu-id="4e192-148">String</span><span class="sxs-lookup"><span data-stu-id="4e192-148">String</span></span>|<span data-ttu-id="4e192-149">CartToClassAssociation の管理者提供の説明。</span><span class="sxs-lookup"><span data-stu-id="4e192-149">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="4e192-150">devicecartids</span><span class="sxs-lookup"><span data-stu-id="4e192-150">deviceCartIds</span></span>|<span data-ttu-id="4e192-151">String collection</span><span class="sxs-lookup"><span data-stu-id="4e192-151">String collection</span></span>|<span data-ttu-id="4e192-152">クラスに関連付けられるデバイスカートの識別子。</span><span class="sxs-lookup"><span data-stu-id="4e192-152">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="4e192-153">classroomIds</span><span class="sxs-lookup"><span data-stu-id="4e192-153">classroomIds</span></span>|<span data-ttu-id="4e192-154">String collection</span><span class="sxs-lookup"><span data-stu-id="4e192-154">String collection</span></span>|<span data-ttu-id="4e192-155">デバイスカートに関連付ける教室の識別子。</span><span class="sxs-lookup"><span data-stu-id="4e192-155">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="4e192-156">応答</span><span class="sxs-lookup"><span data-stu-id="4e192-156">Response</span></span>
<span data-ttu-id="4e192-157">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4e192-157">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e192-158">例</span><span class="sxs-lookup"><span data-stu-id="4e192-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e192-159">要求</span><span class="sxs-lookup"><span data-stu-id="4e192-159">Request</span></span>
<span data-ttu-id="4e192-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e192-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4e192-161">応答</span><span class="sxs-lookup"><span data-stu-id="4e192-161">Response</span></span>
<span data-ttu-id="4e192-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4e192-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




