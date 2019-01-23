---
title: detectedApp の更新
description: detectedApp オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7bfea341aafb25ea010162d270eab451900c0d04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394944"
---
# <a name="update-detectedapp"></a><span data-ttu-id="c8990-103">detectedApp の更新</span><span class="sxs-lookup"><span data-stu-id="c8990-103">Update detectedApp</span></span>

> <span data-ttu-id="c8990-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8990-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c8990-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8990-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8990-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c8990-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8990-107">[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c8990-107">Update the properties of a [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8990-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8990-108">Prerequisites</span></span>
<span data-ttu-id="c8990-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8990-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c8990-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8990-111">Permission type</span></span>|<span data-ttu-id="c8990-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8990-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8990-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8990-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8990-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8990-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="c8990-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8990-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8990-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8990-116">Not supported.</span></span>|
|<span data-ttu-id="c8990-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8990-117">Application</span></span>|<span data-ttu-id="c8990-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8990-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8990-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8990-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="c8990-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8990-120">Request headers</span></span>
|<span data-ttu-id="c8990-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8990-121">Header</span></span>|<span data-ttu-id="c8990-122">値</span><span class="sxs-lookup"><span data-stu-id="c8990-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8990-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8990-123">Authorization</span></span>|<span data-ttu-id="c8990-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c8990-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8990-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8990-125">Accept</span></span>|<span data-ttu-id="c8990-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8990-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8990-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8990-127">Request body</span></span>
<span data-ttu-id="c8990-128">要求本文で、[detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8990-128">In the request body, supply a JSON representation for the [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

<span data-ttu-id="c8990-129">次の表に、[detectedApp](../resources/intune-devices-detectedapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c8990-129">The following table shows the properties that are required when you create the [detectedApp](../resources/intune-devices-detectedapp.md).</span></span>

|<span data-ttu-id="c8990-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8990-130">Property</span></span>|<span data-ttu-id="c8990-131">型</span><span class="sxs-lookup"><span data-stu-id="c8990-131">Type</span></span>|<span data-ttu-id="c8990-132">説明</span><span class="sxs-lookup"><span data-stu-id="c8990-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8990-133">id</span><span class="sxs-lookup"><span data-stu-id="c8990-133">id</span></span>|<span data-ttu-id="c8990-134">String</span><span class="sxs-lookup"><span data-stu-id="c8990-134">String</span></span>|<span data-ttu-id="c8990-135">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="c8990-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="c8990-136">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="c8990-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="c8990-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c8990-137">Read-only.</span></span>|
|<span data-ttu-id="c8990-138">displayName</span><span class="sxs-lookup"><span data-stu-id="c8990-138">displayName</span></span>|<span data-ttu-id="c8990-139">String</span><span class="sxs-lookup"><span data-stu-id="c8990-139">String</span></span>|<span data-ttu-id="c8990-140">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="c8990-140">Name of the discovered application.</span></span> <span data-ttu-id="c8990-141">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="c8990-141">Read-only</span></span>|
|<span data-ttu-id="c8990-142">version</span><span class="sxs-lookup"><span data-stu-id="c8990-142">version</span></span>|<span data-ttu-id="c8990-143">String</span><span class="sxs-lookup"><span data-stu-id="c8990-143">String</span></span>|<span data-ttu-id="c8990-144">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c8990-144">Version of the discovered application.</span></span> <span data-ttu-id="c8990-145">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="c8990-145">Read-only</span></span>|
|<span data-ttu-id="c8990-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="c8990-146">sizeInByte</span></span>|<span data-ttu-id="c8990-147">Int64</span><span class="sxs-lookup"><span data-stu-id="c8990-147">Int64</span></span>|<span data-ttu-id="c8990-148">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="c8990-148">Discovered application size in bytes.</span></span> <span data-ttu-id="c8990-149">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="c8990-149">Read-only</span></span>|
|<span data-ttu-id="c8990-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="c8990-150">deviceCount</span></span>|<span data-ttu-id="c8990-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c8990-151">Int32</span></span>|<span data-ttu-id="c8990-152">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="c8990-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="c8990-153">応答</span><span class="sxs-lookup"><span data-stu-id="c8990-153">Response</span></span>
<span data-ttu-id="c8990-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8990-154">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8990-155">例</span><span class="sxs-lookup"><span data-stu-id="c8990-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8990-156">要求</span><span class="sxs-lookup"><span data-stu-id="c8990-156">Request</span></span>
<span data-ttu-id="c8990-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8990-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/detectedApps/{detectedAppId}
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

### <a name="response"></a><span data-ttu-id="c8990-158">応答</span><span class="sxs-lookup"><span data-stu-id="c8990-158">Response</span></span>
<span data-ttu-id="c8990-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8990-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




