---
title: detectedApp の作成
description: 新しい detectedApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fc94785ac40cae870edf7abfdd0071406c50d00d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310641"
---
# <a name="create-detectedapp"></a><span data-ttu-id="2bdb6-103">detectedApp の作成</span><span class="sxs-lookup"><span data-stu-id="2bdb6-103">Create detectedApp</span></span>

> <span data-ttu-id="2bdb6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bdb6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bdb6-106">新しい [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-106">Create a new [detectedApp](../resources/intune-devices-detectedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bdb6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2bdb6-107">Prerequisites</span></span>
<span data-ttu-id="2bdb6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bdb6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2bdb6-110">Permission type</span></span>|<span data-ttu-id="2bdb6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2bdb6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bdb6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2bdb6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bdb6-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bdb6-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2bdb6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2bdb6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bdb6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-115">Not supported.</span></span>|
|<span data-ttu-id="2bdb6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2bdb6-116">Application</span></span>|<span data-ttu-id="2bdb6-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bdb6-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bdb6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2bdb6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/detectedApps
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps
```

## <a name="request-headers"></a><span data-ttu-id="2bdb6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bdb6-119">Request headers</span></span>
|<span data-ttu-id="2bdb6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2bdb6-120">Header</span></span>|<span data-ttu-id="2bdb6-121">値</span><span class="sxs-lookup"><span data-stu-id="2bdb6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bdb6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2bdb6-122">Authorization</span></span>|<span data-ttu-id="2bdb6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bdb6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2bdb6-124">Accept</span></span>|<span data-ttu-id="2bdb6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bdb6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bdb6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2bdb6-126">Request body</span></span>
<span data-ttu-id="2bdb6-127">要求本文で、detectedApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-127">In the request body, supply a JSON representation for the detectedApp object.</span></span>

<span data-ttu-id="2bdb6-128">次の表に、detectedApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-128">The following table shows the properties that are required when you create the detectedApp.</span></span>

|<span data-ttu-id="2bdb6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2bdb6-129">Property</span></span>|<span data-ttu-id="2bdb6-130">型</span><span class="sxs-lookup"><span data-stu-id="2bdb6-130">Type</span></span>|<span data-ttu-id="2bdb6-131">説明</span><span class="sxs-lookup"><span data-stu-id="2bdb6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bdb6-132">id</span><span class="sxs-lookup"><span data-stu-id="2bdb6-132">id</span></span>|<span data-ttu-id="2bdb6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2bdb6-133">String</span></span>|<span data-ttu-id="2bdb6-134">検出されたアプリケーションの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-134">The unique Identifier for the detected application.</span></span> <span data-ttu-id="2bdb6-135">これは、アプリケーションの作成時に、Intune によって自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-135">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="2bdb6-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-136">Read-only.</span></span>|
|<span data-ttu-id="2bdb6-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2bdb6-137">displayName</span></span>|<span data-ttu-id="2bdb6-138">String</span><span class="sxs-lookup"><span data-stu-id="2bdb6-138">String</span></span>|<span data-ttu-id="2bdb6-139">検出されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-139">Name of the discovered application.</span></span> <span data-ttu-id="2bdb6-140">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="2bdb6-140">Read-only</span></span>|
|<span data-ttu-id="2bdb6-141">version</span><span class="sxs-lookup"><span data-stu-id="2bdb6-141">version</span></span>|<span data-ttu-id="2bdb6-142">String</span><span class="sxs-lookup"><span data-stu-id="2bdb6-142">String</span></span>|<span data-ttu-id="2bdb6-143">検出されたアプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-143">Version of the discovered application.</span></span> <span data-ttu-id="2bdb6-144">読み取り専用</span><span class="sxs-lookup"><span data-stu-id="2bdb6-144">Read-only</span></span>|
|<span data-ttu-id="2bdb6-145">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="2bdb6-145">sizeInByte</span></span>|<span data-ttu-id="2bdb6-146">Int64</span><span class="sxs-lookup"><span data-stu-id="2bdb6-146">Int64</span></span>|<span data-ttu-id="2bdb6-147">検出されたアプリケーションのサイズ (バイト単位)。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-147">Discovered application size in bytes.</span></span> <span data-ttu-id="2bdb6-148">読み取り専用です</span><span class="sxs-lookup"><span data-stu-id="2bdb6-148">Read-only</span></span>|
|<span data-ttu-id="2bdb6-149">deviceCount</span><span class="sxs-lookup"><span data-stu-id="2bdb6-149">deviceCount</span></span>|<span data-ttu-id="2bdb6-150">Int32</span><span class="sxs-lookup"><span data-stu-id="2bdb6-150">Int32</span></span>|<span data-ttu-id="2bdb6-151">このアプリケーションがインストールされているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="2bdb6-151">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="2bdb6-152">応答</span><span class="sxs-lookup"><span data-stu-id="2bdb6-152">Response</span></span>
<span data-ttu-id="2bdb6-153">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [detectedApp](../resources/intune-devices-detectedapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-153">If successful, this method returns a `201 Created` response code and a [detectedApp](../resources/intune-devices-detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2bdb6-154">例</span><span class="sxs-lookup"><span data-stu-id="2bdb6-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bdb6-155">要求</span><span class="sxs-lookup"><span data-stu-id="2bdb6-155">Request</span></span>
<span data-ttu-id="2bdb6-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2bdb6-157">応答</span><span class="sxs-lookup"><span data-stu-id="2bdb6-157">Response</span></span>
<span data-ttu-id="2bdb6-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2bdb6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






