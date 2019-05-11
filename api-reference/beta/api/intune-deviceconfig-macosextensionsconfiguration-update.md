---
title: MacOSExtensionsConfiguration の更新
description: MacOSExtensionsConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 10b383b7bc6b23149bff63ba162c3a674e433969
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922776"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="e72bb-103">MacOSExtensionsConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="e72bb-103">Update macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="e72bb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e72bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e72bb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e72bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e72bb-106">[MacOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e72bb-106">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e72bb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e72bb-107">Prerequisites</span></span>
<span data-ttu-id="e72bb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e72bb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e72bb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e72bb-110">Permission type</span></span>|<span data-ttu-id="e72bb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e72bb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e72bb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e72bb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e72bb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e72bb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e72bb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e72bb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e72bb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e72bb-115">Not supported.</span></span>|
|<span data-ttu-id="e72bb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e72bb-116">Application</span></span>|<span data-ttu-id="e72bb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e72bb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e72bb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e72bb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e72bb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e72bb-119">Request headers</span></span>
|<span data-ttu-id="e72bb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e72bb-120">Header</span></span>|<span data-ttu-id="e72bb-121">値</span><span class="sxs-lookup"><span data-stu-id="e72bb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e72bb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e72bb-122">Authorization</span></span>|<span data-ttu-id="e72bb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e72bb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e72bb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e72bb-124">Accept</span></span>|<span data-ttu-id="e72bb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e72bb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e72bb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e72bb-126">Request body</span></span>
<span data-ttu-id="e72bb-127">要求本文で、 [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e72bb-127">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="e72bb-128">次の表に、 [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e72bb-128">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="e72bb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e72bb-129">Property</span></span>|<span data-ttu-id="e72bb-130">型</span><span class="sxs-lookup"><span data-stu-id="e72bb-130">Type</span></span>|<span data-ttu-id="e72bb-131">説明</span><span class="sxs-lookup"><span data-stu-id="e72bb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e72bb-132">id</span><span class="sxs-lookup"><span data-stu-id="e72bb-132">id</span></span>|<span data-ttu-id="e72bb-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e72bb-133">String</span></span>|<span data-ttu-id="e72bb-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e72bb-134">Key of the entity.</span></span> <span data-ttu-id="e72bb-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e72bb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e72bb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e72bb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e72bb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e72bb-137">DateTimeOffset</span></span>|<span data-ttu-id="e72bb-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e72bb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e72bb-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e72bb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e72bb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e72bb-140">roleScopeTagIds</span></span>|<span data-ttu-id="e72bb-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e72bb-141">String collection</span></span>|<span data-ttu-id="e72bb-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="e72bb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e72bb-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e72bb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e72bb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e72bb-144">supportsScopeTags</span></span>|<span data-ttu-id="e72bb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e72bb-145">Boolean</span></span>|<span data-ttu-id="e72bb-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e72bb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e72bb-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e72bb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e72bb-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="e72bb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e72bb-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e72bb-149">This property is read-only.</span></span> <span data-ttu-id="e72bb-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e72bb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e72bb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e72bb-151">createdDateTime</span></span>|<span data-ttu-id="e72bb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e72bb-152">DateTimeOffset</span></span>|<span data-ttu-id="e72bb-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e72bb-153">DateTime the object was created.</span></span> <span data-ttu-id="e72bb-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e72bb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e72bb-155">description</span><span class="sxs-lookup"><span data-stu-id="e72bb-155">description</span></span>|<span data-ttu-id="e72bb-156">String</span><span class="sxs-lookup"><span data-stu-id="e72bb-156">String</span></span>|<span data-ttu-id="e72bb-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="e72bb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e72bb-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e72bb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e72bb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e72bb-159">displayName</span></span>|<span data-ttu-id="e72bb-160">String</span><span class="sxs-lookup"><span data-stu-id="e72bb-160">String</span></span>|<span data-ttu-id="e72bb-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e72bb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e72bb-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e72bb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e72bb-163">version</span><span class="sxs-lookup"><span data-stu-id="e72bb-163">version</span></span>|<span data-ttu-id="e72bb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e72bb-164">Int32</span></span>|<span data-ttu-id="e72bb-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e72bb-165">Version of the device configuration.</span></span> <span data-ttu-id="e72bb-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e72bb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e72bb-167">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="e72bb-167">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="e72bb-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="e72bb-168">Boolean</span></span>|<span data-ttu-id="e72bb-169">True に設定すると、ユーザーは、構成プロファイルで明示的に許可されていない追加のカーネル拡張機能を承認できます。</span><span class="sxs-lookup"><span data-stu-id="e72bb-169">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="e72bb-170">カーネル識別子</span><span class="sxs-lookup"><span data-stu-id="e72bb-170">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="e72bb-171">String collection</span><span class="sxs-lookup"><span data-stu-id="e72bb-171">String collection</span></span>|<span data-ttu-id="e72bb-172">このリストのチーム識別子によって有効になっているすべてのカーネル拡張機能を読み込むことができます。</span><span class="sxs-lookup"><span data-stu-id="e72bb-172">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="e72bb-173">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="e72bb-173">kernelExtensionsAllowed</span></span>|<span data-ttu-id="e72bb-174">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e72bb-174">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="e72bb-175">読み込むことができるカーネル拡張機能の一覧。</span><span class="sxs-lookup"><span data-stu-id="e72bb-175">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="e72bb-176">.</span><span class="sxs-lookup"><span data-stu-id="e72bb-176"></span></span> <span data-ttu-id="e72bb-177">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e72bb-177">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="e72bb-178">応答</span><span class="sxs-lookup"><span data-stu-id="e72bb-178">Response</span></span>
<span data-ttu-id="e72bb-179">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e72bb-179">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e72bb-180">例</span><span class="sxs-lookup"><span data-stu-id="e72bb-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="e72bb-181">要求</span><span class="sxs-lookup"><span data-stu-id="e72bb-181">Request</span></span>
<span data-ttu-id="e72bb-182">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e72bb-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 610

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="e72bb-183">応答</span><span class="sxs-lookup"><span data-stu-id="e72bb-183">Response</span></span>
<span data-ttu-id="e72bb-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e72bb-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 782

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "Kernel Extension Allowed Team Identifiers value"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "Team Identifier value",
      "bundleId": "Bundle Id value"
    }
  ]
}
```




