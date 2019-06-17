---
title: MacOSExtensionsConfiguration を作成する
description: 新しい macOSExtensionsConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e29456c5440190ebce0ff5028207f5d3851619b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963290"
---
# <a name="create-macosextensionsconfiguration"></a><span data-ttu-id="0caa9-103">MacOSExtensionsConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="0caa9-103">Create macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="0caa9-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0caa9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0caa9-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0caa9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0caa9-106">新しい[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0caa9-106">Create a new [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0caa9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0caa9-107">Prerequisites</span></span>
<span data-ttu-id="0caa9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0caa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0caa9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0caa9-110">Permission type</span></span>|<span data-ttu-id="0caa9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0caa9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0caa9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0caa9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0caa9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0caa9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0caa9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0caa9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0caa9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0caa9-115">Not supported.</span></span>|
|<span data-ttu-id="0caa9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0caa9-116">Application</span></span>|<span data-ttu-id="0caa9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0caa9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0caa9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0caa9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0caa9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0caa9-119">Request headers</span></span>
|<span data-ttu-id="0caa9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0caa9-120">Header</span></span>|<span data-ttu-id="0caa9-121">値</span><span class="sxs-lookup"><span data-stu-id="0caa9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0caa9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0caa9-122">Authorization</span></span>|<span data-ttu-id="0caa9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0caa9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0caa9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0caa9-124">Accept</span></span>|<span data-ttu-id="0caa9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0caa9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0caa9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0caa9-126">Request body</span></span>
<span data-ttu-id="0caa9-127">要求本文で、macOSExtensionsConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0caa9-127">In the request body, supply a JSON representation for the macOSExtensionsConfiguration object.</span></span>

<span data-ttu-id="0caa9-128">次の表に、macOSExtensionsConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0caa9-128">The following table shows the properties that are required when you create the macOSExtensionsConfiguration.</span></span>

|<span data-ttu-id="0caa9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0caa9-129">Property</span></span>|<span data-ttu-id="0caa9-130">型</span><span class="sxs-lookup"><span data-stu-id="0caa9-130">Type</span></span>|<span data-ttu-id="0caa9-131">説明</span><span class="sxs-lookup"><span data-stu-id="0caa9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0caa9-132">id</span><span class="sxs-lookup"><span data-stu-id="0caa9-132">id</span></span>|<span data-ttu-id="0caa9-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0caa9-133">String</span></span>|<span data-ttu-id="0caa9-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0caa9-134">Key of the entity.</span></span> <span data-ttu-id="0caa9-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0caa9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="0caa9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0caa9-137">DateTimeOffset</span></span>|<span data-ttu-id="0caa9-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="0caa9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="0caa9-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0caa9-140">roleScopeTagIds</span></span>|<span data-ttu-id="0caa9-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0caa9-141">String collection</span></span>|<span data-ttu-id="0caa9-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0caa9-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0caa9-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0caa9-144">supportsScopeTags</span></span>|<span data-ttu-id="0caa9-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="0caa9-145">Boolean</span></span>|<span data-ttu-id="0caa9-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0caa9-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0caa9-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="0caa9-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0caa9-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="0caa9-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0caa9-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="0caa9-149">This property is read-only.</span></span> <span data-ttu-id="0caa9-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0caa9-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0caa9-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0caa9-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0caa9-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="0caa9-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0caa9-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0caa9-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0caa9-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0caa9-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0caa9-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="0caa9-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0caa9-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="0caa9-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0caa9-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="0caa9-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0caa9-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="0caa9-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0caa9-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0caa9-163">createdDateTime</span></span>|<span data-ttu-id="0caa9-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0caa9-164">DateTimeOffset</span></span>|<span data-ttu-id="0caa9-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0caa9-165">DateTime the object was created.</span></span> <span data-ttu-id="0caa9-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-167">description</span><span class="sxs-lookup"><span data-stu-id="0caa9-167">description</span></span>|<span data-ttu-id="0caa9-168">String</span><span class="sxs-lookup"><span data-stu-id="0caa9-168">String</span></span>|<span data-ttu-id="0caa9-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="0caa9-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0caa9-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-171">displayName</span><span class="sxs-lookup"><span data-stu-id="0caa9-171">displayName</span></span>|<span data-ttu-id="0caa9-172">String</span><span class="sxs-lookup"><span data-stu-id="0caa9-172">String</span></span>|<span data-ttu-id="0caa9-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="0caa9-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0caa9-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-175">version</span><span class="sxs-lookup"><span data-stu-id="0caa9-175">version</span></span>|<span data-ttu-id="0caa9-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0caa9-176">Int32</span></span>|<span data-ttu-id="0caa9-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0caa9-177">Version of the device configuration.</span></span> <span data-ttu-id="0caa9-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0caa9-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0caa9-179">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="0caa9-179">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="0caa9-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="0caa9-180">Boolean</span></span>|<span data-ttu-id="0caa9-181">True に設定すると、ユーザーは、構成プロファイルで明示的に許可されていない追加のカーネル拡張機能を承認できます。</span><span class="sxs-lookup"><span data-stu-id="0caa9-181">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="0caa9-182">カーネル識別子</span><span class="sxs-lookup"><span data-stu-id="0caa9-182">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="0caa9-183">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0caa9-183">String collection</span></span>|<span data-ttu-id="0caa9-184">このリストのチーム識別子によって有効になっているすべてのカーネル拡張機能を読み込むことができます。</span><span class="sxs-lookup"><span data-stu-id="0caa9-184">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="0caa9-185">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="0caa9-185">kernelExtensionsAllowed</span></span>|<span data-ttu-id="0caa9-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0caa9-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="0caa9-187">読み込むことができるカーネル拡張機能の一覧。</span><span class="sxs-lookup"><span data-stu-id="0caa9-187">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="0caa9-188">.</span><span class="sxs-lookup"><span data-stu-id="0caa9-188"></span></span> <span data-ttu-id="0caa9-189">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0caa9-189">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0caa9-190">応答</span><span class="sxs-lookup"><span data-stu-id="0caa9-190">Response</span></span>
<span data-ttu-id="0caa9-191">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0caa9-191">If successful, this method returns a `201 Created` response code and a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0caa9-192">例</span><span class="sxs-lookup"><span data-stu-id="0caa9-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="0caa9-193">要求</span><span class="sxs-lookup"><span data-stu-id="0caa9-193">Request</span></span>
<span data-ttu-id="0caa9-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0caa9-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1383

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="0caa9-195">応答</span><span class="sxs-lookup"><span data-stu-id="0caa9-195">Response</span></span>
<span data-ttu-id="0caa9-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0caa9-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1555

{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
  "id": "c273f4f6-f4f6-c273-f6f4-73c2f6f473c2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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





