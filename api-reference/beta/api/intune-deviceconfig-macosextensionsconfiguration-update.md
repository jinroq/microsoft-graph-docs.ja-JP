---
title: MacOSExtensionsConfiguration の更新
description: MacOSExtensionsConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e78c317496ee9e116e9319a0ff28ca8a7478224
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963227"
---
# <a name="update-macosextensionsconfiguration"></a><span data-ttu-id="9b46a-103">MacOSExtensionsConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="9b46a-103">Update macOSExtensionsConfiguration</span></span>

> <span data-ttu-id="9b46a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b46a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b46a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b46a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b46a-106">[MacOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9b46a-106">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9b46a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9b46a-107">Prerequisites</span></span>
<span data-ttu-id="9b46a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b46a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b46a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9b46a-110">Permission type</span></span>|<span data-ttu-id="9b46a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9b46a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9b46a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9b46a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9b46a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b46a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9b46a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9b46a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9b46a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b46a-115">Not supported.</span></span>|
|<span data-ttu-id="9b46a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9b46a-116">Application</span></span>|<span data-ttu-id="9b46a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9b46a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b46a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9b46a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9b46a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b46a-119">Request headers</span></span>
|<span data-ttu-id="9b46a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9b46a-120">Header</span></span>|<span data-ttu-id="9b46a-121">値</span><span class="sxs-lookup"><span data-stu-id="9b46a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9b46a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b46a-122">Authorization</span></span>|<span data-ttu-id="9b46a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9b46a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9b46a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9b46a-124">Accept</span></span>|<span data-ttu-id="9b46a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9b46a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9b46a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9b46a-126">Request body</span></span>
<span data-ttu-id="9b46a-127">要求本文で、 [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9b46a-127">In the request body, supply a JSON representation for the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>

<span data-ttu-id="9b46a-128">次の表に、 [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9b46a-128">The following table shows the properties that are required when you create the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>

|<span data-ttu-id="9b46a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b46a-129">Property</span></span>|<span data-ttu-id="9b46a-130">型</span><span class="sxs-lookup"><span data-stu-id="9b46a-130">Type</span></span>|<span data-ttu-id="9b46a-131">説明</span><span class="sxs-lookup"><span data-stu-id="9b46a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b46a-132">id</span><span class="sxs-lookup"><span data-stu-id="9b46a-132">id</span></span>|<span data-ttu-id="9b46a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="9b46a-133">String</span></span>|<span data-ttu-id="9b46a-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9b46a-134">Key of the entity.</span></span> <span data-ttu-id="9b46a-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9b46a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9b46a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b46a-137">DateTimeOffset</span></span>|<span data-ttu-id="9b46a-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="9b46a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9b46a-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9b46a-140">roleScopeTagIds</span></span>|<span data-ttu-id="9b46a-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9b46a-141">String collection</span></span>|<span data-ttu-id="9b46a-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="9b46a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9b46a-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9b46a-144">supportsScopeTags</span></span>|<span data-ttu-id="9b46a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b46a-145">Boolean</span></span>|<span data-ttu-id="9b46a-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9b46a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9b46a-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="9b46a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9b46a-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="9b46a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9b46a-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9b46a-149">This property is read-only.</span></span> <span data-ttu-id="9b46a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9b46a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="9b46a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="9b46a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="9b46a-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="9b46a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="9b46a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9b46a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="9b46a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="9b46a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="9b46a-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="9b46a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="9b46a-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="9b46a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="9b46a-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="9b46a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="9b46a-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="9b46a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="9b46a-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9b46a-163">createdDateTime</span></span>|<span data-ttu-id="9b46a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9b46a-164">DateTimeOffset</span></span>|<span data-ttu-id="9b46a-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9b46a-165">DateTime the object was created.</span></span> <span data-ttu-id="9b46a-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-167">description</span><span class="sxs-lookup"><span data-stu-id="9b46a-167">description</span></span>|<span data-ttu-id="9b46a-168">String</span><span class="sxs-lookup"><span data-stu-id="9b46a-168">String</span></span>|<span data-ttu-id="9b46a-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="9b46a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9b46a-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="9b46a-171">displayName</span></span>|<span data-ttu-id="9b46a-172">String</span><span class="sxs-lookup"><span data-stu-id="9b46a-172">String</span></span>|<span data-ttu-id="9b46a-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="9b46a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9b46a-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-175">version</span><span class="sxs-lookup"><span data-stu-id="9b46a-175">version</span></span>|<span data-ttu-id="9b46a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="9b46a-176">Int32</span></span>|<span data-ttu-id="9b46a-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9b46a-177">Version of the device configuration.</span></span> <span data-ttu-id="9b46a-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9b46a-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9b46a-179">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="9b46a-179">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="9b46a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b46a-180">Boolean</span></span>|<span data-ttu-id="9b46a-181">True に設定すると、ユーザーは、構成プロファイルで明示的に許可されていない追加のカーネル拡張機能を承認できます。</span><span class="sxs-lookup"><span data-stu-id="9b46a-181">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="9b46a-182">カーネル識別子</span><span class="sxs-lookup"><span data-stu-id="9b46a-182">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="9b46a-183">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="9b46a-183">String collection</span></span>|<span data-ttu-id="9b46a-184">このリストのチーム識別子によって有効になっているすべてのカーネル拡張機能を読み込むことができます。</span><span class="sxs-lookup"><span data-stu-id="9b46a-184">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="9b46a-185">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="9b46a-185">kernelExtensionsAllowed</span></span>|<span data-ttu-id="9b46a-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9b46a-186">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="9b46a-187">読み込むことができるカーネル拡張機能の一覧。</span><span class="sxs-lookup"><span data-stu-id="9b46a-187">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="9b46a-188">.</span><span class="sxs-lookup"><span data-stu-id="9b46a-188"></span></span> <span data-ttu-id="9b46a-189">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9b46a-189">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="9b46a-190">応答</span><span class="sxs-lookup"><span data-stu-id="9b46a-190">Response</span></span>
<span data-ttu-id="9b46a-191">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9b46a-191">If successful, this method returns a `200 OK` response code and an updated [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b46a-192">例</span><span class="sxs-lookup"><span data-stu-id="9b46a-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="9b46a-193">要求</span><span class="sxs-lookup"><span data-stu-id="9b46a-193">Request</span></span>
<span data-ttu-id="9b46a-194">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9b46a-194">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="9b46a-195">応答</span><span class="sxs-lookup"><span data-stu-id="9b46a-195">Response</span></span>
<span data-ttu-id="9b46a-p114">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9b46a-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





