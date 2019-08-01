---
title: windowsDefenderAdvancedThreatProtectionConfiguration の作成
description: 新しい windowsDefenderAdvancedThreatProtectionConfigurations オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a762ae3697166efbac3680c8f92dba12bde68b43
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997107"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="a4835-103">windowsDefenderAdvancedThreatProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="a4835-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="a4835-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4835-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4835-105">新しい [windowsDefenderAdvancedThreatProtectionConfigurations](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a4835-105">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4835-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a4835-106">Prerequisites</span></span>
<span data-ttu-id="a4835-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4835-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4835-109">Permission type</span></span>|<span data-ttu-id="a4835-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4835-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4835-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4835-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4835-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4835-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a4835-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4835-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4835-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4835-114">Not supported.</span></span>|
|<span data-ttu-id="a4835-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4835-115">Application</span></span>|<span data-ttu-id="a4835-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4835-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4835-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4835-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a4835-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4835-118">Request headers</span></span>
|<span data-ttu-id="a4835-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4835-119">Header</span></span>|<span data-ttu-id="a4835-120">値</span><span class="sxs-lookup"><span data-stu-id="a4835-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4835-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4835-121">Authorization</span></span>|<span data-ttu-id="a4835-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4835-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4835-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a4835-123">Accept</span></span>|<span data-ttu-id="a4835-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4835-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4835-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4835-125">Request body</span></span>
<span data-ttu-id="a4835-126">要求本文で、windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a4835-126">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="a4835-127">次の表に、windowsDefenderAdvancedThreatProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a4835-127">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="a4835-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4835-128">Property</span></span>|<span data-ttu-id="a4835-129">型</span><span class="sxs-lookup"><span data-stu-id="a4835-129">Type</span></span>|<span data-ttu-id="a4835-130">説明</span><span class="sxs-lookup"><span data-stu-id="a4835-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4835-131">id</span><span class="sxs-lookup"><span data-stu-id="a4835-131">id</span></span>|<span data-ttu-id="a4835-132">文字列</span><span class="sxs-lookup"><span data-stu-id="a4835-132">String</span></span>|<span data-ttu-id="a4835-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a4835-133">Key of the entity.</span></span> <span data-ttu-id="a4835-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4835-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4835-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a4835-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a4835-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4835-136">DateTimeOffset</span></span>|<span data-ttu-id="a4835-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a4835-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a4835-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4835-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4835-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a4835-139">createdDateTime</span></span>|<span data-ttu-id="a4835-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a4835-140">DateTimeOffset</span></span>|<span data-ttu-id="a4835-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a4835-141">DateTime the object was created.</span></span> <span data-ttu-id="a4835-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4835-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4835-143">description</span><span class="sxs-lookup"><span data-stu-id="a4835-143">description</span></span>|<span data-ttu-id="a4835-144">String</span><span class="sxs-lookup"><span data-stu-id="a4835-144">String</span></span>|<span data-ttu-id="a4835-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a4835-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a4835-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4835-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4835-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a4835-147">displayName</span></span>|<span data-ttu-id="a4835-148">String</span><span class="sxs-lookup"><span data-stu-id="a4835-148">String</span></span>|<span data-ttu-id="a4835-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a4835-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a4835-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4835-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4835-151">version</span><span class="sxs-lookup"><span data-stu-id="a4835-151">version</span></span>|<span data-ttu-id="a4835-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a4835-152">Int32</span></span>|<span data-ttu-id="a4835-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a4835-153">Version of the device configuration.</span></span> <span data-ttu-id="a4835-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a4835-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a4835-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="a4835-155">allowSampleSharing</span></span>|<span data-ttu-id="a4835-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4835-156">Boolean</span></span>|<span data-ttu-id="a4835-157">Windows Defender AdvancedThreatProtection の "サンプルの共有を許可する" ルール</span><span class="sxs-lookup"><span data-stu-id="a4835-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="a4835-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="a4835-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="a4835-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4835-159">Boolean</span></span>|<span data-ttu-id="a4835-160">Windows Defender Advanced Threat Protection テレメトリ レポートの頻度を高めます。</span><span class="sxs-lookup"><span data-stu-id="a4835-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="a4835-161">応答</span><span class="sxs-lookup"><span data-stu-id="a4835-161">Response</span></span>
<span data-ttu-id="a4835-162">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a4835-162">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4835-163">例</span><span class="sxs-lookup"><span data-stu-id="a4835-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4835-164">要求</span><span class="sxs-lookup"><span data-stu-id="a4835-164">Request</span></span>
<span data-ttu-id="a4835-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a4835-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```

### <a name="response"></a><span data-ttu-id="a4835-166">応答</span><span class="sxs-lookup"><span data-stu-id="a4835-166">Response</span></span>
<span data-ttu-id="a4835-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a4835-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 439

{
  "@odata.type": "#microsoft.graph.windowsDefenderAdvancedThreatProtectionConfiguration",
  "id": "294373aa-73aa-2943-aa73-4329aa734329",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowSampleSharing": true,
  "enableExpeditedTelemetryReporting": true
}
```



