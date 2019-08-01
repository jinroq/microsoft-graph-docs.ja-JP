---
title: detectedApp の作成
description: 新しい detectedApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f7f0c88f63c3ff6e2dd3cad8586df6b96625e7b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36021061"
---
# <a name="create-detectedapp"></a><span data-ttu-id="6d4a9-103">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="6d4a9-103">Create detectedApp</span></span>

> <span data-ttu-id="6d4a9-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d4a9-105">新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-105">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d4a9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6d4a9-106">Prerequisites</span></span>
<span data-ttu-id="6d4a9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d4a9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d4a9-109">Permission type</span></span>|<span data-ttu-id="6d4a9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d4a9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d4a9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d4a9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6d4a9-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d4a9-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6d4a9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d4a9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d4a9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-114">Not supported.</span></span>|
|<span data-ttu-id="6d4a9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d4a9-115">Application</span></span>|<span data-ttu-id="6d4a9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d4a9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d4a9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="6d4a9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d4a9-118">Request headers</span></span>
|<span data-ttu-id="6d4a9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d4a9-119">Header</span></span>|<span data-ttu-id="6d4a9-120">値</span><span class="sxs-lookup"><span data-stu-id="6d4a9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d4a9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d4a9-121">Authorization</span></span>|<span data-ttu-id="6d4a9-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d4a9-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6d4a9-123">Accept</span></span>|<span data-ttu-id="6d4a9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6d4a9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d4a9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d4a9-125">Request body</span></span>
<span data-ttu-id="6d4a9-126">要求本文で、detectedApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-126">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="6d4a9-127">次の表に、detectedApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-127">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="6d4a9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6d4a9-128">Property</span></span>|<span data-ttu-id="6d4a9-129">型</span><span class="sxs-lookup"><span data-stu-id="6d4a9-129">Type</span></span>|<span data-ttu-id="6d4a9-130">説明</span><span class="sxs-lookup"><span data-stu-id="6d4a9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d4a9-131">id</span><span class="sxs-lookup"><span data-stu-id="6d4a9-131">id</span></span>|<span data-ttu-id="6d4a9-132">文字列</span><span class="sxs-lookup"><span data-stu-id="6d4a9-132">String</span></span>|<span data-ttu-id="6d4a9-133">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="6d4a9-134">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="6d4a9-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-135">Read-only.</span></span>|
|<span data-ttu-id="6d4a9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6d4a9-136">displayName</span></span>|<span data-ttu-id="6d4a9-137">String</span><span class="sxs-lookup"><span data-stu-id="6d4a9-137">String</span></span>|<span data-ttu-id="6d4a9-138">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-138">Name of the discovered application.</span></span> <span data-ttu-id="6d4a9-139">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="6d4a9-139">Read-only</span></span>|
|<span data-ttu-id="6d4a9-140">version</span><span class="sxs-lookup"><span data-stu-id="6d4a9-140">version</span></span>|<span data-ttu-id="6d4a9-141">String</span><span class="sxs-lookup"><span data-stu-id="6d4a9-141">String</span></span>|<span data-ttu-id="6d4a9-142">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-142">Version of the discovered application.</span></span> <span data-ttu-id="6d4a9-143">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="6d4a9-143">Read-only</span></span>|
|<span data-ttu-id="6d4a9-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="6d4a9-144">sizeInByte</span></span>|<span data-ttu-id="6d4a9-145">Int64</span><span class="sxs-lookup"><span data-stu-id="6d4a9-145">Int64</span></span>|<span data-ttu-id="6d4a9-146">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-146">Discovered application size in bytes.</span></span> <span data-ttu-id="6d4a9-147">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="6d4a9-147">Read-only</span></span>|
|<span data-ttu-id="6d4a9-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="6d4a9-148">deviceCount</span></span>|<span data-ttu-id="6d4a9-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6d4a9-149">Int32</span></span>|<span data-ttu-id="6d4a9-150">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="6d4a9-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="6d4a9-151">応答</span><span class="sxs-lookup"><span data-stu-id="6d4a9-151">Response</span></span>
<span data-ttu-id="6d4a9-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-152">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d4a9-153">例</span><span class="sxs-lookup"><span data-stu-id="6d4a9-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d4a9-154">要求</span><span class="sxs-lookup"><span data-stu-id="6d4a9-154">Request</span></span>
<span data-ttu-id="6d4a9-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/detectedApps
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="6d4a9-156">応答</span><span class="sxs-lookup"><span data-stu-id="6d4a9-156">Response</span></span>
<span data-ttu-id="6d4a9-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6d4a9-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```



