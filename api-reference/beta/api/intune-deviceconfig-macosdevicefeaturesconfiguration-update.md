---
title: macOSDeviceFeaturesConfiguration の更新
description: macOSDeviceFeaturesConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d3d583d894a11edc6d95a95f2b1869b08467689
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518738"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="8becb-103">macOSDeviceFeaturesConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="8becb-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="8becb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8becb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8becb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8becb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8becb-106">[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8becb-106">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8becb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8becb-107">Prerequisites</span></span>
<span data-ttu-id="8becb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8becb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8becb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8becb-110">Permission type</span></span>|<span data-ttu-id="8becb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8becb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8becb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8becb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8becb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8becb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8becb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8becb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8becb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8becb-115">Not supported.</span></span>|
|<span data-ttu-id="8becb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8becb-116">Application</span></span>|<span data-ttu-id="8becb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8becb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8becb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8becb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8becb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8becb-119">Request headers</span></span>
|<span data-ttu-id="8becb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8becb-120">Header</span></span>|<span data-ttu-id="8becb-121">値</span><span class="sxs-lookup"><span data-stu-id="8becb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8becb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8becb-122">Authorization</span></span>|<span data-ttu-id="8becb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8becb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8becb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8becb-124">Accept</span></span>|<span data-ttu-id="8becb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8becb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8becb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8becb-126">Request body</span></span>
<span data-ttu-id="8becb-127">要求本文で、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-127">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="8becb-128">次の表に、[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8becb-128">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="8becb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8becb-129">Property</span></span>|<span data-ttu-id="8becb-130">型</span><span class="sxs-lookup"><span data-stu-id="8becb-130">Type</span></span>|<span data-ttu-id="8becb-131">説明</span><span class="sxs-lookup"><span data-stu-id="8becb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8becb-132">id</span><span class="sxs-lookup"><span data-stu-id="8becb-132">id</span></span>|<span data-ttu-id="8becb-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8becb-133">String</span></span>|<span data-ttu-id="8becb-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8becb-134">Key of the entity.</span></span> <span data-ttu-id="8becb-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8becb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8becb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8becb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8becb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8becb-137">DateTimeOffset</span></span>|<span data-ttu-id="8becb-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8becb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8becb-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8becb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8becb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8becb-140">roleScopeTagIds</span></span>|<span data-ttu-id="8becb-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8becb-141">String collection</span></span>|<span data-ttu-id="8becb-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="8becb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8becb-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8becb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8becb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8becb-144">supportsScopeTags</span></span>|<span data-ttu-id="8becb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-145">Boolean</span></span>|<span data-ttu-id="8becb-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8becb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8becb-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="8becb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8becb-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="8becb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8becb-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="8becb-149">This property is read-only.</span></span> <span data-ttu-id="8becb-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8becb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8becb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8becb-151">createdDateTime</span></span>|<span data-ttu-id="8becb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8becb-152">DateTimeOffset</span></span>|<span data-ttu-id="8becb-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8becb-153">DateTime the object was created.</span></span> <span data-ttu-id="8becb-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8becb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8becb-155">説明</span><span class="sxs-lookup"><span data-stu-id="8becb-155">description</span></span>|<span data-ttu-id="8becb-156">String</span><span class="sxs-lookup"><span data-stu-id="8becb-156">String</span></span>|<span data-ttu-id="8becb-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="8becb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8becb-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8becb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8becb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8becb-159">displayName</span></span>|<span data-ttu-id="8becb-160">String</span><span class="sxs-lookup"><span data-stu-id="8becb-160">String</span></span>|<span data-ttu-id="8becb-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="8becb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8becb-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8becb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8becb-163">version</span><span class="sxs-lookup"><span data-stu-id="8becb-163">version</span></span>|<span data-ttu-id="8becb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8becb-164">Int32</span></span>|<span data-ttu-id="8becb-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8becb-165">Version of the device configuration.</span></span> <span data-ttu-id="8becb-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8becb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8becb-167">放映した print行先</span><span class="sxs-lookup"><span data-stu-id="8becb-167">airPrintDestinations</span></span>|<span data-ttu-id="8becb-168">[放映 printdestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8becb-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="8becb-169">常に表示される必要がある、放映中の印刷プリンターの配列です。</span><span class="sxs-lookup"><span data-stu-id="8becb-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="8becb-170">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8becb-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8becb-171">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="8becb-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="8becb-172">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="8becb-172">autoLaunchItems</span></span>|<span data-ttu-id="8becb-173">[macoslaunchitem](../resources/intune-deviceconfig-macoslaunchitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8becb-173">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="8becb-174">ユーザーがログインしたときに起動するアプリケーション、ファイル、フォルダー、およびその他のアイテムのリスト。</span><span class="sxs-lookup"><span data-stu-id="8becb-174">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="8becb-175">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8becb-175">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8becb-176">adminshoの stinfo</span><span class="sxs-lookup"><span data-stu-id="8becb-176">adminShowHostInfo</span></span>|<span data-ttu-id="8becb-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-177">Boolean</span></span>|<span data-ttu-id="8becb-178">ログインウィンドウに管理ホスト情報を表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-178">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="8becb-179">loginwindowtext</span><span class="sxs-lookup"><span data-stu-id="8becb-179">loginWindowText</span></span>|<span data-ttu-id="8becb-180">String</span><span class="sxs-lookup"><span data-stu-id="8becb-180">String</span></span>|<span data-ttu-id="8becb-181">ログインウィンドウに表示されるカスタムテキスト。</span><span class="sxs-lookup"><span data-stu-id="8becb-181">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="8becb-182">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="8becb-182">authorizedUsersListHidden</span></span>|<span data-ttu-id="8becb-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-183">Boolean</span></span>|<span data-ttu-id="8becb-184">ログインウィンドウで [名前とパスワード] ダイアログを表示するか、ユーザーの一覧を表示するかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-184">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="8becb-185">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="8becb-185">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="8becb-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-186">Boolean</span></span>|<span data-ttu-id="8becb-187">ログインウィンドウの承認済みユーザーの一覧に、ネットワークユーザーとシステムユーザーのみを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-187">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8becb-188">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="8becb-188">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="8becb-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-189">Boolean</span></span>|<span data-ttu-id="8becb-190">ログインウィンドウの承認されたユーザーの一覧でモバイルユーザーを非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-190">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8becb-191">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="8becb-191">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="8becb-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-192">Boolean</span></span>|<span data-ttu-id="8becb-193">[ログイン] ウィンドウで、承認されたユーザーの一覧にネットワークユーザーを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-193">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8becb-194">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="8becb-194">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="8becb-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-195">Boolean</span></span>|<span data-ttu-id="8becb-196">ログインウィンドウの承認されたユーザーの一覧で管理者ユーザーを非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-196">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8becb-197">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="8becb-197">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="8becb-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-198">Boolean</span></span>|<span data-ttu-id="8becb-199">[ログイン] ウィンドウで、承認されたユーザーの一覧に他のユーザーを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-199">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="8becb-200">shutdowndisabled</span><span class="sxs-lookup"><span data-stu-id="8becb-200">shutDownDisabled</span></span>|<span data-ttu-id="8becb-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-201">Boolean</span></span>|<span data-ttu-id="8becb-202">ログインウィンドウで [シャットダウン] ボタンの項目を非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-202">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="8becb-203">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="8becb-203">restartDisabled</span></span>|<span data-ttu-id="8becb-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-204">Boolean</span></span>|<span data-ttu-id="8becb-205">ログインウィンドウで [再起動] ボタンの項目を非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-205">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="8becb-206">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="8becb-206">sleepDisabled</span></span>|<span data-ttu-id="8becb-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-207">Boolean</span></span>|<span data-ttu-id="8becb-208">ログインウィンドウで [スリープ] メニュー項目を非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-208">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="8becb-209">consoleaccessdisabled</span><span class="sxs-lookup"><span data-stu-id="8becb-209">consoleAccessDisabled</span></span>|<span data-ttu-id="8becb-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-210">Boolean</span></span>|<span data-ttu-id="8becb-211">他のユーザーが ' >console> 特殊ユーザー名の使用を無視するかどうか。</span><span class="sxs-lookup"><span data-stu-id="8becb-211">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="8becb-212">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="8becb-212">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="8becb-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-213">Boolean</span></span>|<span data-ttu-id="8becb-214">ログインウィンドウの [シャットダウン] メニュー項目が、ユーザーのログイン中に無効になるかどうか。</span><span class="sxs-lookup"><span data-stu-id="8becb-214">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="8becb-215">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="8becb-215">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="8becb-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-216">Boolean</span></span>|<span data-ttu-id="8becb-217">ログインウィンドウの [再起動] メニュー項目が、ユーザーのログイン中に無効になるかどうか。</span><span class="sxs-lookup"><span data-stu-id="8becb-217">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="8becb-218">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="8becb-218">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="8becb-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-219">Boolean</span></span>|<span data-ttu-id="8becb-220">ログインウィンドウの [電源オフ] メニュー項目が、ユーザーのログイン中に無効になるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-220">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="8becb-221">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="8becb-221">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="8becb-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-222">Boolean</span></span>|<span data-ttu-id="8becb-223">ログインウィンドウの [Log Out] メニュー項目が、ユーザーのログイン中に無効になるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-223">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="8becb-224">screenlockdisableimmediate</span><span class="sxs-lookup"><span data-stu-id="8becb-224">screenLockDisableImmediate</span></span>|<span data-ttu-id="8becb-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="8becb-225">Boolean</span></span>|<span data-ttu-id="8becb-226">即時画面ロック機能を無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8becb-226">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="8becb-227">応答</span><span class="sxs-lookup"><span data-stu-id="8becb-227">Response</span></span>
<span data-ttu-id="8becb-228">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8becb-228">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8becb-229">例</span><span class="sxs-lookup"><span data-stu-id="8becb-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="8becb-230">要求</span><span class="sxs-lookup"><span data-stu-id="8becb-230">Request</span></span>
<span data-ttu-id="8becb-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8becb-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1334

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

### <a name="response"></a><span data-ttu-id="8becb-232">応答</span><span class="sxs-lookup"><span data-stu-id="8becb-232">Response</span></span>
<span data-ttu-id="8becb-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8becb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1506

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





