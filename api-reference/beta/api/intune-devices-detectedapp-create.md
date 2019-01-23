---
title: detectedApp の作成
description: 新しい detectedApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 24151e64b23e1e0d57485fab82d63eff839eb84a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393103"
---
# <a name="create-detectedapp"></a><span data-ttu-id="e51b7-103">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="e51b7-103">Create detectedApp</span></span>

> <span data-ttu-id="e51b7-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e51b7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e51b7-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e51b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e51b7-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e51b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e51b7-107">新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e51b7-107">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e51b7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e51b7-108">Prerequisites</span></span>
<span data-ttu-id="e51b7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e51b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e51b7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e51b7-111">Permission type</span></span>|<span data-ttu-id="e51b7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e51b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e51b7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e51b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e51b7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e51b7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e51b7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e51b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e51b7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e51b7-116">Not supported.</span></span>|
|<span data-ttu-id="e51b7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e51b7-117">Application</span></span>|<span data-ttu-id="e51b7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e51b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e51b7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e51b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="e51b7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e51b7-120">Request headers</span></span>
|<span data-ttu-id="e51b7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e51b7-121">Header</span></span>|<span data-ttu-id="e51b7-122">値</span><span class="sxs-lookup"><span data-stu-id="e51b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e51b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e51b7-123">Authorization</span></span>|<span data-ttu-id="e51b7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e51b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e51b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e51b7-125">Accept</span></span>|<span data-ttu-id="e51b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e51b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e51b7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e51b7-127">Request body</span></span>
<span data-ttu-id="e51b7-128">要求本文で、detectedApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e51b7-128">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="e51b7-129">次の表に、detectedApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e51b7-129">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="e51b7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e51b7-130">Property</span></span>|<span data-ttu-id="e51b7-131">型</span><span class="sxs-lookup"><span data-stu-id="e51b7-131">Type</span></span>|<span data-ttu-id="e51b7-132">説明</span><span class="sxs-lookup"><span data-stu-id="e51b7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e51b7-133">id</span><span class="sxs-lookup"><span data-stu-id="e51b7-133">id</span></span>|<span data-ttu-id="e51b7-134">String</span><span class="sxs-lookup"><span data-stu-id="e51b7-134">String</span></span>|<span data-ttu-id="e51b7-135">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e51b7-135">The unique Identifier for the detected application.</span></span> <span data-ttu-id="e51b7-136">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="e51b7-136">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="e51b7-137">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e51b7-137">Read-only.</span></span>|
|<span data-ttu-id="e51b7-138">displayName</span><span class="sxs-lookup"><span data-stu-id="e51b7-138">displayName</span></span>|<span data-ttu-id="e51b7-139">String</span><span class="sxs-lookup"><span data-stu-id="e51b7-139">String</span></span>|<span data-ttu-id="e51b7-140">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="e51b7-140">Name of the discovered application.</span></span> <span data-ttu-id="e51b7-141">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="e51b7-141">Read-only</span></span>|
|<span data-ttu-id="e51b7-142">version</span><span class="sxs-lookup"><span data-stu-id="e51b7-142">version</span></span>|<span data-ttu-id="e51b7-143">String</span><span class="sxs-lookup"><span data-stu-id="e51b7-143">String</span></span>|<span data-ttu-id="e51b7-144">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e51b7-144">Version of the discovered application.</span></span> <span data-ttu-id="e51b7-145">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="e51b7-145">Read-only</span></span>|
|<span data-ttu-id="e51b7-146">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="e51b7-146">sizeInByte</span></span>|<span data-ttu-id="e51b7-147">Int64</span><span class="sxs-lookup"><span data-stu-id="e51b7-147">Int64</span></span>|<span data-ttu-id="e51b7-148">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="e51b7-148">Discovered application size in bytes.</span></span> <span data-ttu-id="e51b7-149">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="e51b7-149">Read-only</span></span>|
|<span data-ttu-id="e51b7-150">deviceCount</span><span class="sxs-lookup"><span data-stu-id="e51b7-150">deviceCount</span></span>|<span data-ttu-id="e51b7-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e51b7-151">Int32</span></span>|<span data-ttu-id="e51b7-152">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e51b7-152">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="e51b7-153">応答</span><span class="sxs-lookup"><span data-stu-id="e51b7-153">Response</span></span>
<span data-ttu-id="e51b7-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e51b7-154">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e51b7-155">例</span><span class="sxs-lookup"><span data-stu-id="e51b7-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="e51b7-156">要求</span><span class="sxs-lookup"><span data-stu-id="e51b7-156">Request</span></span>
<span data-ttu-id="e51b7-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e51b7-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/detectedApps
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

### <a name="response"></a><span data-ttu-id="e51b7-158">応答</span><span class="sxs-lookup"><span data-stu-id="e51b7-158">Response</span></span>
<span data-ttu-id="e51b7-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e51b7-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




