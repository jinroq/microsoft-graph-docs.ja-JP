---
title: macOSDeviceFeaturesConfiguration の更新
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 780a99d3a298caee1e50d8b85699e9f6a4c2a9af
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34976807"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="79a39-103">macOSDeviceFeaturesConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="79a39-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="79a39-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79a39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79a39-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79a39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79a39-106">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="79a39-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79a39-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="79a39-107">Prerequisites</span></span>
<span data-ttu-id="79a39-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79a39-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79a39-110">Permission type</span></span>|<span data-ttu-id="79a39-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79a39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79a39-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79a39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="79a39-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79a39-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="79a39-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79a39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79a39-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79a39-115">Not supported.</span></span>|
|<span data-ttu-id="79a39-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79a39-116">Application</span></span>|<span data-ttu-id="79a39-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79a39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79a39-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79a39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="79a39-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79a39-119">Request headers</span></span>
|<span data-ttu-id="79a39-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79a39-120">Header</span></span>|<span data-ttu-id="79a39-121">値</span><span class="sxs-lookup"><span data-stu-id="79a39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79a39-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79a39-122">Authorization</span></span>|<span data-ttu-id="79a39-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="79a39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79a39-124">承諾</span><span class="sxs-lookup"><span data-stu-id="79a39-124">Accept</span></span>|<span data-ttu-id="79a39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="79a39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79a39-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="79a39-126">Request body</span></span>
<span data-ttu-id="79a39-127">要求本文で、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="79a39-128">次の表に、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="79a39-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="79a39-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79a39-129">Property</span></span>|<span data-ttu-id="79a39-130">型</span><span class="sxs-lookup"><span data-stu-id="79a39-130">Type</span></span>|<span data-ttu-id="79a39-131">説明</span><span class="sxs-lookup"><span data-stu-id="79a39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79a39-132">id</span><span class="sxs-lookup"><span data-stu-id="79a39-132">id</span></span>|<span data-ttu-id="79a39-133">文字列</span><span class="sxs-lookup"><span data-stu-id="79a39-133">String</span></span>|<span data-ttu-id="79a39-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="79a39-134">Key of the entity.</span></span> <span data-ttu-id="79a39-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79a39-136">lastModifiedDateTime</span></span>|<span data-ttu-id="79a39-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79a39-137">DateTimeOffset</span></span>|<span data-ttu-id="79a39-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="79a39-138">DateTime the object was last modified.</span></span> <span data-ttu-id="79a39-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="79a39-140">roleScopeTagIds</span></span>|<span data-ttu-id="79a39-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="79a39-141">String collection</span></span>|<span data-ttu-id="79a39-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="79a39-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="79a39-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="79a39-144">supportsScopeTags</span></span>|<span data-ttu-id="79a39-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-145">Boolean</span></span>|<span data-ttu-id="79a39-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="79a39-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="79a39-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="79a39-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="79a39-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="79a39-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="79a39-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="79a39-149">This property is read-only.</span></span> <span data-ttu-id="79a39-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="79a39-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="79a39-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="79a39-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="79a39-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="79a39-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="79a39-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="79a39-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="79a39-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="79a39-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="79a39-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="79a39-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="79a39-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="79a39-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="79a39-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="79a39-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="79a39-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="79a39-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="79a39-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="79a39-163">createdDateTime</span></span>|<span data-ttu-id="79a39-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79a39-164">DateTimeOffset</span></span>|<span data-ttu-id="79a39-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="79a39-165">DateTime the object was created.</span></span> <span data-ttu-id="79a39-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-167">description</span><span class="sxs-lookup"><span data-stu-id="79a39-167">description</span></span>|<span data-ttu-id="79a39-168">String</span><span class="sxs-lookup"><span data-stu-id="79a39-168">String</span></span>|<span data-ttu-id="79a39-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="79a39-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="79a39-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-171">displayName</span><span class="sxs-lookup"><span data-stu-id="79a39-171">displayName</span></span>|<span data-ttu-id="79a39-172">String</span><span class="sxs-lookup"><span data-stu-id="79a39-172">String</span></span>|<span data-ttu-id="79a39-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="79a39-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="79a39-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-175">version</span><span class="sxs-lookup"><span data-stu-id="79a39-175">version</span></span>|<span data-ttu-id="79a39-176">Int32</span><span class="sxs-lookup"><span data-stu-id="79a39-176">Int32</span></span>|<span data-ttu-id="79a39-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="79a39-177">Version of the device configuration.</span></span> <span data-ttu-id="79a39-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="79a39-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="79a39-179">放映した Print行先</span><span class="sxs-lookup"><span data-stu-id="79a39-179">airPrintDestinations</span></span>|<span data-ttu-id="79a39-180">[放映 Printdestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="79a39-180">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="79a39-181">常に表示される必要がある、放映中の印刷プリンターの配列です。</span><span class="sxs-lookup"><span data-stu-id="79a39-181">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="79a39-182">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="79a39-182">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="79a39-183">[AppleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="79a39-183">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="79a39-184">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="79a39-184">autoLaunchItems</span></span>|<span data-ttu-id="79a39-185">[Macoslaunchitem](../resources/intune-deviceconfig-macoslaunchitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="79a39-185">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="79a39-186">ユーザーがログインしたときに起動するアプリケーション、ファイル、フォルダー、およびその他のアイテムのリスト。</span><span class="sxs-lookup"><span data-stu-id="79a39-186">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="79a39-187">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="79a39-187">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="79a39-188">Adminshoの Stinfo</span><span class="sxs-lookup"><span data-stu-id="79a39-188">adminShowHostInfo</span></span>|<span data-ttu-id="79a39-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-189">Boolean</span></span>|<span data-ttu-id="79a39-190">ログインウィンドウに管理ホスト情報を表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-190">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="79a39-191">loginWindowText</span><span class="sxs-lookup"><span data-stu-id="79a39-191">loginWindowText</span></span>|<span data-ttu-id="79a39-192">String</span><span class="sxs-lookup"><span data-stu-id="79a39-192">String</span></span>|<span data-ttu-id="79a39-193">ログインウィンドウに表示されるカスタムテキスト。</span><span class="sxs-lookup"><span data-stu-id="79a39-193">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="79a39-194">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="79a39-194">authorizedUsersListHidden</span></span>|<span data-ttu-id="79a39-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-195">Boolean</span></span>|<span data-ttu-id="79a39-196">ログインウィンドウで [名前とパスワード] ダイアログを表示するか、ユーザーの一覧を表示するかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-196">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="79a39-197">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="79a39-197">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="79a39-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-198">Boolean</span></span>|<span data-ttu-id="79a39-199">ログインウィンドウの承認済みユーザーの一覧に、ネットワークユーザーとシステムユーザーのみを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-199">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="79a39-200">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="79a39-200">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="79a39-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-201">Boolean</span></span>|<span data-ttu-id="79a39-202">ログインウィンドウの承認されたユーザーの一覧でモバイルユーザーを非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-202">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="79a39-203">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="79a39-203">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="79a39-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-204">Boolean</span></span>|<span data-ttu-id="79a39-205">[ログイン] ウィンドウで、承認されたユーザーの一覧にネットワークユーザーを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-205">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="79a39-206">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="79a39-206">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="79a39-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-207">Boolean</span></span>|<span data-ttu-id="79a39-208">ログインウィンドウの承認されたユーザーの一覧で管理者ユーザーを非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-208">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="79a39-209">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="79a39-209">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="79a39-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-210">Boolean</span></span>|<span data-ttu-id="79a39-211">[ログイン] ウィンドウで、承認されたユーザーの一覧に他のユーザーを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-211">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="79a39-212">shutDownDisabled</span><span class="sxs-lookup"><span data-stu-id="79a39-212">shutDownDisabled</span></span>|<span data-ttu-id="79a39-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-213">Boolean</span></span>|<span data-ttu-id="79a39-214">ログインウィンドウで [シャットダウン] ボタンの項目を非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-214">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="79a39-215">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="79a39-215">restartDisabled</span></span>|<span data-ttu-id="79a39-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-216">Boolean</span></span>|<span data-ttu-id="79a39-217">ログインウィンドウで [再起動] ボタンの項目を非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-217">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="79a39-218">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="79a39-218">sleepDisabled</span></span>|<span data-ttu-id="79a39-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-219">Boolean</span></span>|<span data-ttu-id="79a39-220">ログインウィンドウで [スリープ] メニュー項目を非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-220">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="79a39-221">consoleAccessDisabled</span><span class="sxs-lookup"><span data-stu-id="79a39-221">consoleAccessDisabled</span></span>|<span data-ttu-id="79a39-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-222">Boolean</span></span>|<span data-ttu-id="79a39-223">他のユーザーが '>コンソール> 特別なユーザー名を使用しないかどうか。</span><span class="sxs-lookup"><span data-stu-id="79a39-223">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="79a39-224">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="79a39-224">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="79a39-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-225">Boolean</span></span>|<span data-ttu-id="79a39-226">ログインウィンドウの [シャットダウン] メニュー項目が、ユーザーのログイン中に無効になるかどうか。</span><span class="sxs-lookup"><span data-stu-id="79a39-226">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="79a39-227">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="79a39-227">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="79a39-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-228">Boolean</span></span>|<span data-ttu-id="79a39-229">ログインウィンドウの [再起動] メニュー項目が、ユーザーのログイン中に無効になるかどうか。</span><span class="sxs-lookup"><span data-stu-id="79a39-229">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="79a39-230">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="79a39-230">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="79a39-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-231">Boolean</span></span>|<span data-ttu-id="79a39-232">ログインウィンドウの [電源オフ] メニュー項目が、ユーザーのログイン中に無効になるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-232">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="79a39-233">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="79a39-233">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="79a39-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-234">Boolean</span></span>|<span data-ttu-id="79a39-235">ログインウィンドウの [Log Out] メニュー項目が、ユーザーのログイン中に無効になるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-235">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="79a39-236">screenLockDisableImmediate</span><span class="sxs-lookup"><span data-stu-id="79a39-236">screenLockDisableImmediate</span></span>|<span data-ttu-id="79a39-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="79a39-237">Boolean</span></span>|<span data-ttu-id="79a39-238">即時画面ロック機能を無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="79a39-238">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="79a39-239">応答</span><span class="sxs-lookup"><span data-stu-id="79a39-239">Response</span></span>
<span data-ttu-id="79a39-240">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="79a39-240">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79a39-241">例</span><span class="sxs-lookup"><span data-stu-id="79a39-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="79a39-242">要求</span><span class="sxs-lookup"><span data-stu-id="79a39-242">Request</span></span>
<span data-ttu-id="79a39-243">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79a39-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2107

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true
}
```

### <a name="response"></a><span data-ttu-id="79a39-244">応答</span><span class="sxs-lookup"><span data-stu-id="79a39-244">Response</span></span>
<span data-ttu-id="79a39-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79a39-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2279

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "Path value",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "Login Window Text value",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true
}
```





