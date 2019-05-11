---
title: WindowsKioskConfiguration の作成
description: 新しい windowsKioskConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f7549fbbb9859c58f1acd56618130744107141ab
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917892"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="2dea1-103">WindowsKioskConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="2dea1-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="2dea1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dea1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2dea1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2dea1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2dea1-106">新しい[Windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2dea1-106">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2dea1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2dea1-107">Prerequisites</span></span>
<span data-ttu-id="2dea1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2dea1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dea1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2dea1-110">Permission type</span></span>|<span data-ttu-id="2dea1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2dea1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dea1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2dea1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2dea1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dea1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2dea1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2dea1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dea1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dea1-115">Not supported.</span></span>|
|<span data-ttu-id="2dea1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2dea1-116">Application</span></span>|<span data-ttu-id="2dea1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2dea1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dea1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2dea1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2dea1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2dea1-119">Request headers</span></span>
|<span data-ttu-id="2dea1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2dea1-120">Header</span></span>|<span data-ttu-id="2dea1-121">値</span><span class="sxs-lookup"><span data-stu-id="2dea1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2dea1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dea1-122">Authorization</span></span>|<span data-ttu-id="2dea1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2dea1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2dea1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2dea1-124">Accept</span></span>|<span data-ttu-id="2dea1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2dea1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dea1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2dea1-126">Request body</span></span>
<span data-ttu-id="2dea1-127">要求本文で、windowsKioskConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2dea1-127">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="2dea1-128">次の表に、windowsKioskConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2dea1-128">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="2dea1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2dea1-129">Property</span></span>|<span data-ttu-id="2dea1-130">型</span><span class="sxs-lookup"><span data-stu-id="2dea1-130">Type</span></span>|<span data-ttu-id="2dea1-131">説明</span><span class="sxs-lookup"><span data-stu-id="2dea1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dea1-132">id</span><span class="sxs-lookup"><span data-stu-id="2dea1-132">id</span></span>|<span data-ttu-id="2dea1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="2dea1-133">String</span></span>|<span data-ttu-id="2dea1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2dea1-134">Key of the entity.</span></span> <span data-ttu-id="2dea1-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2dea1-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dea1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2dea1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2dea1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dea1-137">DateTimeOffset</span></span>|<span data-ttu-id="2dea1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="2dea1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2dea1-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2dea1-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dea1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2dea1-140">roleScopeTagIds</span></span>|<span data-ttu-id="2dea1-141">String collection</span><span class="sxs-lookup"><span data-stu-id="2dea1-141">String collection</span></span>|<span data-ttu-id="2dea1-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="2dea1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2dea1-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2dea1-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dea1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2dea1-144">supportsScopeTags</span></span>|<span data-ttu-id="2dea1-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dea1-145">Boolean</span></span>|<span data-ttu-id="2dea1-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2dea1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2dea1-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="2dea1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2dea1-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="2dea1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2dea1-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="2dea1-149">This property is read-only.</span></span> <span data-ttu-id="2dea1-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2dea1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dea1-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2dea1-151">createdDateTime</span></span>|<span data-ttu-id="2dea1-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2dea1-152">DateTimeOffset</span></span>|<span data-ttu-id="2dea1-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2dea1-153">DateTime the object was created.</span></span> <span data-ttu-id="2dea1-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2dea1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dea1-155">description</span><span class="sxs-lookup"><span data-stu-id="2dea1-155">description</span></span>|<span data-ttu-id="2dea1-156">String</span><span class="sxs-lookup"><span data-stu-id="2dea1-156">String</span></span>|<span data-ttu-id="2dea1-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="2dea1-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2dea1-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2dea1-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dea1-159">displayName</span><span class="sxs-lookup"><span data-stu-id="2dea1-159">displayName</span></span>|<span data-ttu-id="2dea1-160">String</span><span class="sxs-lookup"><span data-stu-id="2dea1-160">String</span></span>|<span data-ttu-id="2dea1-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="2dea1-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2dea1-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2dea1-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dea1-163">version</span><span class="sxs-lookup"><span data-stu-id="2dea1-163">version</span></span>|<span data-ttu-id="2dea1-164">Int32</span><span class="sxs-lookup"><span data-stu-id="2dea1-164">Int32</span></span>|<span data-ttu-id="2dea1-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2dea1-165">Version of the device configuration.</span></span> <span data-ttu-id="2dea1-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2dea1-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2dea1-167">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="2dea1-167">kioskProfiles</span></span>|<span data-ttu-id="2dea1-168">[Windowskioskprofile](../resources/intune-deviceconfig-windowskioskprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2dea1-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="2dea1-169">このポリシー設定を使用すると、キオスクの構成のキオスクプロファイルの一覧を定義できます。</span><span class="sxs-lookup"><span data-stu-id="2dea1-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="2dea1-170">このコレクションには、最大3つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2dea1-170">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="2dea1-171">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="2dea1-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="2dea1-172">String</span><span class="sxs-lookup"><span data-stu-id="2dea1-172">String</span></span>|<span data-ttu-id="2dea1-173">ブラウザーが起動時に移動する既定の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="2dea1-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="2dea1-174">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="2dea1-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="2dea1-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dea1-175">Boolean</span></span>|<span data-ttu-id="2dea1-176">キオスクブラウザーの [ホーム] ボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="2dea1-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="2dea1-177">既定では、[ホーム] ボタンは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="2dea1-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="2dea1-178">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="2dea1-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="2dea1-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dea1-179">Boolean</span></span>|<span data-ttu-id="2dea1-180">キオスクブラウザーのナビゲーションボタン (前方/後方) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2dea1-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="2dea1-181">既定では、ナビゲーションボタンは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="2dea1-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="2dea1-182">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="2dea1-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="2dea1-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dea1-183">Boolean</span></span>|<span data-ttu-id="2dea1-184">キオスクブラウザーの [セッションの終了] ボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="2dea1-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="2dea1-185">既定では、[セッションの終了] ボタンは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="2dea1-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="2dea1-186">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="2dea1-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="2dea1-187">Int32</span><span class="sxs-lookup"><span data-stu-id="2dea1-187">Int32</span></span>|<span data-ttu-id="2dea1-188">キオスクブラウザーが新しい状態で再起動するまで、セッションがアイドル状態になっている時間 (分) を指定します。</span><span class="sxs-lookup"><span data-stu-id="2dea1-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="2dea1-189">有効な値は1-1440 です。</span><span class="sxs-lookup"><span data-stu-id="2dea1-189">Valid values are 1-1440.</span></span> <span data-ttu-id="2dea1-190">有効な値は 1 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="2dea1-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="2dea1-191">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="2dea1-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="2dea1-192">String collection</span><span class="sxs-lookup"><span data-stu-id="2dea1-192">String collection</span></span>|<span data-ttu-id="2dea1-193">キオスクブラウザーが移動しない Url を指定する</span><span class="sxs-lookup"><span data-stu-id="2dea1-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="2dea1-194">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="2dea1-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="2dea1-195">String collection</span><span class="sxs-lookup"><span data-stu-id="2dea1-195">String collection</span></span>|<span data-ttu-id="2dea1-196">キオスクブラウザーでの移動が許可されている Url を指定する</span><span class="sxs-lookup"><span data-stu-id="2dea1-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="2dea1-197">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="2dea1-197">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="2dea1-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="2dea1-198">Boolean</span></span>|<span data-ttu-id="2dea1-199">Microsoft Edge ブラウザーのパブリックブラウズキオスクモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="2dea1-199">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="2dea1-200">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="2dea1-200">The Default is false.</span></span>|



## <a name="response"></a><span data-ttu-id="2dea1-201">応答</span><span class="sxs-lookup"><span data-stu-id="2dea1-201">Response</span></span>
<span data-ttu-id="2dea1-202">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2dea1-202">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dea1-203">例</span><span class="sxs-lookup"><span data-stu-id="2dea1-203">Example</span></span>

### <a name="request"></a><span data-ttu-id="2dea1-204">要求</span><span class="sxs-lookup"><span data-stu-id="2dea1-204">Request</span></span>
<span data-ttu-id="2dea1-205">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2dea1-205">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1753

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "autoLaunch": true,
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true
}
```

### <a name="response"></a><span data-ttu-id="2dea1-206">応答</span><span class="sxs-lookup"><span data-stu-id="2dea1-206">Response</span></span>
<span data-ttu-id="2dea1-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2dea1-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1925

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "146a990b-990b-146a-0b99-6a140b996a14",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "Profile Id value",
      "profileName": "Profile Name value",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "small",
            "name": "Name value",
            "appType": "store",
            "autoLaunch": true,
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 6,
  "kioskBrowserBlockedURLs": [
    "Kiosk Browser Blocked URLs value"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "Kiosk Browser Blocked Url Exceptions value"
  ],
  "edgeKioskEnablePublicBrowsing": true
}
```




