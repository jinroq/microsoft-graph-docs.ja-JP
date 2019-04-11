---
title: macOSDeviceFeaturesConfiguration の作成
description: 新しい macOSDeviceFeaturesConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: df5edc6fc28b4e4f9e242bd30cff38458e5edd42
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771419"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="64189-103">macOSDeviceFeaturesConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="64189-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="64189-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64189-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64189-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="64189-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64189-106">新しい [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="64189-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64189-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="64189-107">Prerequisites</span></span>
<span data-ttu-id="64189-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64189-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64189-110">Permission type</span></span>|<span data-ttu-id="64189-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="64189-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64189-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64189-112">Delegated (work or school account)</span></span>|<span data-ttu-id="64189-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64189-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="64189-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64189-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64189-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64189-115">Not supported.</span></span>|
|<span data-ttu-id="64189-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64189-116">Application</span></span>|<span data-ttu-id="64189-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64189-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64189-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64189-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="64189-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64189-119">Request headers</span></span>
|<span data-ttu-id="64189-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64189-120">Header</span></span>|<span data-ttu-id="64189-121">値</span><span class="sxs-lookup"><span data-stu-id="64189-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64189-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="64189-122">Authorization</span></span>|<span data-ttu-id="64189-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="64189-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64189-124">承諾</span><span class="sxs-lookup"><span data-stu-id="64189-124">Accept</span></span>|<span data-ttu-id="64189-125">application/json</span><span class="sxs-lookup"><span data-stu-id="64189-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64189-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="64189-126">Request body</span></span>
<span data-ttu-id="64189-127">要求本文で、macOSDeviceFeaturesConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="64189-128">次の表に、macOSDeviceFeaturesConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="64189-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="64189-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64189-129">Property</span></span>|<span data-ttu-id="64189-130">型</span><span class="sxs-lookup"><span data-stu-id="64189-130">Type</span></span>|<span data-ttu-id="64189-131">説明</span><span class="sxs-lookup"><span data-stu-id="64189-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64189-132">id</span><span class="sxs-lookup"><span data-stu-id="64189-132">id</span></span>|<span data-ttu-id="64189-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="64189-133">String</span></span>|<span data-ttu-id="64189-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="64189-134">Key of the entity.</span></span> <span data-ttu-id="64189-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64189-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64189-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="64189-136">lastModifiedDateTime</span></span>|<span data-ttu-id="64189-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64189-137">DateTimeOffset</span></span>|<span data-ttu-id="64189-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="64189-138">DateTime the object was last modified.</span></span> <span data-ttu-id="64189-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64189-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64189-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="64189-140">roleScopeTagIds</span></span>|<span data-ttu-id="64189-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="64189-141">String collection</span></span>|<span data-ttu-id="64189-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="64189-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="64189-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64189-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64189-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="64189-144">supportsScopeTags</span></span>|<span data-ttu-id="64189-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-145">Boolean</span></span>|<span data-ttu-id="64189-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="64189-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="64189-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="64189-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="64189-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="64189-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="64189-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="64189-149">This property is read-only.</span></span> <span data-ttu-id="64189-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64189-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64189-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="64189-151">createdDateTime</span></span>|<span data-ttu-id="64189-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64189-152">DateTimeOffset</span></span>|<span data-ttu-id="64189-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="64189-153">DateTime the object was created.</span></span> <span data-ttu-id="64189-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64189-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64189-155">説明</span><span class="sxs-lookup"><span data-stu-id="64189-155">description</span></span>|<span data-ttu-id="64189-156">String</span><span class="sxs-lookup"><span data-stu-id="64189-156">String</span></span>|<span data-ttu-id="64189-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="64189-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="64189-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64189-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64189-159">displayName</span><span class="sxs-lookup"><span data-stu-id="64189-159">displayName</span></span>|<span data-ttu-id="64189-160">String</span><span class="sxs-lookup"><span data-stu-id="64189-160">String</span></span>|<span data-ttu-id="64189-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="64189-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="64189-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64189-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64189-163">version</span><span class="sxs-lookup"><span data-stu-id="64189-163">version</span></span>|<span data-ttu-id="64189-164">Int32</span><span class="sxs-lookup"><span data-stu-id="64189-164">Int32</span></span>|<span data-ttu-id="64189-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="64189-165">Version of the device configuration.</span></span> <span data-ttu-id="64189-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64189-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="64189-167">放映した print行先</span><span class="sxs-lookup"><span data-stu-id="64189-167">airPrintDestinations</span></span>|<span data-ttu-id="64189-168">[放映 printdestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="64189-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="64189-169">常に表示される必要がある、放映中の印刷プリンターの配列です。</span><span class="sxs-lookup"><span data-stu-id="64189-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="64189-170">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="64189-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="64189-171">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="64189-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="64189-172">autoLaunchItems</span><span class="sxs-lookup"><span data-stu-id="64189-172">autoLaunchItems</span></span>|<span data-ttu-id="64189-173">[macoslaunchitem](../resources/intune-deviceconfig-macoslaunchitem.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="64189-173">[macOSLaunchItem](../resources/intune-deviceconfig-macoslaunchitem.md) collection</span></span>|<span data-ttu-id="64189-174">ユーザーがログインしたときに起動するアプリケーション、ファイル、フォルダー、およびその他のアイテムのリスト。</span><span class="sxs-lookup"><span data-stu-id="64189-174">List of applications, files, folders, and other items to launch when the user logs in.</span></span> <span data-ttu-id="64189-175">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="64189-175">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="64189-176">adminshoの stinfo</span><span class="sxs-lookup"><span data-stu-id="64189-176">adminShowHostInfo</span></span>|<span data-ttu-id="64189-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-177">Boolean</span></span>|<span data-ttu-id="64189-178">ログインウィンドウに管理ホスト情報を表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-178">Whether to show admin host information on the login window.</span></span>|
|<span data-ttu-id="64189-179">loginwindowtext</span><span class="sxs-lookup"><span data-stu-id="64189-179">loginWindowText</span></span>|<span data-ttu-id="64189-180">文字列</span><span class="sxs-lookup"><span data-stu-id="64189-180">String</span></span>|<span data-ttu-id="64189-181">ログインウィンドウに表示されるカスタムテキスト。</span><span class="sxs-lookup"><span data-stu-id="64189-181">Custom text to be displayed on the login window.</span></span>|
|<span data-ttu-id="64189-182">authorizedUsersListHidden</span><span class="sxs-lookup"><span data-stu-id="64189-182">authorizedUsersListHidden</span></span>|<span data-ttu-id="64189-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-183">Boolean</span></span>|<span data-ttu-id="64189-184">ログインウィンドウで [名前とパスワード] ダイアログを表示するか、ユーザーの一覧を表示するかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-184">Whether to show the name and password dialog or a list of users on the login window.</span></span>|
|<span data-ttu-id="64189-185">authorizedUsersListHideLocalUsers</span><span class="sxs-lookup"><span data-stu-id="64189-185">authorizedUsersListHideLocalUsers</span></span>|<span data-ttu-id="64189-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-186">Boolean</span></span>|<span data-ttu-id="64189-187">ログインウィンドウの承認済みユーザーの一覧に、ネットワークユーザーとシステムユーザーのみを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-187">Whether to show only network and system users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="64189-188">authorizedUsersListHideMobileAccounts</span><span class="sxs-lookup"><span data-stu-id="64189-188">authorizedUsersListHideMobileAccounts</span></span>|<span data-ttu-id="64189-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-189">Boolean</span></span>|<span data-ttu-id="64189-190">ログインウィンドウの承認されたユーザーの一覧でモバイルユーザーを非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-190">Whether to hide mobile users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="64189-191">authorizedUsersListIncludeNetworkUsers</span><span class="sxs-lookup"><span data-stu-id="64189-191">authorizedUsersListIncludeNetworkUsers</span></span>|<span data-ttu-id="64189-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-192">Boolean</span></span>|<span data-ttu-id="64189-193">[ログイン] ウィンドウで、承認されたユーザーの一覧にネットワークユーザーを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-193">Whether to show network users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="64189-194">authorizedUsersListHideAdminUsers</span><span class="sxs-lookup"><span data-stu-id="64189-194">authorizedUsersListHideAdminUsers</span></span>|<span data-ttu-id="64189-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-195">Boolean</span></span>|<span data-ttu-id="64189-196">ログインウィンドウの承認されたユーザーの一覧で管理者ユーザーを非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-196">Whether to hide admin users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="64189-197">authorizedUsersListShowOtherManagedUsers</span><span class="sxs-lookup"><span data-stu-id="64189-197">authorizedUsersListShowOtherManagedUsers</span></span>|<span data-ttu-id="64189-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-198">Boolean</span></span>|<span data-ttu-id="64189-199">[ログイン] ウィンドウで、承認されたユーザーの一覧に他のユーザーを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-199">Whether to show other users in the authorized users list on the login window.</span></span>|
|<span data-ttu-id="64189-200">shutdowndisabled</span><span class="sxs-lookup"><span data-stu-id="64189-200">shutDownDisabled</span></span>|<span data-ttu-id="64189-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-201">Boolean</span></span>|<span data-ttu-id="64189-202">ログインウィンドウで [シャットダウン] ボタンの項目を非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-202">Whether to hide the Shut Down button item on the login window.</span></span>|
|<span data-ttu-id="64189-203">restartDisabled</span><span class="sxs-lookup"><span data-stu-id="64189-203">restartDisabled</span></span>|<span data-ttu-id="64189-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-204">Boolean</span></span>|<span data-ttu-id="64189-205">ログインウィンドウで [再起動] ボタンの項目を非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-205">Whether to hide the Restart button item on the login window.</span></span>|
|<span data-ttu-id="64189-206">sleepDisabled</span><span class="sxs-lookup"><span data-stu-id="64189-206">sleepDisabled</span></span>|<span data-ttu-id="64189-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-207">Boolean</span></span>|<span data-ttu-id="64189-208">ログインウィンドウで [スリープ] メニュー項目を非表示にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-208">Whether to hide the Sleep menu item on the login window.</span></span>|
|<span data-ttu-id="64189-209">consoleaccessdisabled</span><span class="sxs-lookup"><span data-stu-id="64189-209">consoleAccessDisabled</span></span>|<span data-ttu-id="64189-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-210">Boolean</span></span>|<span data-ttu-id="64189-211">他のユーザーが ' >console> 特殊ユーザー名の使用を無視するかどうか。</span><span class="sxs-lookup"><span data-stu-id="64189-211">Whether the Other user will disregard use of the \`>console> special user name.</span></span>|
|<span data-ttu-id="64189-212">shutDownDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="64189-212">shutDownDisabledWhileLoggedIn</span></span>|<span data-ttu-id="64189-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-213">Boolean</span></span>|<span data-ttu-id="64189-214">ログインウィンドウの [シャットダウン] メニュー項目が、ユーザーのログイン中に無効になるかどうか。</span><span class="sxs-lookup"><span data-stu-id="64189-214">Whether the Shut Down menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="64189-215">restartDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="64189-215">restartDisabledWhileLoggedIn</span></span>|<span data-ttu-id="64189-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-216">Boolean</span></span>|<span data-ttu-id="64189-217">ログインウィンドウの [再起動] メニュー項目が、ユーザーのログイン中に無効になるかどうか。</span><span class="sxs-lookup"><span data-stu-id="64189-217">Whether the Restart menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="64189-218">powerOffDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="64189-218">powerOffDisabledWhileLoggedIn</span></span>|<span data-ttu-id="64189-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-219">Boolean</span></span>|<span data-ttu-id="64189-220">ログインウィンドウの [電源オフ] メニュー項目が、ユーザーのログイン中に無効になるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-220">Whether the Power Off menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="64189-221">logOutDisabledWhileLoggedIn</span><span class="sxs-lookup"><span data-stu-id="64189-221">logOutDisabledWhileLoggedIn</span></span>|<span data-ttu-id="64189-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-222">Boolean</span></span>|<span data-ttu-id="64189-223">ログインウィンドウの [Log Out] メニュー項目が、ユーザーのログイン中に無効になるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-223">Whether the Log Out menu item on the login window will be disabled while the user is logged in.</span></span>|
|<span data-ttu-id="64189-224">screenlockdisableimmediate</span><span class="sxs-lookup"><span data-stu-id="64189-224">screenLockDisableImmediate</span></span>|<span data-ttu-id="64189-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="64189-225">Boolean</span></span>|<span data-ttu-id="64189-226">即時画面ロック機能を無効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="64189-226">Whether to disable the immediate screen lock functions.</span></span>|



## <a name="response"></a><span data-ttu-id="64189-227">応答</span><span class="sxs-lookup"><span data-stu-id="64189-227">Response</span></span>
<span data-ttu-id="64189-228">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="64189-228">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64189-229">例</span><span class="sxs-lookup"><span data-stu-id="64189-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="64189-230">要求</span><span class="sxs-lookup"><span data-stu-id="64189-230">Request</span></span>
<span data-ttu-id="64189-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64189-231">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="64189-232">応答</span><span class="sxs-lookup"><span data-stu-id="64189-232">Response</span></span>
<span data-ttu-id="64189-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="64189-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





