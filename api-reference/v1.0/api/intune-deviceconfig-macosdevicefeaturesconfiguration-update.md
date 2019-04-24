---
title: macOSDeviceFeaturesConfiguration の更新
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3754eaa1018c92259b3b4136536151bc3850f633
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503619"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="96d71-103">macOSDeviceFeaturesConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="96d71-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="96d71-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96d71-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96d71-105">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="96d71-105">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96d71-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="96d71-106">Prerequisites</span></span>
<span data-ttu-id="96d71-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96d71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96d71-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96d71-109">Permission type</span></span>|<span data-ttu-id="96d71-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="96d71-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96d71-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96d71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="96d71-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96d71-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96d71-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96d71-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96d71-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96d71-114">Not supported.</span></span>|
|<span data-ttu-id="96d71-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96d71-115">Application</span></span>|<span data-ttu-id="96d71-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96d71-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96d71-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96d71-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="96d71-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96d71-118">Request headers</span></span>
|<span data-ttu-id="96d71-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96d71-119">Header</span></span>|<span data-ttu-id="96d71-120">値</span><span class="sxs-lookup"><span data-stu-id="96d71-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96d71-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96d71-121">Authorization</span></span>|<span data-ttu-id="96d71-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="96d71-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96d71-123">承諾</span><span class="sxs-lookup"><span data-stu-id="96d71-123">Accept</span></span>|<span data-ttu-id="96d71-124">application/json</span><span class="sxs-lookup"><span data-stu-id="96d71-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96d71-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="96d71-125">Request body</span></span>
<span data-ttu-id="96d71-126">要求本文で、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="96d71-126">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="96d71-127">次の表に、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="96d71-127">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="96d71-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96d71-128">Property</span></span>|<span data-ttu-id="96d71-129">型</span><span class="sxs-lookup"><span data-stu-id="96d71-129">Type</span></span>|<span data-ttu-id="96d71-130">説明</span><span class="sxs-lookup"><span data-stu-id="96d71-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96d71-131">id</span><span class="sxs-lookup"><span data-stu-id="96d71-131">id</span></span>|<span data-ttu-id="96d71-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="96d71-132">String</span></span>|<span data-ttu-id="96d71-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="96d71-133">Key of the entity.</span></span> <span data-ttu-id="96d71-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96d71-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96d71-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96d71-135">lastModifiedDateTime</span></span>|<span data-ttu-id="96d71-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96d71-136">DateTimeOffset</span></span>|<span data-ttu-id="96d71-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="96d71-137">DateTime the object was last modified.</span></span> <span data-ttu-id="96d71-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96d71-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96d71-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96d71-139">createdDateTime</span></span>|<span data-ttu-id="96d71-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96d71-140">DateTimeOffset</span></span>|<span data-ttu-id="96d71-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="96d71-141">DateTime the object was created.</span></span> <span data-ttu-id="96d71-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96d71-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96d71-143">説明</span><span class="sxs-lookup"><span data-stu-id="96d71-143">description</span></span>|<span data-ttu-id="96d71-144">String</span><span class="sxs-lookup"><span data-stu-id="96d71-144">String</span></span>|<span data-ttu-id="96d71-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="96d71-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="96d71-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96d71-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96d71-147">displayName</span><span class="sxs-lookup"><span data-stu-id="96d71-147">displayName</span></span>|<span data-ttu-id="96d71-148">String</span><span class="sxs-lookup"><span data-stu-id="96d71-148">String</span></span>|<span data-ttu-id="96d71-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="96d71-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="96d71-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96d71-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="96d71-151">version</span><span class="sxs-lookup"><span data-stu-id="96d71-151">version</span></span>|<span data-ttu-id="96d71-152">Int32</span><span class="sxs-lookup"><span data-stu-id="96d71-152">Int32</span></span>|<span data-ttu-id="96d71-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="96d71-153">Version of the device configuration.</span></span> <span data-ttu-id="96d71-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="96d71-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="96d71-155">応答</span><span class="sxs-lookup"><span data-stu-id="96d71-155">Response</span></span>
<span data-ttu-id="96d71-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="96d71-156">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96d71-157">例</span><span class="sxs-lookup"><span data-stu-id="96d71-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="96d71-158">要求</span><span class="sxs-lookup"><span data-stu-id="96d71-158">Request</span></span>
<span data-ttu-id="96d71-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96d71-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="96d71-160">応答</span><span class="sxs-lookup"><span data-stu-id="96d71-160">Response</span></span>
<span data-ttu-id="96d71-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="96d71-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



