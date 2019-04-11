---
title: アン supporteddevicの作成
description: 新しいアン supporteddevic/オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e6012a286a98f676986fb8cb4aa6bb45948f50c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797600"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="a0b94-103">アン supporteddevicの作成</span><span class="sxs-lookup"><span data-stu-id="a0b94-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="a0b94-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0b94-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0b94-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0b94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0b94-106">新しい[アン supporteddevic/](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a0b94-106">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0b94-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a0b94-107">Prerequisites</span></span>
<span data-ttu-id="a0b94-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a0b94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0b94-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a0b94-110">Permission type</span></span>|<span data-ttu-id="a0b94-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a0b94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0b94-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a0b94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0b94-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0b94-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0b94-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a0b94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0b94-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0b94-115">Not supported.</span></span>|
|<span data-ttu-id="a0b94-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a0b94-116">Application</span></span>|<span data-ttu-id="a0b94-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0b94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0b94-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a0b94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a0b94-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0b94-119">Request headers</span></span>
|<span data-ttu-id="a0b94-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0b94-120">Header</span></span>|<span data-ttu-id="a0b94-121">値</span><span class="sxs-lookup"><span data-stu-id="a0b94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0b94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0b94-122">Authorization</span></span>|<span data-ttu-id="a0b94-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0b94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0b94-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a0b94-124">Accept</span></span>|<span data-ttu-id="a0b94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0b94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0b94-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a0b94-126">Request body</span></span>
<span data-ttu-id="a0b94-127">要求本文で、アン supporteddevic/オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a0b94-127">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="a0b94-128">次の表に、アン supporteddevicの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a0b94-128">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="a0b94-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0b94-129">Property</span></span>|<span data-ttu-id="a0b94-130">型</span><span class="sxs-lookup"><span data-stu-id="a0b94-130">Type</span></span>|<span data-ttu-id="a0b94-131">説明</span><span class="sxs-lookup"><span data-stu-id="a0b94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0b94-132">id</span><span class="sxs-lookup"><span data-stu-id="a0b94-132">id</span></span>|<span data-ttu-id="a0b94-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a0b94-133">String</span></span>|<span data-ttu-id="a0b94-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a0b94-134">Key of the entity.</span></span> <span data-ttu-id="a0b94-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a0b94-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b94-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a0b94-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a0b94-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0b94-137">DateTimeOffset</span></span>|<span data-ttu-id="a0b94-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a0b94-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a0b94-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a0b94-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b94-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a0b94-140">roleScopeTagIds</span></span>|<span data-ttu-id="a0b94-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a0b94-141">String collection</span></span>|<span data-ttu-id="a0b94-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="a0b94-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a0b94-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a0b94-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b94-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a0b94-144">supportsScopeTags</span></span>|<span data-ttu-id="a0b94-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a0b94-145">Boolean</span></span>|<span data-ttu-id="a0b94-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a0b94-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a0b94-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="a0b94-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a0b94-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="a0b94-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a0b94-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="a0b94-149">This property is read-only.</span></span> <span data-ttu-id="a0b94-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a0b94-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b94-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0b94-151">createdDateTime</span></span>|<span data-ttu-id="a0b94-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0b94-152">DateTimeOffset</span></span>|<span data-ttu-id="a0b94-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a0b94-153">DateTime the object was created.</span></span> <span data-ttu-id="a0b94-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a0b94-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b94-155">説明</span><span class="sxs-lookup"><span data-stu-id="a0b94-155">description</span></span>|<span data-ttu-id="a0b94-156">String</span><span class="sxs-lookup"><span data-stu-id="a0b94-156">String</span></span>|<span data-ttu-id="a0b94-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="a0b94-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a0b94-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a0b94-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b94-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a0b94-159">displayName</span></span>|<span data-ttu-id="a0b94-160">String</span><span class="sxs-lookup"><span data-stu-id="a0b94-160">String</span></span>|<span data-ttu-id="a0b94-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="a0b94-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a0b94-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a0b94-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b94-163">version</span><span class="sxs-lookup"><span data-stu-id="a0b94-163">version</span></span>|<span data-ttu-id="a0b94-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a0b94-164">Int32</span></span>|<span data-ttu-id="a0b94-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a0b94-165">Version of the device configuration.</span></span> <span data-ttu-id="a0b94-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a0b94-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a0b94-167">originalentitytypename</span><span class="sxs-lookup"><span data-stu-id="a0b94-167">originalEntityTypeName</span></span>|<span data-ttu-id="a0b94-168">文字列</span><span class="sxs-lookup"><span data-stu-id="a0b94-168">String</span></span>|<span data-ttu-id="a0b94-169">それ以外の場合に返されるエンティティの種類。</span><span class="sxs-lookup"><span data-stu-id="a0b94-169">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="a0b94-170">詳細</span><span class="sxs-lookup"><span data-stu-id="a0b94-170">details</span></span>|<span data-ttu-id="a0b94-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a0b94-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="a0b94-172">エンティティがサポートされていない理由について説明します。</span><span class="sxs-lookup"><span data-stu-id="a0b94-172">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="a0b94-173">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a0b94-173">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a0b94-174">応答</span><span class="sxs-lookup"><span data-stu-id="a0b94-174">Response</span></span>
<span data-ttu-id="a0b94-175">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[アン supporteddevicの](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a0b94-175">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0b94-176">例</span><span class="sxs-lookup"><span data-stu-id="a0b94-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0b94-177">要求</span><span class="sxs-lookup"><span data-stu-id="a0b94-177">Request</span></span>
<span data-ttu-id="a0b94-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a0b94-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="a0b94-179">応答</span><span class="sxs-lookup"><span data-stu-id="a0b94-179">Response</span></span>
<span data-ttu-id="a0b94-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a0b94-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 690

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```





