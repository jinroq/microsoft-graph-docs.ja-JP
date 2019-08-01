---
title: windowsPhone81CustomConfiguration の更新
description: windowsPhone81CustomConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eba02dd93b71fb4f869839e9f4c046563e2bed68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018751"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="b70ee-103">windowsPhone81CustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="b70ee-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="b70ee-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b70ee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b70ee-105">[windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b70ee-105">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b70ee-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b70ee-106">Prerequisites</span></span>
<span data-ttu-id="b70ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b70ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b70ee-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b70ee-109">Permission type</span></span>|<span data-ttu-id="b70ee-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b70ee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b70ee-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b70ee-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b70ee-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b70ee-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b70ee-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b70ee-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b70ee-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b70ee-114">Not supported.</span></span>|
|<span data-ttu-id="b70ee-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b70ee-115">Application</span></span>|<span data-ttu-id="b70ee-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b70ee-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b70ee-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b70ee-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b70ee-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b70ee-118">Request headers</span></span>
|<span data-ttu-id="b70ee-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b70ee-119">Header</span></span>|<span data-ttu-id="b70ee-120">値</span><span class="sxs-lookup"><span data-stu-id="b70ee-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b70ee-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b70ee-121">Authorization</span></span>|<span data-ttu-id="b70ee-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b70ee-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b70ee-123">承諾</span><span class="sxs-lookup"><span data-stu-id="b70ee-123">Accept</span></span>|<span data-ttu-id="b70ee-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b70ee-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b70ee-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b70ee-125">Request body</span></span>
<span data-ttu-id="b70ee-126">要求本文で、[windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b70ee-126">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="b70ee-127">次の表に、[windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b70ee-127">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="b70ee-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b70ee-128">Property</span></span>|<span data-ttu-id="b70ee-129">型</span><span class="sxs-lookup"><span data-stu-id="b70ee-129">Type</span></span>|<span data-ttu-id="b70ee-130">説明</span><span class="sxs-lookup"><span data-stu-id="b70ee-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b70ee-131">id</span><span class="sxs-lookup"><span data-stu-id="b70ee-131">id</span></span>|<span data-ttu-id="b70ee-132">文字列</span><span class="sxs-lookup"><span data-stu-id="b70ee-132">String</span></span>|<span data-ttu-id="b70ee-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b70ee-133">Key of the entity.</span></span> <span data-ttu-id="b70ee-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b70ee-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b70ee-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b70ee-135">lastModifiedDateTime</span></span>|<span data-ttu-id="b70ee-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b70ee-136">DateTimeOffset</span></span>|<span data-ttu-id="b70ee-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b70ee-137">DateTime the object was last modified.</span></span> <span data-ttu-id="b70ee-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b70ee-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b70ee-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b70ee-139">createdDateTime</span></span>|<span data-ttu-id="b70ee-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b70ee-140">DateTimeOffset</span></span>|<span data-ttu-id="b70ee-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b70ee-141">DateTime the object was created.</span></span> <span data-ttu-id="b70ee-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b70ee-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b70ee-143">description</span><span class="sxs-lookup"><span data-stu-id="b70ee-143">description</span></span>|<span data-ttu-id="b70ee-144">String</span><span class="sxs-lookup"><span data-stu-id="b70ee-144">String</span></span>|<span data-ttu-id="b70ee-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b70ee-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b70ee-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b70ee-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b70ee-147">displayName</span><span class="sxs-lookup"><span data-stu-id="b70ee-147">displayName</span></span>|<span data-ttu-id="b70ee-148">String</span><span class="sxs-lookup"><span data-stu-id="b70ee-148">String</span></span>|<span data-ttu-id="b70ee-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b70ee-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b70ee-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b70ee-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b70ee-151">version</span><span class="sxs-lookup"><span data-stu-id="b70ee-151">version</span></span>|<span data-ttu-id="b70ee-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b70ee-152">Int32</span></span>|<span data-ttu-id="b70ee-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b70ee-153">Version of the device configuration.</span></span> <span data-ttu-id="b70ee-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b70ee-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b70ee-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="b70ee-155">omaSettings</span></span>|<span data-ttu-id="b70ee-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b70ee-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="b70ee-157">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="b70ee-157">OMA settings.</span></span> <span data-ttu-id="b70ee-158">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b70ee-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b70ee-159">応答</span><span class="sxs-lookup"><span data-stu-id="b70ee-159">Response</span></span>
<span data-ttu-id="b70ee-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b70ee-160">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b70ee-161">例</span><span class="sxs-lookup"><span data-stu-id="b70ee-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="b70ee-162">要求</span><span class="sxs-lookup"><span data-stu-id="b70ee-162">Request</span></span>
<span data-ttu-id="b70ee-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b70ee-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="b70ee-164">応答</span><span class="sxs-lookup"><span data-stu-id="b70ee-164">Response</span></span>
<span data-ttu-id="b70ee-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b70ee-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
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



