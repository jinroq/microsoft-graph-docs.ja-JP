---
title: macOSCustomConfiguration の更新
description: macOSCustomConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 29d7ef8b896a6c47760a777c3b30e6c09a0642f4
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258913"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="64e1c-103">macOSCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="64e1c-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="64e1c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="64e1c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64e1c-105">[macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="64e1c-105">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64e1c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="64e1c-106">Prerequisites</span></span>
<span data-ttu-id="64e1c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64e1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="64e1c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64e1c-109">Permission type</span></span>|<span data-ttu-id="64e1c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="64e1c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64e1c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64e1c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64e1c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64e1c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64e1c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64e1c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64e1c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64e1c-114">Not supported.</span></span>|
|<span data-ttu-id="64e1c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64e1c-115">Application</span></span>|<span data-ttu-id="64e1c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64e1c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64e1c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64e1c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="64e1c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64e1c-118">Request headers</span></span>
|<span data-ttu-id="64e1c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64e1c-119">Header</span></span>|<span data-ttu-id="64e1c-120">値</span><span class="sxs-lookup"><span data-stu-id="64e1c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64e1c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="64e1c-121">Authorization</span></span>|<span data-ttu-id="64e1c-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="64e1c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64e1c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="64e1c-123">Accept</span></span>|<span data-ttu-id="64e1c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="64e1c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64e1c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="64e1c-125">Request body</span></span>
<span data-ttu-id="64e1c-126">要求本文で、[macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="64e1c-126">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="64e1c-127">次の表に、[macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="64e1c-127">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="64e1c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64e1c-128">Property</span></span>|<span data-ttu-id="64e1c-129">型</span><span class="sxs-lookup"><span data-stu-id="64e1c-129">Type</span></span>|<span data-ttu-id="64e1c-130">説明</span><span class="sxs-lookup"><span data-stu-id="64e1c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64e1c-131">id</span><span class="sxs-lookup"><span data-stu-id="64e1c-131">id</span></span>|<span data-ttu-id="64e1c-132">文字列</span><span class="sxs-lookup"><span data-stu-id="64e1c-132">String</span></span>|<span data-ttu-id="64e1c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="64e1c-133">Key of the entity.</span></span> <span data-ttu-id="64e1c-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64e1c-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e1c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64e1c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="64e1c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64e1c-136">DateTimeOffset</span></span>|<span data-ttu-id="64e1c-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="64e1c-137">DateTime the object was last modified.</span></span> <span data-ttu-id="64e1c-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64e1c-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e1c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64e1c-139">createdDateTime</span></span>|<span data-ttu-id="64e1c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64e1c-140">DateTimeOffset</span></span>|<span data-ttu-id="64e1c-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="64e1c-141">DateTime the object was created.</span></span> <span data-ttu-id="64e1c-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64e1c-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e1c-143">説明</span><span class="sxs-lookup"><span data-stu-id="64e1c-143">description</span></span>|<span data-ttu-id="64e1c-144">文字列</span><span class="sxs-lookup"><span data-stu-id="64e1c-144">String</span></span>|<span data-ttu-id="64e1c-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="64e1c-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64e1c-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64e1c-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e1c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="64e1c-147">displayName</span></span>|<span data-ttu-id="64e1c-148">String</span><span class="sxs-lookup"><span data-stu-id="64e1c-148">String</span></span>|<span data-ttu-id="64e1c-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="64e1c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64e1c-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64e1c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e1c-151">version</span><span class="sxs-lookup"><span data-stu-id="64e1c-151">version</span></span>|<span data-ttu-id="64e1c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="64e1c-152">Int32</span></span>|<span data-ttu-id="64e1c-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="64e1c-153">Version of the device configuration.</span></span> <span data-ttu-id="64e1c-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64e1c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64e1c-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="64e1c-155">payloadName</span></span>|<span data-ttu-id="64e1c-156">String</span><span class="sxs-lookup"><span data-stu-id="64e1c-156">String</span></span>|<span data-ttu-id="64e1c-157">ユーザーに表示される名前。</span><span class="sxs-lookup"><span data-stu-id="64e1c-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="64e1c-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="64e1c-158">payloadFileName</span></span>|<span data-ttu-id="64e1c-159">String</span><span class="sxs-lookup"><span data-stu-id="64e1c-159">String</span></span>|<span data-ttu-id="64e1c-160">ペイロード ファイル名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="64e1c-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="64e1c-161">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="64e1c-161">\*.xml).</span></span>|
|<span data-ttu-id="64e1c-162">payload</span><span class="sxs-lookup"><span data-stu-id="64e1c-162">payload</span></span>|<span data-ttu-id="64e1c-163">Binary</span><span class="sxs-lookup"><span data-stu-id="64e1c-163">Binary</span></span>|<span data-ttu-id="64e1c-164">ペイロード。</span><span class="sxs-lookup"><span data-stu-id="64e1c-164">Payload.</span></span> <span data-ttu-id="64e1c-165">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="64e1c-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="64e1c-166">応答</span><span class="sxs-lookup"><span data-stu-id="64e1c-166">Response</span></span>
<span data-ttu-id="64e1c-167">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="64e1c-167">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64e1c-168">例</span><span class="sxs-lookup"><span data-stu-id="64e1c-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="64e1c-169">要求</span><span class="sxs-lookup"><span data-stu-id="64e1c-169">Request</span></span>
<span data-ttu-id="64e1c-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64e1c-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="64e1c-171">応答</span><span class="sxs-lookup"><span data-stu-id="64e1c-171">Response</span></span>
<span data-ttu-id="64e1c-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="64e1c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



