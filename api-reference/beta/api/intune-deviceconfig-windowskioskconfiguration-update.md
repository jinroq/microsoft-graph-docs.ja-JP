---
title: WindowsKioskConfiguration を更新します。
description: WindowsKioskConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: e399daa1f57ac7ddcbbd1add9e414392bb8e3789
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360054"
---
# <a name="update-windowskioskconfiguration"></a><span data-ttu-id="1de8f-103">WindowsKioskConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-103">Update windowsKioskConfiguration</span></span>

> <span data-ttu-id="1de8f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1de8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1de8f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1de8f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1de8f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1de8f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1de8f-107">[WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-107">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1de8f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1de8f-108">Prerequisites</span></span>
<span data-ttu-id="1de8f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1de8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1de8f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1de8f-111">Permission type</span></span>|<span data-ttu-id="1de8f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1de8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1de8f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1de8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1de8f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1de8f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1de8f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1de8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1de8f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1de8f-116">Not supported.</span></span>|
|<span data-ttu-id="1de8f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1de8f-117">Application</span></span>|<span data-ttu-id="1de8f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1de8f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1de8f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1de8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="1de8f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1de8f-120">Request headers</span></span>
|<span data-ttu-id="1de8f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1de8f-121">Header</span></span>|<span data-ttu-id="1de8f-122">値</span><span class="sxs-lookup"><span data-stu-id="1de8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1de8f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1de8f-123">Authorization</span></span>|<span data-ttu-id="1de8f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1de8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1de8f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1de8f-125">Accept</span></span>|<span data-ttu-id="1de8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1de8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1de8f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1de8f-127">Request body</span></span>
<span data-ttu-id="1de8f-128">要求の本文に[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-128">In the request body, supply a JSON representation for the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

<span data-ttu-id="1de8f-129">[WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-129">The following table shows the properties that are required when you create the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>

|<span data-ttu-id="1de8f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1de8f-130">Property</span></span>|<span data-ttu-id="1de8f-131">種類</span><span class="sxs-lookup"><span data-stu-id="1de8f-131">Type</span></span>|<span data-ttu-id="1de8f-132">説明</span><span class="sxs-lookup"><span data-stu-id="1de8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1de8f-133">ID</span><span class="sxs-lookup"><span data-stu-id="1de8f-133">id</span></span>|<span data-ttu-id="1de8f-134">String</span><span class="sxs-lookup"><span data-stu-id="1de8f-134">String</span></span>|<span data-ttu-id="1de8f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1de8f-135">Key of the entity.</span></span> <span data-ttu-id="1de8f-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1de8f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de8f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1de8f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1de8f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1de8f-138">DateTimeOffset</span></span>|<span data-ttu-id="1de8f-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1de8f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1de8f-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1de8f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de8f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1de8f-141">roleScopeTagIds</span></span>|<span data-ttu-id="1de8f-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1de8f-142">String collection</span></span>|<span data-ttu-id="1de8f-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="1de8f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1de8f-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1de8f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de8f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1de8f-145">supportsScopeTags</span></span>|<span data-ttu-id="1de8f-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="1de8f-146">Boolean</span></span>|<span data-ttu-id="1de8f-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1de8f-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="1de8f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1de8f-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="1de8f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1de8f-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1de8f-150">This property is read-only.</span></span> <span data-ttu-id="1de8f-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1de8f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de8f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1de8f-152">createdDateTime</span></span>|<span data-ttu-id="1de8f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1de8f-153">DateTimeOffset</span></span>|<span data-ttu-id="1de8f-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1de8f-154">DateTime the object was created.</span></span> <span data-ttu-id="1de8f-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1de8f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de8f-156">説明</span><span class="sxs-lookup"><span data-stu-id="1de8f-156">description</span></span>|<span data-ttu-id="1de8f-157">String</span><span class="sxs-lookup"><span data-stu-id="1de8f-157">String</span></span>|<span data-ttu-id="1de8f-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1de8f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1de8f-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1de8f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de8f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="1de8f-160">displayName</span></span>|<span data-ttu-id="1de8f-161">String</span><span class="sxs-lookup"><span data-stu-id="1de8f-161">String</span></span>|<span data-ttu-id="1de8f-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1de8f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1de8f-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1de8f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de8f-164">version</span><span class="sxs-lookup"><span data-stu-id="1de8f-164">version</span></span>|<span data-ttu-id="1de8f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="1de8f-165">Int32</span></span>|<span data-ttu-id="1de8f-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1de8f-166">Version of the device configuration.</span></span> <span data-ttu-id="1de8f-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1de8f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1de8f-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="1de8f-168">kioskProfiles</span></span>|<span data-ttu-id="1de8f-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1de8f-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="1de8f-170">このポリシー設定は、構成のキオスクのキオスクのプロファイルの一覧を定義します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="1de8f-171">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1de8f-171">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="1de8f-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="1de8f-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="1de8f-173">String</span><span class="sxs-lookup"><span data-stu-id="1de8f-173">String</span></span>|<span data-ttu-id="1de8f-174">起動時にブラウザーが移動する必要があります既定の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="1de8f-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="1de8f-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="1de8f-176">ブール型</span><span class="sxs-lookup"><span data-stu-id="1de8f-176">Boolean</span></span>|<span data-ttu-id="1de8f-177">キオスク ブラウザーの [ホーム] ボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="1de8f-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="1de8f-178">既定では、[ホーム] ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="1de8f-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="1de8f-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="1de8f-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="1de8f-180">ブール型</span><span class="sxs-lookup"><span data-stu-id="1de8f-180">Boolean</span></span>|<span data-ttu-id="1de8f-181">キオスク ブラウザーのナビゲーションの buttons(forward/back) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="1de8f-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="1de8f-182">既定では、ナビゲーション ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="1de8f-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="1de8f-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="1de8f-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="1de8f-184">ブール型</span><span class="sxs-lookup"><span data-stu-id="1de8f-184">Boolean</span></span>|<span data-ttu-id="1de8f-185">キオスク ブラウザーの最後のセッションのボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="1de8f-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="1de8f-186">既定では、セッションの終了] ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="1de8f-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="1de8f-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="1de8f-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="1de8f-188">Int32</span><span class="sxs-lookup"><span data-stu-id="1de8f-188">Int32</span></span>|<span data-ttu-id="1de8f-189">キオスク ブラウザーを最新の状態で再起動するまで、セッションがアイドル状態の分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="1de8f-190">有効な値は、1 ~ 1440 です。</span><span class="sxs-lookup"><span data-stu-id="1de8f-190">Valid values are 1-1440.</span></span> <span data-ttu-id="1de8f-191">1 から 1440 の有効な値</span><span class="sxs-lookup"><span data-stu-id="1de8f-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="1de8f-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="1de8f-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="1de8f-193">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1de8f-193">String collection</span></span>|<span data-ttu-id="1de8f-194">キオスクのブラウザーの移動先のない Url を指定します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="1de8f-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="1de8f-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="1de8f-196">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1de8f-196">String collection</span></span>|<span data-ttu-id="1de8f-197">キオスクのブラウザーに移動するのには許可されている Url を指定します。</span><span class="sxs-lookup"><span data-stu-id="1de8f-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|



## <a name="response"></a><span data-ttu-id="1de8f-198">応答</span><span class="sxs-lookup"><span data-stu-id="1de8f-198">Response</span></span>
<span data-ttu-id="1de8f-199">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1de8f-199">If successful, this method returns a `200 OK` response code and an updated [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1de8f-200">例</span><span class="sxs-lookup"><span data-stu-id="1de8f-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="1de8f-201">要求</span><span class="sxs-lookup"><span data-stu-id="1de8f-201">Request</span></span>
<span data-ttu-id="1de8f-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1de8f-202">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1598

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
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
  ]
}
```

### <a name="response"></a><span data-ttu-id="1de8f-203">応答</span><span class="sxs-lookup"><span data-stu-id="1de8f-203">Response</span></span>
<span data-ttu-id="1de8f-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1de8f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1770

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
            "appUserModelId": "App User Model Id value",
            "appId": "App Id value",
            "containedAppId": "Contained App Id value"
          }
        ],
        "showTaskBar": true,
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
  ]
}
```





