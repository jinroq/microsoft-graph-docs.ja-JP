---
title: CartToClassAssociation の更新
description: CartToClassAssociation オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4acc9f2a94857e9929d48884bb3620cf04557a7c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36340374"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="d4e53-103">CartToClassAssociation の更新</span><span class="sxs-lookup"><span data-stu-id="d4e53-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="d4e53-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4e53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4e53-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4e53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4e53-106">[CartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d4e53-106">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4e53-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4e53-107">Prerequisites</span></span>
<span data-ttu-id="d4e53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e53-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4e53-110">Permission type</span></span>|<span data-ttu-id="d4e53-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4e53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4e53-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4e53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4e53-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e53-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d4e53-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4e53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4e53-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4e53-115">Not supported.</span></span>|
|<span data-ttu-id="d4e53-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4e53-116">Application</span></span>|<span data-ttu-id="d4e53-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e53-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4e53-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4e53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="d4e53-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4e53-119">Request headers</span></span>
|<span data-ttu-id="d4e53-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4e53-120">Header</span></span>|<span data-ttu-id="d4e53-121">値</span><span class="sxs-lookup"><span data-stu-id="d4e53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4e53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4e53-122">Authorization</span></span>|<span data-ttu-id="d4e53-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4e53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4e53-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d4e53-124">Accept</span></span>|<span data-ttu-id="d4e53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4e53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4e53-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4e53-126">Request body</span></span>
<span data-ttu-id="d4e53-127">要求本文で、 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d4e53-127">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="d4e53-128">次の表に、 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d4e53-128">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="d4e53-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4e53-129">Property</span></span>|<span data-ttu-id="d4e53-130">型</span><span class="sxs-lookup"><span data-stu-id="d4e53-130">Type</span></span>|<span data-ttu-id="d4e53-131">説明</span><span class="sxs-lookup"><span data-stu-id="d4e53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4e53-132">id</span><span class="sxs-lookup"><span data-stu-id="d4e53-132">id</span></span>|<span data-ttu-id="d4e53-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d4e53-133">String</span></span>|<span data-ttu-id="d4e53-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d4e53-134">Key of the entity.</span></span>|
|<span data-ttu-id="d4e53-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e53-135">createdDateTime</span></span>|<span data-ttu-id="d4e53-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e53-136">DateTimeOffset</span></span>|<span data-ttu-id="d4e53-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d4e53-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="d4e53-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4e53-138">lastModifiedDateTime</span></span>|<span data-ttu-id="d4e53-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4e53-139">DateTimeOffset</span></span>|<span data-ttu-id="d4e53-140">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d4e53-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d4e53-141">version</span><span class="sxs-lookup"><span data-stu-id="d4e53-141">version</span></span>|<span data-ttu-id="d4e53-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d4e53-142">Int32</span></span>|<span data-ttu-id="d4e53-143">CartToClassAssociation のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d4e53-143">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="d4e53-144">displayName</span><span class="sxs-lookup"><span data-stu-id="d4e53-144">displayName</span></span>|<span data-ttu-id="d4e53-145">String</span><span class="sxs-lookup"><span data-stu-id="d4e53-145">String</span></span>|<span data-ttu-id="d4e53-146">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="d4e53-146">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="d4e53-147">description</span><span class="sxs-lookup"><span data-stu-id="d4e53-147">description</span></span>|<span data-ttu-id="d4e53-148">String</span><span class="sxs-lookup"><span data-stu-id="d4e53-148">String</span></span>|<span data-ttu-id="d4e53-149">CartToClassAssociation の管理者提供の説明。</span><span class="sxs-lookup"><span data-stu-id="d4e53-149">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="d4e53-150">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="d4e53-150">deviceCartIds</span></span>|<span data-ttu-id="d4e53-151">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d4e53-151">String collection</span></span>|<span data-ttu-id="d4e53-152">クラスに関連付けられるデバイスカートの識別子。</span><span class="sxs-lookup"><span data-stu-id="d4e53-152">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="d4e53-153">classroomIds</span><span class="sxs-lookup"><span data-stu-id="d4e53-153">classroomIds</span></span>|<span data-ttu-id="d4e53-154">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d4e53-154">String collection</span></span>|<span data-ttu-id="d4e53-155">デバイスカートに関連付ける教室の識別子。</span><span class="sxs-lookup"><span data-stu-id="d4e53-155">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="d4e53-156">応答</span><span class="sxs-lookup"><span data-stu-id="d4e53-156">Response</span></span>
<span data-ttu-id="d4e53-157">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d4e53-157">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4e53-158">例</span><span class="sxs-lookup"><span data-stu-id="d4e53-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4e53-159">要求</span><span class="sxs-lookup"><span data-stu-id="d4e53-159">Request</span></span>
<span data-ttu-id="d4e53-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4e53-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d4e53-161">応答</span><span class="sxs-lookup"><span data-stu-id="d4e53-161">Response</span></span>
<span data-ttu-id="d4e53-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4e53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






