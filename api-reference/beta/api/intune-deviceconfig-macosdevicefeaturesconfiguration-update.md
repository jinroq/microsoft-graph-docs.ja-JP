---
title: macOSDeviceFeaturesConfiguration の更新
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cdd65480ee4ce29ded7c841cd1ac33d59c05d974
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957886"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="9e914-103">macOSDeviceFeaturesConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="9e914-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="9e914-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e914-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e914-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e914-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e914-106">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9e914-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e914-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e914-107">Prerequisites</span></span>
<span data-ttu-id="9e914-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e914-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e914-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e914-110">Permission type</span></span>|<span data-ttu-id="9e914-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e914-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e914-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e914-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e914-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e914-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e914-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e914-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e914-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e914-115">Not supported.</span></span>|
|<span data-ttu-id="9e914-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e914-116">Application</span></span>|<span data-ttu-id="9e914-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e914-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e914-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e914-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9e914-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e914-119">Request headers</span></span>
|<span data-ttu-id="9e914-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e914-120">Header</span></span>|<span data-ttu-id="9e914-121">値</span><span class="sxs-lookup"><span data-stu-id="9e914-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e914-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e914-122">Authorization</span></span>|<span data-ttu-id="9e914-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9e914-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e914-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9e914-124">Accept</span></span>|<span data-ttu-id="9e914-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e914-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e914-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e914-126">Request body</span></span>
<span data-ttu-id="9e914-127">要求本文で、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e914-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="9e914-128">次の表に、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9e914-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="9e914-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e914-129">Property</span></span>|<span data-ttu-id="9e914-130">型</span><span class="sxs-lookup"><span data-stu-id="9e914-130">Type</span></span>|<span data-ttu-id="9e914-131">説明</span><span class="sxs-lookup"><span data-stu-id="9e914-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e914-132">id</span><span class="sxs-lookup"><span data-stu-id="9e914-132">id</span></span>|<span data-ttu-id="9e914-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9e914-133">String</span></span>|<span data-ttu-id="9e914-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9e914-134">Key of the entity.</span></span> <span data-ttu-id="9e914-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e914-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e914-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e914-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9e914-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e914-137">DateTimeOffset</span></span>|<span data-ttu-id="9e914-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="9e914-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9e914-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e914-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e914-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e914-140">roleScopeTagIds</span></span>|<span data-ttu-id="9e914-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9e914-141">String collection</span></span>|<span data-ttu-id="9e914-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="9e914-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9e914-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e914-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e914-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9e914-144">supportsScopeTags</span></span>|<span data-ttu-id="9e914-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e914-145">Boolean</span></span>|<span data-ttu-id="9e914-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9e914-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9e914-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="9e914-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9e914-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="9e914-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9e914-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9e914-149">This property is read-only.</span></span> <span data-ttu-id="9e914-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e914-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e914-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e914-151">createdDateTime</span></span>|<span data-ttu-id="9e914-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e914-152">DateTimeOffset</span></span>|<span data-ttu-id="9e914-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9e914-153">DateTime the object was created.</span></span> <span data-ttu-id="9e914-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e914-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e914-155">description</span><span class="sxs-lookup"><span data-stu-id="9e914-155">description</span></span>|<span data-ttu-id="9e914-156">String</span><span class="sxs-lookup"><span data-stu-id="9e914-156">String</span></span>|<span data-ttu-id="9e914-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="9e914-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9e914-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e914-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e914-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9e914-159">displayName</span></span>|<span data-ttu-id="9e914-160">String</span><span class="sxs-lookup"><span data-stu-id="9e914-160">String</span></span>|<span data-ttu-id="9e914-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="9e914-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9e914-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e914-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e914-163">version</span><span class="sxs-lookup"><span data-stu-id="9e914-163">version</span></span>|<span data-ttu-id="9e914-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9e914-164">Int32</span></span>|<span data-ttu-id="9e914-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9e914-165">Version of the device configuration.</span></span> <span data-ttu-id="9e914-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9e914-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e914-167">放映した print行先</span><span class="sxs-lookup"><span data-stu-id="9e914-167">airPrintDestinations</span></span>|<span data-ttu-id="9e914-168">[放映 printdestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9e914-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="9e914-169">常に表示される必要がある、放映中の印刷プリンターの配列です。</span><span class="sxs-lookup"><span data-stu-id="9e914-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="9e914-170">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9e914-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="9e914-171">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9e914-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="9e914-172">応答</span><span class="sxs-lookup"><span data-stu-id="9e914-172">Response</span></span>
<span data-ttu-id="9e914-173">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9e914-173">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e914-174">例</span><span class="sxs-lookup"><span data-stu-id="9e914-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e914-175">要求</span><span class="sxs-lookup"><span data-stu-id="9e914-175">Request</span></span>
<span data-ttu-id="9e914-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e914-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 500

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="9e914-177">応答</span><span class="sxs-lookup"><span data-stu-id="9e914-177">Response</span></span>
<span data-ttu-id="9e914-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e914-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 672

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```




