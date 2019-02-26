---
title: macOSDeviceFeaturesConfiguration の更新
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36d285a6553a127c4924b5a1606872656ef062dd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139747"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="a614f-103">macOSDeviceFeaturesConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="a614f-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="a614f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a614f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a614f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a614f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a614f-106">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a614f-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a614f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a614f-107">Prerequisites</span></span>
<span data-ttu-id="a614f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a614f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a614f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a614f-110">Permission type</span></span>|<span data-ttu-id="a614f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a614f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a614f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a614f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a614f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a614f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a614f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a614f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a614f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a614f-115">Not supported.</span></span>|
|<span data-ttu-id="a614f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a614f-116">Application</span></span>|<span data-ttu-id="a614f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a614f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a614f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a614f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a614f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a614f-119">Request headers</span></span>
|<span data-ttu-id="a614f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a614f-120">Header</span></span>|<span data-ttu-id="a614f-121">値</span><span class="sxs-lookup"><span data-stu-id="a614f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a614f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a614f-122">Authorization</span></span>|<span data-ttu-id="a614f-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a614f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a614f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a614f-124">Accept</span></span>|<span data-ttu-id="a614f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a614f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a614f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a614f-126">Request body</span></span>
<span data-ttu-id="a614f-127">要求本文で、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a614f-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="a614f-128">次の表に、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a614f-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="a614f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a614f-129">Property</span></span>|<span data-ttu-id="a614f-130">型</span><span class="sxs-lookup"><span data-stu-id="a614f-130">Type</span></span>|<span data-ttu-id="a614f-131">説明</span><span class="sxs-lookup"><span data-stu-id="a614f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a614f-132">id</span><span class="sxs-lookup"><span data-stu-id="a614f-132">id</span></span>|<span data-ttu-id="a614f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a614f-133">String</span></span>|<span data-ttu-id="a614f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a614f-134">Key of the entity.</span></span> <span data-ttu-id="a614f-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a614f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a614f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a614f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a614f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a614f-137">DateTimeOffset</span></span>|<span data-ttu-id="a614f-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a614f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a614f-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a614f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a614f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a614f-140">roleScopeTagIds</span></span>|<span data-ttu-id="a614f-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a614f-141">String collection</span></span>|<span data-ttu-id="a614f-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a614f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a614f-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a614f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a614f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a614f-144">supportsScopeTags</span></span>|<span data-ttu-id="a614f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a614f-145">Boolean</span></span>|<span data-ttu-id="a614f-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a614f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a614f-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a614f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a614f-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a614f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a614f-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a614f-149">This property is read-only.</span></span> <span data-ttu-id="a614f-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a614f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a614f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a614f-151">createdDateTime</span></span>|<span data-ttu-id="a614f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a614f-152">DateTimeOffset</span></span>|<span data-ttu-id="a614f-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a614f-153">DateTime the object was created.</span></span> <span data-ttu-id="a614f-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a614f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a614f-155">説明</span><span class="sxs-lookup"><span data-stu-id="a614f-155">description</span></span>|<span data-ttu-id="a614f-156">String</span><span class="sxs-lookup"><span data-stu-id="a614f-156">String</span></span>|<span data-ttu-id="a614f-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="a614f-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a614f-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a614f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a614f-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a614f-159">displayName</span></span>|<span data-ttu-id="a614f-160">String</span><span class="sxs-lookup"><span data-stu-id="a614f-160">String</span></span>|<span data-ttu-id="a614f-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="a614f-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a614f-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a614f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a614f-163">version</span><span class="sxs-lookup"><span data-stu-id="a614f-163">version</span></span>|<span data-ttu-id="a614f-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a614f-164">Int32</span></span>|<span data-ttu-id="a614f-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a614f-165">Version of the device configuration.</span></span> <span data-ttu-id="a614f-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a614f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a614f-167">放映した print行先</span><span class="sxs-lookup"><span data-stu-id="a614f-167">airPrintDestinations</span></span>|<span data-ttu-id="a614f-168">[放映 printdestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a614f-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="a614f-169">常に表示される必要がある、放映中の印刷プリンターの配列です。</span><span class="sxs-lookup"><span data-stu-id="a614f-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="a614f-170">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a614f-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="a614f-171">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="a614f-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a614f-172">応答</span><span class="sxs-lookup"><span data-stu-id="a614f-172">Response</span></span>
<span data-ttu-id="a614f-173">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a614f-173">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a614f-174">例</span><span class="sxs-lookup"><span data-stu-id="a614f-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="a614f-175">要求</span><span class="sxs-lookup"><span data-stu-id="a614f-175">Request</span></span>
<span data-ttu-id="a614f-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a614f-176">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a614f-177">応答</span><span class="sxs-lookup"><span data-stu-id="a614f-177">Response</span></span>
<span data-ttu-id="a614f-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a614f-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




