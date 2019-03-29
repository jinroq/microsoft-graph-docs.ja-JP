---
title: androidCustomConfiguration の更新
description: androidCustomConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 01a6738e4fcd9e86c965ff3d33aac0b9f07918e8
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962835"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="ab440-103">androidCustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="ab440-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="ab440-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ab440-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab440-105">[androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab440-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ab440-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ab440-106">Prerequisites</span></span>
<span data-ttu-id="ab440-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab440-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab440-109">Permission type</span></span>|<span data-ttu-id="ab440-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab440-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab440-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab440-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ab440-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab440-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab440-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab440-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab440-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab440-114">Not supported.</span></span>|
|<span data-ttu-id="ab440-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab440-115">Application</span></span>|<span data-ttu-id="ab440-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab440-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab440-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab440-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ab440-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab440-118">Request headers</span></span>
|<span data-ttu-id="ab440-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab440-119">Header</span></span>|<span data-ttu-id="ab440-120">値</span><span class="sxs-lookup"><span data-stu-id="ab440-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab440-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab440-121">Authorization</span></span>|<span data-ttu-id="ab440-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ab440-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab440-123">承諾</span><span class="sxs-lookup"><span data-stu-id="ab440-123">Accept</span></span>|<span data-ttu-id="ab440-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ab440-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab440-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab440-125">Request body</span></span>
<span data-ttu-id="ab440-126">要求本文で、[androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ab440-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="ab440-127">次の表に、[androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ab440-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="ab440-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab440-128">Property</span></span>|<span data-ttu-id="ab440-129">型</span><span class="sxs-lookup"><span data-stu-id="ab440-129">Type</span></span>|<span data-ttu-id="ab440-130">説明</span><span class="sxs-lookup"><span data-stu-id="ab440-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab440-131">id</span><span class="sxs-lookup"><span data-stu-id="ab440-131">id</span></span>|<span data-ttu-id="ab440-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ab440-132">String</span></span>|<span data-ttu-id="ab440-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ab440-133">Key of the entity.</span></span> <span data-ttu-id="ab440-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ab440-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab440-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ab440-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ab440-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab440-136">DateTimeOffset</span></span>|<span data-ttu-id="ab440-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ab440-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ab440-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ab440-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab440-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ab440-139">createdDateTime</span></span>|<span data-ttu-id="ab440-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab440-140">DateTimeOffset</span></span>|<span data-ttu-id="ab440-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="ab440-141">DateTime the object was created.</span></span> <span data-ttu-id="ab440-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ab440-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab440-143">description</span><span class="sxs-lookup"><span data-stu-id="ab440-143">description</span></span>|<span data-ttu-id="ab440-144">String</span><span class="sxs-lookup"><span data-stu-id="ab440-144">String</span></span>|<span data-ttu-id="ab440-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="ab440-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ab440-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ab440-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab440-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ab440-147">displayName</span></span>|<span data-ttu-id="ab440-148">String</span><span class="sxs-lookup"><span data-stu-id="ab440-148">String</span></span>|<span data-ttu-id="ab440-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="ab440-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ab440-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ab440-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab440-151">version</span><span class="sxs-lookup"><span data-stu-id="ab440-151">version</span></span>|<span data-ttu-id="ab440-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ab440-152">Int32</span></span>|<span data-ttu-id="ab440-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ab440-153">Version of the device configuration.</span></span> <span data-ttu-id="ab440-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ab440-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ab440-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ab440-155">omaSettings</span></span>|<span data-ttu-id="ab440-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ab440-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="ab440-157">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="ab440-157">OMA settings.</span></span> <span data-ttu-id="ab440-158">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="ab440-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ab440-159">応答</span><span class="sxs-lookup"><span data-stu-id="ab440-159">Response</span></span>
<span data-ttu-id="ab440-160">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="ab440-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab440-161">例</span><span class="sxs-lookup"><span data-stu-id="ab440-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="ab440-162">要求</span><span class="sxs-lookup"><span data-stu-id="ab440-162">Request</span></span>
<span data-ttu-id="ab440-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ab440-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ab440-164">応答</span><span class="sxs-lookup"><span data-stu-id="ab440-164">Response</span></span>
<span data-ttu-id="ab440-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ab440-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```



