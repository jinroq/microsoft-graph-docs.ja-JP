---
title: detectedApp の更新
description: detectedApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 68572281eab1d1449a3d855ebd3e9563adb3bd46
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926548"
---
# <a name="update-detectedapp"></a><span data-ttu-id="b58ca-103">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="b58ca-103">Update detectedApp</span></span>

> <span data-ttu-id="b58ca-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b58ca-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b58ca-105">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b58ca-105">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b58ca-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b58ca-106">Prerequisites</span></span>
<span data-ttu-id="b58ca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b58ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b58ca-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b58ca-109">Permission type</span></span>|<span data-ttu-id="b58ca-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b58ca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b58ca-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b58ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b58ca-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b58ca-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b58ca-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b58ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b58ca-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b58ca-114">Not supported.</span></span>|
|<span data-ttu-id="b58ca-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b58ca-115">Application</span></span>|<span data-ttu-id="b58ca-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b58ca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b58ca-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b58ca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b58ca-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b58ca-118">Request headers</span></span>
|<span data-ttu-id="b58ca-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b58ca-119">Header</span></span>|<span data-ttu-id="b58ca-120">値</span><span class="sxs-lookup"><span data-stu-id="b58ca-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b58ca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b58ca-121">Authorization</span></span>|<span data-ttu-id="b58ca-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b58ca-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b58ca-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b58ca-123">Accept</span></span>|<span data-ttu-id="b58ca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b58ca-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b58ca-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b58ca-125">Request body</span></span>
<span data-ttu-id="b58ca-126">要求本文で、[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b58ca-126">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="b58ca-127">次の表に、[detectedApp](../resources/intune-devices-detectedapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b58ca-127">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="b58ca-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b58ca-128">Property</span></span>|<span data-ttu-id="b58ca-129">種類</span><span class="sxs-lookup"><span data-stu-id="b58ca-129">Type</span></span>|<span data-ttu-id="b58ca-130">説明</span><span class="sxs-lookup"><span data-stu-id="b58ca-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b58ca-131">ID</span><span class="sxs-lookup"><span data-stu-id="b58ca-131">id</span></span>|<span data-ttu-id="b58ca-132">String</span><span class="sxs-lookup"><span data-stu-id="b58ca-132">String</span></span>|<span data-ttu-id="b58ca-133">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b58ca-133">The unique Identifier for the detected application.</span></span> <span data-ttu-id="b58ca-134">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="b58ca-134">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="b58ca-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b58ca-135">Read-only.</span></span>|
|<span data-ttu-id="b58ca-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b58ca-136">displayName</span></span>|<span data-ttu-id="b58ca-137">String</span><span class="sxs-lookup"><span data-stu-id="b58ca-137">String</span></span>|<span data-ttu-id="b58ca-138">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="b58ca-138">Name of the discovered application.</span></span> <span data-ttu-id="b58ca-139">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="b58ca-139">Read-only</span></span>|
|<span data-ttu-id="b58ca-140">version</span><span class="sxs-lookup"><span data-stu-id="b58ca-140">version</span></span>|<span data-ttu-id="b58ca-141">String</span><span class="sxs-lookup"><span data-stu-id="b58ca-141">String</span></span>|<span data-ttu-id="b58ca-142">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b58ca-142">Version of the discovered application.</span></span> <span data-ttu-id="b58ca-143">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="b58ca-143">Read-only</span></span>|
|<span data-ttu-id="b58ca-144">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="b58ca-144">sizeInByte</span></span>|<span data-ttu-id="b58ca-145">Int64</span><span class="sxs-lookup"><span data-stu-id="b58ca-145">Int64</span></span>|<span data-ttu-id="b58ca-146">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="b58ca-146">Discovered application size in bytes.</span></span> <span data-ttu-id="b58ca-147">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="b58ca-147">Read-only</span></span>|
|<span data-ttu-id="b58ca-148">deviceCount</span><span class="sxs-lookup"><span data-stu-id="b58ca-148">deviceCount</span></span>|<span data-ttu-id="b58ca-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b58ca-149">Int32</span></span>|<span data-ttu-id="b58ca-150">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="b58ca-150">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="b58ca-151">応答</span><span class="sxs-lookup"><span data-stu-id="b58ca-151">Response</span></span>
<span data-ttu-id="b58ca-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b58ca-152">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b58ca-153">例</span><span class="sxs-lookup"><span data-stu-id="b58ca-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="b58ca-154">要求</span><span class="sxs-lookup"><span data-stu-id="b58ca-154">Request</span></span>
<span data-ttu-id="b58ca-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b58ca-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
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

### <a name="response"></a><span data-ttu-id="b58ca-156">応答</span><span class="sxs-lookup"><span data-stu-id="b58ca-156">Response</span></span>
<span data-ttu-id="b58ca-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b58ca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



