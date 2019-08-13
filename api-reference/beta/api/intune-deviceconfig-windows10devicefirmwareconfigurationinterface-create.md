---
title: Windows10DeviceFirmwareConfigurationInterface を作成する
description: 新しい windows10DeviceFirmwareConfigurationInterface オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 998935ac319a0ecd1643e70ca7c4d5da0d0a9806
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314680"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a><span data-ttu-id="fea7f-103">Windows10DeviceFirmwareConfigurationInterface を作成する</span><span class="sxs-lookup"><span data-stu-id="fea7f-103">Create windows10DeviceFirmwareConfigurationInterface</span></span>

> <span data-ttu-id="fea7f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fea7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fea7f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fea7f-106">新しい[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-106">Create a new [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fea7f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fea7f-107">Prerequisites</span></span>
<span data-ttu-id="fea7f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fea7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fea7f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fea7f-110">Permission type</span></span>|<span data-ttu-id="fea7f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fea7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fea7f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fea7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fea7f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea7f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fea7f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fea7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fea7f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fea7f-115">Not supported.</span></span>|
|<span data-ttu-id="fea7f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fea7f-116">Application</span></span>|<span data-ttu-id="fea7f-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fea7f-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fea7f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fea7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fea7f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fea7f-119">Request headers</span></span>
|<span data-ttu-id="fea7f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fea7f-120">Header</span></span>|<span data-ttu-id="fea7f-121">値</span><span class="sxs-lookup"><span data-stu-id="fea7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fea7f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fea7f-122">Authorization</span></span>|<span data-ttu-id="fea7f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fea7f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fea7f-124">Accept</span></span>|<span data-ttu-id="fea7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fea7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fea7f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fea7f-126">Request body</span></span>
<span data-ttu-id="fea7f-127">要求本文で、windows10DeviceFirmwareConfigurationInterface オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-127">In the request body, supply a JSON representation for the windows10DeviceFirmwareConfigurationInterface object.</span></span>

<span data-ttu-id="fea7f-128">次の表に、windows10DeviceFirmwareConfigurationInterface の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-128">The following table shows the properties that are required when you create the windows10DeviceFirmwareConfigurationInterface.</span></span>

|<span data-ttu-id="fea7f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fea7f-129">Property</span></span>|<span data-ttu-id="fea7f-130">型</span><span class="sxs-lookup"><span data-stu-id="fea7f-130">Type</span></span>|<span data-ttu-id="fea7f-131">説明</span><span class="sxs-lookup"><span data-stu-id="fea7f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fea7f-132">id</span><span class="sxs-lookup"><span data-stu-id="fea7f-132">id</span></span>|<span data-ttu-id="fea7f-133">文字列</span><span class="sxs-lookup"><span data-stu-id="fea7f-133">String</span></span>|<span data-ttu-id="fea7f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fea7f-134">Key of the entity.</span></span> <span data-ttu-id="fea7f-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fea7f-136">lastModifiedDateTime</span></span>|<span data-ttu-id="fea7f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea7f-137">DateTimeOffset</span></span>|<span data-ttu-id="fea7f-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="fea7f-138">DateTime the object was last modified.</span></span> <span data-ttu-id="fea7f-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="fea7f-140">roleScopeTagIds</span></span>|<span data-ttu-id="fea7f-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="fea7f-141">String collection</span></span>|<span data-ttu-id="fea7f-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="fea7f-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="fea7f-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="fea7f-144">supportsScopeTags</span></span>|<span data-ttu-id="fea7f-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="fea7f-145">Boolean</span></span>|<span data-ttu-id="fea7f-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="fea7f-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="fea7f-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="fea7f-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="fea7f-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="fea7f-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-149">This property is read-only.</span></span> <span data-ttu-id="fea7f-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fea7f-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="fea7f-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="fea7f-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="fea7f-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="fea7f-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="fea7f-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fea7f-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="fea7f-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="fea7f-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="fea7f-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="fea7f-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="fea7f-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="fea7f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="fea7f-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="fea7f-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="fea7f-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="fea7f-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="fea7f-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fea7f-163">createdDateTime</span></span>|<span data-ttu-id="fea7f-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea7f-164">DateTimeOffset</span></span>|<span data-ttu-id="fea7f-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="fea7f-165">DateTime the object was created.</span></span> <span data-ttu-id="fea7f-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-167">description</span><span class="sxs-lookup"><span data-stu-id="fea7f-167">description</span></span>|<span data-ttu-id="fea7f-168">String</span><span class="sxs-lookup"><span data-stu-id="fea7f-168">String</span></span>|<span data-ttu-id="fea7f-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="fea7f-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="fea7f-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-171">displayName</span><span class="sxs-lookup"><span data-stu-id="fea7f-171">displayName</span></span>|<span data-ttu-id="fea7f-172">String</span><span class="sxs-lookup"><span data-stu-id="fea7f-172">String</span></span>|<span data-ttu-id="fea7f-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="fea7f-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="fea7f-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-175">version</span><span class="sxs-lookup"><span data-stu-id="fea7f-175">version</span></span>|<span data-ttu-id="fea7f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="fea7f-176">Int32</span></span>|<span data-ttu-id="fea7f-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="fea7f-177">Version of the device configuration.</span></span> <span data-ttu-id="fea7f-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="fea7f-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="fea7f-179">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="fea7f-179">changeUefiSettingsPermission</span></span>|[<span data-ttu-id="fea7f-180">changeUefiSettingsPermission</span><span class="sxs-lookup"><span data-stu-id="fea7f-180">changeUefiSettingsPermission</span></span>](../resources/intune-deviceconfig-changeuefisettingspermission.md)|<span data-ttu-id="fea7f-181">ユーザーに対して、UEFI 設定を変更するために付与されるアクセス許可レベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-181">Defines the permission level granted to users to change UEFI settings.</span></span> <span data-ttu-id="fea7f-182">可能な値は、`notConfiguredOnly`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-182">Possible values are: `notConfiguredOnly`, `none`.</span></span>|
|<span data-ttu-id="fea7f-183">virtualizationOfCpuAndIO</span><span class="sxs-lookup"><span data-stu-id="fea7f-183">virtualizationOfCpuAndIO</span></span>|[<span data-ttu-id="fea7f-184">購入</span><span class="sxs-lookup"><span data-stu-id="fea7f-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="fea7f-185">CPU と IO の仮想化を有効にするかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-185">Defines whether CPU and IO virtualization is enabled.</span></span> <span data-ttu-id="fea7f-186">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="fea7f-187">撮影</span><span class="sxs-lookup"><span data-stu-id="fea7f-187">cameras</span></span>|[<span data-ttu-id="fea7f-188">購入</span><span class="sxs-lookup"><span data-stu-id="fea7f-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="fea7f-189">組み込みのカメラを有効にするかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-189">Defines whether built-in cameras are enabled.</span></span> <span data-ttu-id="fea7f-190">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="fea7f-191">microphonesAndSpeakers</span><span class="sxs-lookup"><span data-stu-id="fea7f-191">microphonesAndSpeakers</span></span>|[<span data-ttu-id="fea7f-192">購入</span><span class="sxs-lookup"><span data-stu-id="fea7f-192">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="fea7f-193">組み込みマイクまたはスピーカーを有効にするかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-193">Defines whether built-in microphones or speakers are enabled.</span></span> <span data-ttu-id="fea7f-194">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="fea7f-195">機器</span><span class="sxs-lookup"><span data-stu-id="fea7f-195">radios</span></span>|[<span data-ttu-id="fea7f-196">購入</span><span class="sxs-lookup"><span data-stu-id="fea7f-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="fea7f-197">組み込みの無線機 (WI-FI、NFC、Bluetooth など) を有効にするかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-197">Defines whether built-in radios e.g. WIFI, NFC, Bluetooth, are enabled.</span></span> <span data-ttu-id="fea7f-198">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="fea7f-199">bootFromExternalMedia</span><span class="sxs-lookup"><span data-stu-id="fea7f-199">bootFromExternalMedia</span></span>|[<span data-ttu-id="fea7f-200">購入</span><span class="sxs-lookup"><span data-stu-id="fea7f-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="fea7f-201">ユーザーが外部メディアからの起動を許可されているかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-201">Defines whether a user is allowed to boot from external media.</span></span> <span data-ttu-id="fea7f-202">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="fea7f-203">bootFromBuiltInNetworkAdapters</span><span class="sxs-lookup"><span data-stu-id="fea7f-203">bootFromBuiltInNetworkAdapters</span></span>|[<span data-ttu-id="fea7f-204">購入</span><span class="sxs-lookup"><span data-stu-id="fea7f-204">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="fea7f-205">ユーザーが組み込みのネットワークアダプターからの起動を許可されているかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-205">Defines whether a user is allowed to boot from built-in network adapters.</span></span> <span data-ttu-id="fea7f-206">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="fea7f-207">応答</span><span class="sxs-lookup"><span data-stu-id="fea7f-207">Response</span></span>
<span data-ttu-id="fea7f-208">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fea7f-208">If successful, this method returns a `201 Created` response code and a [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fea7f-209">例</span><span class="sxs-lookup"><span data-stu-id="fea7f-209">Example</span></span>

### <a name="request"></a><span data-ttu-id="fea7f-210">要求</span><span class="sxs-lookup"><span data-stu-id="fea7f-210">Request</span></span>
<span data-ttu-id="fea7f-211">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fea7f-211">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1309

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
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
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="fea7f-212">応答</span><span class="sxs-lookup"><span data-stu-id="fea7f-212">Response</span></span>
<span data-ttu-id="fea7f-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fea7f-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1481

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "id": "96474363-4363-9647-6343-479663434796",
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
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled"
}
```






