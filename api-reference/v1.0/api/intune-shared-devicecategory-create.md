---
title: deviceCategory の作成
description: 新しい deviceCategory オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bd5c0a8285ad2b48f208cd3250dde95ceae82160
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023518"
---
# <a name="create-devicecategory"></a><span data-ttu-id="0ac2e-103">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="0ac2e-103">Create deviceCategory</span></span>

> <span data-ttu-id="0ac2e-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ac2e-105">新しい [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-105">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ac2e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0ac2e-106">Prerequisites</span></span>
<span data-ttu-id="0ac2e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ac2e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ac2e-109">Permission type</span></span>|<span data-ttu-id="0ac2e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ac2e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ac2e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ac2e-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0ac2e-112">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="0ac2e-112">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0ac2e-113">DeviceManagementManaged 対象のデバイス。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-113">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="0ac2e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ac2e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ac2e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-115">Not supported.</span></span>|
|<span data-ttu-id="0ac2e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ac2e-116">Application</span></span>|<span data-ttu-id="0ac2e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ac2e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ac2e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="0ac2e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ac2e-119">Request headers</span></span>
|<span data-ttu-id="0ac2e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ac2e-120">Header</span></span>|<span data-ttu-id="0ac2e-121">値</span><span class="sxs-lookup"><span data-stu-id="0ac2e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ac2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ac2e-122">Authorization</span></span>|<span data-ttu-id="0ac2e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ac2e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0ac2e-124">Accept</span></span>|<span data-ttu-id="0ac2e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ac2e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ac2e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ac2e-126">Request body</span></span>
<span data-ttu-id="0ac2e-127">要求本文で、deviceCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-127">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="0ac2e-128">次の表に、deviceCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-128">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="0ac2e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ac2e-129">Property</span></span>|<span data-ttu-id="0ac2e-130">型</span><span class="sxs-lookup"><span data-stu-id="0ac2e-130">Type</span></span>|<span data-ttu-id="0ac2e-131">説明</span><span class="sxs-lookup"><span data-stu-id="0ac2e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ac2e-132">id</span><span class="sxs-lookup"><span data-stu-id="0ac2e-132">id</span></span>|<span data-ttu-id="0ac2e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0ac2e-133">String</span></span>|<span data-ttu-id="0ac2e-134">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-134">Unique identifier for the device category.</span></span> <span data-ttu-id="0ac2e-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-135">Read-only.</span></span>|
|<span data-ttu-id="0ac2e-136">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="0ac2e-136">**Onboarding**</span></span>|
|<span data-ttu-id="0ac2e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac2e-137">displayName</span></span>|<span data-ttu-id="0ac2e-138">String</span><span class="sxs-lookup"><span data-stu-id="0ac2e-138">String</span></span>|<span data-ttu-id="0ac2e-139">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-139">Display name for the device category.</span></span>|
|<span data-ttu-id="0ac2e-140">description</span><span class="sxs-lookup"><span data-stu-id="0ac2e-140">description</span></span>|<span data-ttu-id="0ac2e-141">String</span><span class="sxs-lookup"><span data-stu-id="0ac2e-141">String</span></span>|<span data-ttu-id="0ac2e-142">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-142">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="0ac2e-143">応答</span><span class="sxs-lookup"><span data-stu-id="0ac2e-143">Response</span></span>
<span data-ttu-id="0ac2e-144">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-144">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac2e-145">例</span><span class="sxs-lookup"><span data-stu-id="0ac2e-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ac2e-146">要求</span><span class="sxs-lookup"><span data-stu-id="0ac2e-146">Request</span></span>
<span data-ttu-id="0ac2e-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="0ac2e-148">応答</span><span class="sxs-lookup"><span data-stu-id="0ac2e-148">Response</span></span>
<span data-ttu-id="0ac2e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ac2e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



