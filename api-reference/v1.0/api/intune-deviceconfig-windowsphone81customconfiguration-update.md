---
title: windowsPhone81CustomConfiguration の更新
description: windowsPhone81CustomConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 218049be884e361e7dff38190f9a4debc49d3e7f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32520047"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="3fb0a-103">windowsPhone81CustomConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="3fb0a-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="3fb0a-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fb0a-105">[windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-105">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3fb0a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="3fb0a-106">Prerequisites</span></span>
<span data-ttu-id="3fb0a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3fb0a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3fb0a-109">Permission type</span></span>|<span data-ttu-id="3fb0a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3fb0a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fb0a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3fb0a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3fb0a-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3fb0a-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3fb0a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3fb0a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3fb0a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-114">Not supported.</span></span>|
|<span data-ttu-id="3fb0a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3fb0a-115">Application</span></span>|<span data-ttu-id="3fb0a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3fb0a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3fb0a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="3fb0a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fb0a-118">Request headers</span></span>
|<span data-ttu-id="3fb0a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3fb0a-119">Header</span></span>|<span data-ttu-id="3fb0a-120">値</span><span class="sxs-lookup"><span data-stu-id="3fb0a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3fb0a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3fb0a-121">Authorization</span></span>|<span data-ttu-id="3fb0a-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3fb0a-123">承諾</span><span class="sxs-lookup"><span data-stu-id="3fb0a-123">Accept</span></span>|<span data-ttu-id="3fb0a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3fb0a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fb0a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3fb0a-125">Request body</span></span>
<span data-ttu-id="3fb0a-126">要求本文で、[windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-126">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="3fb0a-127">次の表に、[windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-127">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="3fb0a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3fb0a-128">Property</span></span>|<span data-ttu-id="3fb0a-129">型</span><span class="sxs-lookup"><span data-stu-id="3fb0a-129">Type</span></span>|<span data-ttu-id="3fb0a-130">説明</span><span class="sxs-lookup"><span data-stu-id="3fb0a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fb0a-131">id</span><span class="sxs-lookup"><span data-stu-id="3fb0a-131">id</span></span>|<span data-ttu-id="3fb0a-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="3fb0a-132">String</span></span>|<span data-ttu-id="3fb0a-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-133">Key of the entity.</span></span> <span data-ttu-id="3fb0a-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3fb0a-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fb0a-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3fb0a-135">lastModifiedDateTime</span></span>|<span data-ttu-id="3fb0a-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fb0a-136">DateTimeOffset</span></span>|<span data-ttu-id="3fb0a-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-137">DateTime the object was last modified.</span></span> <span data-ttu-id="3fb0a-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3fb0a-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fb0a-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3fb0a-139">createdDateTime</span></span>|<span data-ttu-id="3fb0a-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3fb0a-140">DateTimeOffset</span></span>|<span data-ttu-id="3fb0a-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-141">DateTime the object was created.</span></span> <span data-ttu-id="3fb0a-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3fb0a-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fb0a-143">説明</span><span class="sxs-lookup"><span data-stu-id="3fb0a-143">description</span></span>|<span data-ttu-id="3fb0a-144">String</span><span class="sxs-lookup"><span data-stu-id="3fb0a-144">String</span></span>|<span data-ttu-id="3fb0a-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3fb0a-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3fb0a-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fb0a-147">displayName</span><span class="sxs-lookup"><span data-stu-id="3fb0a-147">displayName</span></span>|<span data-ttu-id="3fb0a-148">String</span><span class="sxs-lookup"><span data-stu-id="3fb0a-148">String</span></span>|<span data-ttu-id="3fb0a-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3fb0a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3fb0a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fb0a-151">version</span><span class="sxs-lookup"><span data-stu-id="3fb0a-151">version</span></span>|<span data-ttu-id="3fb0a-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3fb0a-152">Int32</span></span>|<span data-ttu-id="3fb0a-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-153">Version of the device configuration.</span></span> <span data-ttu-id="3fb0a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="3fb0a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3fb0a-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="3fb0a-155">omaSettings</span></span>|<span data-ttu-id="3fb0a-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3fb0a-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="3fb0a-157">OMA 設定。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-157">OMA settings.</span></span> <span data-ttu-id="3fb0a-158">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3fb0a-159">応答</span><span class="sxs-lookup"><span data-stu-id="3fb0a-159">Response</span></span>
<span data-ttu-id="3fb0a-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-160">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3fb0a-161">例</span><span class="sxs-lookup"><span data-stu-id="3fb0a-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="3fb0a-162">要求</span><span class="sxs-lookup"><span data-stu-id="3fb0a-162">Request</span></span>
<span data-ttu-id="3fb0a-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3fb0a-164">応答</span><span class="sxs-lookup"><span data-stu-id="3fb0a-164">Response</span></span>
<span data-ttu-id="3fb0a-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3fb0a-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



