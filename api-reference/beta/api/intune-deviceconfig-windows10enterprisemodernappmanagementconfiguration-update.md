---
title: windows10EnterpriseModernAppManagementConfiguration の更新
description: windows10EnterpriseModernAppManagementConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 454c17f80466bfb0d348991072f073eccfe6e59c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159158"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="28529-103">windows10EnterpriseModernAppManagementConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="28529-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="28529-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28529-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28529-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="28529-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28529-106">[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="28529-106">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28529-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="28529-107">Prerequisites</span></span>
<span data-ttu-id="28529-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28529-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28529-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28529-110">Permission type</span></span>|<span data-ttu-id="28529-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="28529-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28529-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28529-112">Delegated (work or school account)</span></span>|<span data-ttu-id="28529-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28529-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28529-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28529-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28529-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28529-115">Not supported.</span></span>|
|<span data-ttu-id="28529-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28529-116">Application</span></span>|<span data-ttu-id="28529-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28529-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28529-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28529-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="28529-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28529-119">Request headers</span></span>
|<span data-ttu-id="28529-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28529-120">Header</span></span>|<span data-ttu-id="28529-121">値</span><span class="sxs-lookup"><span data-stu-id="28529-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28529-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="28529-122">Authorization</span></span>|<span data-ttu-id="28529-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="28529-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28529-124">承諾</span><span class="sxs-lookup"><span data-stu-id="28529-124">Accept</span></span>|<span data-ttu-id="28529-125">application/json</span><span class="sxs-lookup"><span data-stu-id="28529-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28529-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="28529-126">Request body</span></span>
<span data-ttu-id="28529-127">要求本文で、[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="28529-127">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="28529-128">次の表に、[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="28529-128">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="28529-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28529-129">Property</span></span>|<span data-ttu-id="28529-130">型</span><span class="sxs-lookup"><span data-stu-id="28529-130">Type</span></span>|<span data-ttu-id="28529-131">説明</span><span class="sxs-lookup"><span data-stu-id="28529-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28529-132">id</span><span class="sxs-lookup"><span data-stu-id="28529-132">id</span></span>|<span data-ttu-id="28529-133">文字列</span><span class="sxs-lookup"><span data-stu-id="28529-133">String</span></span>|<span data-ttu-id="28529-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="28529-134">Key of the entity.</span></span> <span data-ttu-id="28529-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="28529-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28529-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="28529-136">lastModifiedDateTime</span></span>|<span data-ttu-id="28529-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28529-137">DateTimeOffset</span></span>|<span data-ttu-id="28529-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="28529-138">DateTime the object was last modified.</span></span> <span data-ttu-id="28529-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="28529-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28529-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="28529-140">roleScopeTagIds</span></span>|<span data-ttu-id="28529-141">String collection</span><span class="sxs-lookup"><span data-stu-id="28529-141">String collection</span></span>|<span data-ttu-id="28529-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="28529-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="28529-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="28529-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28529-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="28529-144">supportsScopeTags</span></span>|<span data-ttu-id="28529-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="28529-145">Boolean</span></span>|<span data-ttu-id="28529-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="28529-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="28529-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="28529-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="28529-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="28529-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="28529-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="28529-149">This property is read-only.</span></span> <span data-ttu-id="28529-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="28529-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28529-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="28529-151">createdDateTime</span></span>|<span data-ttu-id="28529-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28529-152">DateTimeOffset</span></span>|<span data-ttu-id="28529-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="28529-153">DateTime the object was created.</span></span> <span data-ttu-id="28529-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="28529-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28529-155">説明</span><span class="sxs-lookup"><span data-stu-id="28529-155">description</span></span>|<span data-ttu-id="28529-156">String</span><span class="sxs-lookup"><span data-stu-id="28529-156">String</span></span>|<span data-ttu-id="28529-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="28529-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="28529-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="28529-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28529-159">displayName</span><span class="sxs-lookup"><span data-stu-id="28529-159">displayName</span></span>|<span data-ttu-id="28529-160">String</span><span class="sxs-lookup"><span data-stu-id="28529-160">String</span></span>|<span data-ttu-id="28529-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="28529-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="28529-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="28529-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28529-163">version</span><span class="sxs-lookup"><span data-stu-id="28529-163">version</span></span>|<span data-ttu-id="28529-164">Int32</span><span class="sxs-lookup"><span data-stu-id="28529-164">Int32</span></span>|<span data-ttu-id="28529-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="28529-165">Version of the device configuration.</span></span> <span data-ttu-id="28529-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="28529-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="28529-167">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="28529-167">uninstallBuiltInApps</span></span>|<span data-ttu-id="28529-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="28529-168">Boolean</span></span>|<span data-ttu-id="28529-169">組み込みの Windows アプリの固定リストをアンインストールするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="28529-169">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="28529-170">応答</span><span class="sxs-lookup"><span data-stu-id="28529-170">Response</span></span>
<span data-ttu-id="28529-171">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="28529-171">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28529-172">例</span><span class="sxs-lookup"><span data-stu-id="28529-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="28529-173">要求</span><span class="sxs-lookup"><span data-stu-id="28529-173">Request</span></span>
<span data-ttu-id="28529-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="28529-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="28529-175">応答</span><span class="sxs-lookup"><span data-stu-id="28529-175">Response</span></span>
<span data-ttu-id="28529-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="28529-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```




