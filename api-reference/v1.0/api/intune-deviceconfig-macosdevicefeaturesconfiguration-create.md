---
title: macOSDeviceFeaturesConfiguration の作成
description: 新しい macOSDeviceFeaturesConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a431d88dd5914aa5e6cb90b06900c38d2ce4d244
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975022"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="a94f2-103">macOSDeviceFeaturesConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="a94f2-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="a94f2-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a94f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a94f2-105">新しい [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a94f2-105">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a94f2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a94f2-106">Prerequisites</span></span>
<span data-ttu-id="a94f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a94f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a94f2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a94f2-109">Permission type</span></span>|<span data-ttu-id="a94f2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a94f2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a94f2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a94f2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a94f2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a94f2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a94f2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a94f2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a94f2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a94f2-114">Not supported.</span></span>|
|<span data-ttu-id="a94f2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a94f2-115">Application</span></span>|<span data-ttu-id="a94f2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a94f2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a94f2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a94f2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a94f2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a94f2-118">Request headers</span></span>
|<span data-ttu-id="a94f2-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a94f2-119">Header</span></span>|<span data-ttu-id="a94f2-120">値</span><span class="sxs-lookup"><span data-stu-id="a94f2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a94f2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a94f2-121">Authorization</span></span>|<span data-ttu-id="a94f2-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a94f2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a94f2-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a94f2-123">Accept</span></span>|<span data-ttu-id="a94f2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a94f2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a94f2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a94f2-125">Request body</span></span>
<span data-ttu-id="a94f2-126">要求本文で、macOSDeviceFeaturesConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a94f2-126">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="a94f2-127">次の表に、macOSDeviceFeaturesConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a94f2-127">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="a94f2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a94f2-128">Property</span></span>|<span data-ttu-id="a94f2-129">型</span><span class="sxs-lookup"><span data-stu-id="a94f2-129">Type</span></span>|<span data-ttu-id="a94f2-130">説明</span><span class="sxs-lookup"><span data-stu-id="a94f2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a94f2-131">id</span><span class="sxs-lookup"><span data-stu-id="a94f2-131">id</span></span>|<span data-ttu-id="a94f2-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a94f2-132">String</span></span>|<span data-ttu-id="a94f2-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a94f2-133">Key of the entity.</span></span> <span data-ttu-id="a94f2-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a94f2-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a94f2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a94f2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a94f2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a94f2-136">DateTimeOffset</span></span>|<span data-ttu-id="a94f2-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a94f2-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a94f2-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a94f2-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a94f2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a94f2-139">createdDateTime</span></span>|<span data-ttu-id="a94f2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a94f2-140">DateTimeOffset</span></span>|<span data-ttu-id="a94f2-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a94f2-141">DateTime the object was created.</span></span> <span data-ttu-id="a94f2-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a94f2-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a94f2-143">description</span><span class="sxs-lookup"><span data-stu-id="a94f2-143">description</span></span>|<span data-ttu-id="a94f2-144">String</span><span class="sxs-lookup"><span data-stu-id="a94f2-144">String</span></span>|<span data-ttu-id="a94f2-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a94f2-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a94f2-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a94f2-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a94f2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a94f2-147">displayName</span></span>|<span data-ttu-id="a94f2-148">String</span><span class="sxs-lookup"><span data-stu-id="a94f2-148">String</span></span>|<span data-ttu-id="a94f2-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a94f2-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a94f2-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a94f2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a94f2-151">version</span><span class="sxs-lookup"><span data-stu-id="a94f2-151">version</span></span>|<span data-ttu-id="a94f2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a94f2-152">Int32</span></span>|<span data-ttu-id="a94f2-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a94f2-153">Version of the device configuration.</span></span> <span data-ttu-id="a94f2-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a94f2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a94f2-155">応答</span><span class="sxs-lookup"><span data-stu-id="a94f2-155">Response</span></span>
<span data-ttu-id="a94f2-156">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a94f2-156">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a94f2-157">例</span><span class="sxs-lookup"><span data-stu-id="a94f2-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="a94f2-158">要求</span><span class="sxs-lookup"><span data-stu-id="a94f2-158">Request</span></span>
<span data-ttu-id="a94f2-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a94f2-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="a94f2-160">応答</span><span class="sxs-lookup"><span data-stu-id="a94f2-160">Response</span></span>
<span data-ttu-id="a94f2-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a94f2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```



