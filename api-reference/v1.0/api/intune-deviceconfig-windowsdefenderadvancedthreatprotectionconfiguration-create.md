---
title: windowsDefenderAdvancedThreatProtectionConfiguration の作成
description: 新しい windowsDefenderAdvancedThreatProtectionConfigurations オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92afe2c99b1345fb1d987f80e8b97e3f62e74914
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258038"
---
# <a name="create-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="43c49-103">windowsDefenderAdvancedThreatProtectionConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="43c49-103">Create windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="43c49-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43c49-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43c49-105">新しい [windowsDefenderAdvancedThreatProtectionConfigurations](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="43c49-105">Create a new [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43c49-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="43c49-106">Prerequisites</span></span>
<span data-ttu-id="43c49-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43c49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="43c49-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43c49-109">Permission type</span></span>|<span data-ttu-id="43c49-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="43c49-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43c49-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43c49-111">Delegated (work or school account)</span></span>|<span data-ttu-id="43c49-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43c49-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="43c49-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43c49-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43c49-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43c49-114">Not supported.</span></span>|
|<span data-ttu-id="43c49-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43c49-115">Application</span></span>|<span data-ttu-id="43c49-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43c49-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43c49-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43c49-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="43c49-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43c49-118">Request headers</span></span>
|<span data-ttu-id="43c49-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43c49-119">Header</span></span>|<span data-ttu-id="43c49-120">値</span><span class="sxs-lookup"><span data-stu-id="43c49-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43c49-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="43c49-121">Authorization</span></span>|<span data-ttu-id="43c49-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="43c49-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43c49-123">承諾</span><span class="sxs-lookup"><span data-stu-id="43c49-123">Accept</span></span>|<span data-ttu-id="43c49-124">application/json</span><span class="sxs-lookup"><span data-stu-id="43c49-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43c49-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="43c49-125">Request body</span></span>
<span data-ttu-id="43c49-126">要求本文で、windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="43c49-126">In the request body, supply a JSON representation for the windowsDefenderAdvancedThreatProtectionConfiguration object.</span></span>

<span data-ttu-id="43c49-127">次の表に、windowsDefenderAdvancedThreatProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="43c49-127">The following table shows the properties that are required when you create the windowsDefenderAdvancedThreatProtectionConfiguration.</span></span>

|<span data-ttu-id="43c49-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43c49-128">Property</span></span>|<span data-ttu-id="43c49-129">型</span><span class="sxs-lookup"><span data-stu-id="43c49-129">Type</span></span>|<span data-ttu-id="43c49-130">説明</span><span class="sxs-lookup"><span data-stu-id="43c49-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43c49-131">id</span><span class="sxs-lookup"><span data-stu-id="43c49-131">id</span></span>|<span data-ttu-id="43c49-132">文字列</span><span class="sxs-lookup"><span data-stu-id="43c49-132">String</span></span>|<span data-ttu-id="43c49-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="43c49-133">Key of the entity.</span></span> <span data-ttu-id="43c49-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43c49-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43c49-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43c49-135">lastModifiedDateTime</span></span>|<span data-ttu-id="43c49-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43c49-136">DateTimeOffset</span></span>|<span data-ttu-id="43c49-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="43c49-137">DateTime the object was last modified.</span></span> <span data-ttu-id="43c49-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43c49-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43c49-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43c49-139">createdDateTime</span></span>|<span data-ttu-id="43c49-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43c49-140">DateTimeOffset</span></span>|<span data-ttu-id="43c49-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="43c49-141">DateTime the object was created.</span></span> <span data-ttu-id="43c49-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43c49-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43c49-143">説明</span><span class="sxs-lookup"><span data-stu-id="43c49-143">description</span></span>|<span data-ttu-id="43c49-144">String</span><span class="sxs-lookup"><span data-stu-id="43c49-144">String</span></span>|<span data-ttu-id="43c49-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="43c49-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="43c49-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43c49-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43c49-147">displayName</span><span class="sxs-lookup"><span data-stu-id="43c49-147">displayName</span></span>|<span data-ttu-id="43c49-148">String</span><span class="sxs-lookup"><span data-stu-id="43c49-148">String</span></span>|<span data-ttu-id="43c49-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="43c49-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="43c49-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43c49-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43c49-151">version</span><span class="sxs-lookup"><span data-stu-id="43c49-151">version</span></span>|<span data-ttu-id="43c49-152">Int32</span><span class="sxs-lookup"><span data-stu-id="43c49-152">Int32</span></span>|<span data-ttu-id="43c49-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="43c49-153">Version of the device configuration.</span></span> <span data-ttu-id="43c49-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="43c49-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="43c49-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="43c49-155">allowSampleSharing</span></span>|<span data-ttu-id="43c49-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="43c49-156">Boolean</span></span>|<span data-ttu-id="43c49-157">Windows Defender AdvancedThreatProtection の "サンプルの共有を許可する" ルール</span><span class="sxs-lookup"><span data-stu-id="43c49-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="43c49-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="43c49-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="43c49-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="43c49-159">Boolean</span></span>|<span data-ttu-id="43c49-160">Windows Defender Advanced Threat Protection テレメトリ レポートの頻度を高めます。</span><span class="sxs-lookup"><span data-stu-id="43c49-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="43c49-161">応答</span><span class="sxs-lookup"><span data-stu-id="43c49-161">Response</span></span>
<span data-ttu-id="43c49-162">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="43c49-162">If successful, this method returns a `201 Created` response code and a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43c49-163">例</span><span class="sxs-lookup"><span data-stu-id="43c49-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="43c49-164">要求</span><span class="sxs-lookup"><span data-stu-id="43c49-164">Request</span></span>
<span data-ttu-id="43c49-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43c49-165">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43c49-166">応答</span><span class="sxs-lookup"><span data-stu-id="43c49-166">Response</span></span>
<span data-ttu-id="43c49-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43c49-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



