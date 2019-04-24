---
title: cartToClassAssociation を作成する
description: 新しい cartToClassAssociation オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c683b2ae19caa55c62f0af834fbb8b74d5fb904c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32471582"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="e72b5-103">cartToClassAssociation を作成する</span><span class="sxs-lookup"><span data-stu-id="e72b5-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="e72b5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e72b5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e72b5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e72b5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e72b5-106">新しい[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e72b5-106">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e72b5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e72b5-107">Prerequisites</span></span>
<span data-ttu-id="e72b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e72b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e72b5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e72b5-110">Permission type</span></span>|<span data-ttu-id="e72b5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e72b5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e72b5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e72b5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e72b5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e72b5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e72b5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e72b5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e72b5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e72b5-115">Not supported.</span></span>|
|<span data-ttu-id="e72b5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e72b5-116">Application</span></span>|<span data-ttu-id="e72b5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e72b5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e72b5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e72b5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="e72b5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e72b5-119">Request headers</span></span>
|<span data-ttu-id="e72b5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e72b5-120">Header</span></span>|<span data-ttu-id="e72b5-121">値</span><span class="sxs-lookup"><span data-stu-id="e72b5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e72b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e72b5-122">Authorization</span></span>|<span data-ttu-id="e72b5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e72b5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e72b5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e72b5-124">Accept</span></span>|<span data-ttu-id="e72b5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e72b5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e72b5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e72b5-126">Request body</span></span>
<span data-ttu-id="e72b5-127">要求本文で、cartToClassAssociation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e72b5-127">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="e72b5-128">次の表に、cartToClassAssociation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e72b5-128">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="e72b5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e72b5-129">Property</span></span>|<span data-ttu-id="e72b5-130">型</span><span class="sxs-lookup"><span data-stu-id="e72b5-130">Type</span></span>|<span data-ttu-id="e72b5-131">説明</span><span class="sxs-lookup"><span data-stu-id="e72b5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e72b5-132">id</span><span class="sxs-lookup"><span data-stu-id="e72b5-132">id</span></span>|<span data-ttu-id="e72b5-133">String</span><span class="sxs-lookup"><span data-stu-id="e72b5-133">String</span></span>|<span data-ttu-id="e72b5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e72b5-134">Key of the entity.</span></span>|
|<span data-ttu-id="e72b5-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e72b5-135">createdDateTime</span></span>|<span data-ttu-id="e72b5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e72b5-136">DateTimeOffset</span></span>|<span data-ttu-id="e72b5-137">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e72b5-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="e72b5-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e72b5-138">lastModifiedDateTime</span></span>|<span data-ttu-id="e72b5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e72b5-139">DateTimeOffset</span></span>|<span data-ttu-id="e72b5-140">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e72b5-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e72b5-141">version</span><span class="sxs-lookup"><span data-stu-id="e72b5-141">version</span></span>|<span data-ttu-id="e72b5-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e72b5-142">Int32</span></span>|<span data-ttu-id="e72b5-143">CartToClassAssociation のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e72b5-143">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="e72b5-144">displayName</span><span class="sxs-lookup"><span data-stu-id="e72b5-144">displayName</span></span>|<span data-ttu-id="e72b5-145">String</span><span class="sxs-lookup"><span data-stu-id="e72b5-145">String</span></span>|<span data-ttu-id="e72b5-146">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e72b5-146">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="e72b5-147">説明</span><span class="sxs-lookup"><span data-stu-id="e72b5-147">description</span></span>|<span data-ttu-id="e72b5-148">String</span><span class="sxs-lookup"><span data-stu-id="e72b5-148">String</span></span>|<span data-ttu-id="e72b5-149">CartToClassAssociation の管理者提供の説明。</span><span class="sxs-lookup"><span data-stu-id="e72b5-149">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="e72b5-150">devicecartids</span><span class="sxs-lookup"><span data-stu-id="e72b5-150">deviceCartIds</span></span>|<span data-ttu-id="e72b5-151">String collection</span><span class="sxs-lookup"><span data-stu-id="e72b5-151">String collection</span></span>|<span data-ttu-id="e72b5-152">クラスに関連付けられるデバイスカートの識別子。</span><span class="sxs-lookup"><span data-stu-id="e72b5-152">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="e72b5-153">classroomIds</span><span class="sxs-lookup"><span data-stu-id="e72b5-153">classroomIds</span></span>|<span data-ttu-id="e72b5-154">String collection</span><span class="sxs-lookup"><span data-stu-id="e72b5-154">String collection</span></span>|<span data-ttu-id="e72b5-155">デバイスカートに関連付ける教室の識別子。</span><span class="sxs-lookup"><span data-stu-id="e72b5-155">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="e72b5-156">応答</span><span class="sxs-lookup"><span data-stu-id="e72b5-156">Response</span></span>
<span data-ttu-id="e72b5-157">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e72b5-157">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e72b5-158">例</span><span class="sxs-lookup"><span data-stu-id="e72b5-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="e72b5-159">要求</span><span class="sxs-lookup"><span data-stu-id="e72b5-159">Request</span></span>
<span data-ttu-id="e72b5-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e72b5-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e72b5-161">応答</span><span class="sxs-lookup"><span data-stu-id="e72b5-161">Response</span></span>
<span data-ttu-id="e72b5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e72b5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





