---
title: macOSCustomConfiguration の作成
description: 新しい macOSCustomConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dcf798f506b4f805114e3810949ab0817639405c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997513"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="a17a6-103">macOSCustomConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="a17a6-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="a17a6-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a17a6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a17a6-105">新しい [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a17a6-105">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a17a6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a17a6-106">Prerequisites</span></span>
<span data-ttu-id="a17a6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a17a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a17a6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a17a6-109">Permission type</span></span>|<span data-ttu-id="a17a6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a17a6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a17a6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a17a6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a17a6-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a17a6-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a17a6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a17a6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a17a6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a17a6-114">Not supported.</span></span>|
|<span data-ttu-id="a17a6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a17a6-115">Application</span></span>|<span data-ttu-id="a17a6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a17a6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a17a6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a17a6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a17a6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a17a6-118">Request headers</span></span>
|<span data-ttu-id="a17a6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a17a6-119">Header</span></span>|<span data-ttu-id="a17a6-120">値</span><span class="sxs-lookup"><span data-stu-id="a17a6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a17a6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a17a6-121">Authorization</span></span>|<span data-ttu-id="a17a6-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a17a6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a17a6-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a17a6-123">Accept</span></span>|<span data-ttu-id="a17a6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a17a6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a17a6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a17a6-125">Request body</span></span>
<span data-ttu-id="a17a6-126">要求本文で、macOSCustomConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a17a6-126">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="a17a6-127">次の表に、macOSCustomConfiguration 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a17a6-127">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="a17a6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a17a6-128">Property</span></span>|<span data-ttu-id="a17a6-129">型</span><span class="sxs-lookup"><span data-stu-id="a17a6-129">Type</span></span>|<span data-ttu-id="a17a6-130">説明</span><span class="sxs-lookup"><span data-stu-id="a17a6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a17a6-131">id</span><span class="sxs-lookup"><span data-stu-id="a17a6-131">id</span></span>|<span data-ttu-id="a17a6-132">文字列</span><span class="sxs-lookup"><span data-stu-id="a17a6-132">String</span></span>|<span data-ttu-id="a17a6-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a17a6-133">Key of the entity.</span></span> <span data-ttu-id="a17a6-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a17a6-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a17a6-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a17a6-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a17a6-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a17a6-136">DateTimeOffset</span></span>|<span data-ttu-id="a17a6-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a17a6-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a17a6-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a17a6-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a17a6-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a17a6-139">createdDateTime</span></span>|<span data-ttu-id="a17a6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a17a6-140">DateTimeOffset</span></span>|<span data-ttu-id="a17a6-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a17a6-141">DateTime the object was created.</span></span> <span data-ttu-id="a17a6-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a17a6-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a17a6-143">description</span><span class="sxs-lookup"><span data-stu-id="a17a6-143">description</span></span>|<span data-ttu-id="a17a6-144">String</span><span class="sxs-lookup"><span data-stu-id="a17a6-144">String</span></span>|<span data-ttu-id="a17a6-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a17a6-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a17a6-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a17a6-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a17a6-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a17a6-147">displayName</span></span>|<span data-ttu-id="a17a6-148">String</span><span class="sxs-lookup"><span data-stu-id="a17a6-148">String</span></span>|<span data-ttu-id="a17a6-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a17a6-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a17a6-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a17a6-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a17a6-151">version</span><span class="sxs-lookup"><span data-stu-id="a17a6-151">version</span></span>|<span data-ttu-id="a17a6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a17a6-152">Int32</span></span>|<span data-ttu-id="a17a6-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a17a6-153">Version of the device configuration.</span></span> <span data-ttu-id="a17a6-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a17a6-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a17a6-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="a17a6-155">payloadName</span></span>|<span data-ttu-id="a17a6-156">String</span><span class="sxs-lookup"><span data-stu-id="a17a6-156">String</span></span>|<span data-ttu-id="a17a6-157">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="a17a6-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="a17a6-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="a17a6-158">payloadFileName</span></span>|<span data-ttu-id="a17a6-159">String</span><span class="sxs-lookup"><span data-stu-id="a17a6-159">String</span></span>|<span data-ttu-id="a17a6-160">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="a17a6-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="a17a6-161">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="a17a6-161">\*.xml).</span></span>|
|<span data-ttu-id="a17a6-162">payload</span><span class="sxs-lookup"><span data-stu-id="a17a6-162">payload</span></span>|<span data-ttu-id="a17a6-163">Binary</span><span class="sxs-lookup"><span data-stu-id="a17a6-163">Binary</span></span>|<span data-ttu-id="a17a6-164">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="a17a6-164">Payload.</span></span> <span data-ttu-id="a17a6-165">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="a17a6-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="a17a6-166">応答</span><span class="sxs-lookup"><span data-stu-id="a17a6-166">Response</span></span>
<span data-ttu-id="a17a6-167">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a17a6-167">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a17a6-168">例</span><span class="sxs-lookup"><span data-stu-id="a17a6-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="a17a6-169">要求</span><span class="sxs-lookup"><span data-stu-id="a17a6-169">Request</span></span>
<span data-ttu-id="a17a6-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a17a6-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="a17a6-171">応答</span><span class="sxs-lookup"><span data-stu-id="a17a6-171">Response</span></span>
<span data-ttu-id="a17a6-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a17a6-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```



