---
title: windowsDefenderAdvancedThreatProtectionConfiguration の更新
description: windowsDefenderAdvancedThreatProtectionConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 49e8a1fb44933d3ff43c38f1b4b3b0e71a6a7b2d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319832"
---
# <a name="update-windowsdefenderadvancedthreatprotectionconfiguration"></a><span data-ttu-id="0bac0-103">windowsDefenderAdvancedThreatProtectionConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="0bac0-103">Update windowsDefenderAdvancedThreatProtectionConfiguration</span></span>

> <span data-ttu-id="0bac0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0bac0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bac0-105">[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0bac0-105">Update the properties of a [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bac0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="0bac0-106">Prerequisites</span></span>
<span data-ttu-id="0bac0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bac0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bac0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bac0-109">Permission type</span></span>|<span data-ttu-id="0bac0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bac0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bac0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bac0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0bac0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0bac0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0bac0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bac0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bac0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bac0-114">Not supported.</span></span>|
|<span data-ttu-id="0bac0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bac0-115">Application</span></span>|<span data-ttu-id="0bac0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bac0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bac0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0bac0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0bac0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bac0-118">Request headers</span></span>
|<span data-ttu-id="0bac0-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bac0-119">Header</span></span>|<span data-ttu-id="0bac0-120">値</span><span class="sxs-lookup"><span data-stu-id="0bac0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bac0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bac0-121">Authorization</span></span>|<span data-ttu-id="0bac0-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0bac0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bac0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="0bac0-123">Accept</span></span>|<span data-ttu-id="0bac0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0bac0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bac0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0bac0-125">Request body</span></span>
<span data-ttu-id="0bac0-126">要求本文で、[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0bac0-126">In the request body, supply a JSON representation for the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="0bac0-127">次の表に、[windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0bac0-127">The following table shows the properties that are required when you create the [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md).</span></span>

|<span data-ttu-id="0bac0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0bac0-128">Property</span></span>|<span data-ttu-id="0bac0-129">種類</span><span class="sxs-lookup"><span data-stu-id="0bac0-129">Type</span></span>|<span data-ttu-id="0bac0-130">説明</span><span class="sxs-lookup"><span data-stu-id="0bac0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bac0-131">ID</span><span class="sxs-lookup"><span data-stu-id="0bac0-131">id</span></span>|<span data-ttu-id="0bac0-132">String</span><span class="sxs-lookup"><span data-stu-id="0bac0-132">String</span></span>|<span data-ttu-id="0bac0-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0bac0-133">Key of the entity.</span></span> <span data-ttu-id="0bac0-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bac0-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bac0-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0bac0-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0bac0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bac0-136">DateTimeOffset</span></span>|<span data-ttu-id="0bac0-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0bac0-137">DateTime the object was last modified.</span></span> <span data-ttu-id="0bac0-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bac0-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bac0-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0bac0-139">createdDateTime</span></span>|<span data-ttu-id="0bac0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0bac0-140">DateTimeOffset</span></span>|<span data-ttu-id="0bac0-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0bac0-141">DateTime the object was created.</span></span> <span data-ttu-id="0bac0-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bac0-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bac0-143">説明</span><span class="sxs-lookup"><span data-stu-id="0bac0-143">description</span></span>|<span data-ttu-id="0bac0-144">String</span><span class="sxs-lookup"><span data-stu-id="0bac0-144">String</span></span>|<span data-ttu-id="0bac0-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="0bac0-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0bac0-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bac0-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bac0-147">displayName</span><span class="sxs-lookup"><span data-stu-id="0bac0-147">displayName</span></span>|<span data-ttu-id="0bac0-148">String</span><span class="sxs-lookup"><span data-stu-id="0bac0-148">String</span></span>|<span data-ttu-id="0bac0-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="0bac0-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0bac0-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bac0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bac0-151">version</span><span class="sxs-lookup"><span data-stu-id="0bac0-151">version</span></span>|<span data-ttu-id="0bac0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0bac0-152">Int32</span></span>|<span data-ttu-id="0bac0-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0bac0-153">Version of the device configuration.</span></span> <span data-ttu-id="0bac0-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0bac0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0bac0-155">allowSampleSharing</span><span class="sxs-lookup"><span data-stu-id="0bac0-155">allowSampleSharing</span></span>|<span data-ttu-id="0bac0-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bac0-156">Boolean</span></span>|<span data-ttu-id="0bac0-157">Windows Defender AdvancedThreatProtection の "サンプルの共有を許可する" ルール</span><span class="sxs-lookup"><span data-stu-id="0bac0-157">Windows Defender AdvancedThreatProtection "Allow Sample Sharing" Rule</span></span>|
|<span data-ttu-id="0bac0-158">enableExpeditedTelemetryReporting</span><span class="sxs-lookup"><span data-stu-id="0bac0-158">enableExpeditedTelemetryReporting</span></span>|<span data-ttu-id="0bac0-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bac0-159">Boolean</span></span>|<span data-ttu-id="0bac0-160">Windows Defender Advanced Threat Protection テレメトリ レポートの頻度を高めます。</span><span class="sxs-lookup"><span data-stu-id="0bac0-160">Expedite Windows Defender Advanced Threat Protection telemetry reporting frequency.</span></span>|



## <a name="response"></a><span data-ttu-id="0bac0-161">応答</span><span class="sxs-lookup"><span data-stu-id="0bac0-161">Response</span></span>
<span data-ttu-id="0bac0-162">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0bac0-162">If successful, this method returns a `200 OK` response code and an updated [windowsDefenderAdvancedThreatProtectionConfiguration](../resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bac0-163">例</span><span class="sxs-lookup"><span data-stu-id="0bac0-163">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bac0-164">要求</span><span class="sxs-lookup"><span data-stu-id="0bac0-164">Request</span></span>
<span data-ttu-id="0bac0-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0bac0-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="0bac0-166">応答</span><span class="sxs-lookup"><span data-stu-id="0bac0-166">Response</span></span>
<span data-ttu-id="0bac0-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0bac0-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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


