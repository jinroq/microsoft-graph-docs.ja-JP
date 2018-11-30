---
title: WindowsKioskConfiguration を作成します。
description: 新しい windowsKioskConfiguration オブジェクトを作成します。
ms.openlocfilehash: 4878ea77d866e29f5b225ba6e50bc3394f3a3545
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068453"
---
# <a name="create-windowskioskconfiguration"></a><span data-ttu-id="d471c-103">WindowsKioskConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="d471c-103">Create windowsKioskConfiguration</span></span>

> <span data-ttu-id="d471c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d471c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d471c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d471c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d471c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d471c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d471c-107">新しい[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d471c-107">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d471c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d471c-108">Prerequisites</span></span>
<span data-ttu-id="d471c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d471c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d471c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d471c-111">Permission type</span></span>|<span data-ttu-id="d471c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d471c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d471c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d471c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d471c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d471c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d471c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d471c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d471c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d471c-116">Not supported.</span></span>|
|<span data-ttu-id="d471c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d471c-117">Application</span></span>|<span data-ttu-id="d471c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d471c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d471c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d471c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d471c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d471c-120">Request headers</span></span>
|<span data-ttu-id="d471c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d471c-121">Header</span></span>|<span data-ttu-id="d471c-122">値</span><span class="sxs-lookup"><span data-stu-id="d471c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d471c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d471c-123">Authorization</span></span>|<span data-ttu-id="d471c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d471c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d471c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d471c-125">Accept</span></span>|<span data-ttu-id="d471c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d471c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d471c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d471c-127">Request body</span></span>
<span data-ttu-id="d471c-128">要求の本文に windowsKioskConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d471c-128">In the request body, supply a JSON representation for the windowsKioskConfiguration object.</span></span>

<span data-ttu-id="d471c-129">次の表は、windowsKioskConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d471c-129">The following table shows the properties that are required when you create the windowsKioskConfiguration.</span></span>

|<span data-ttu-id="d471c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d471c-130">Property</span></span>|<span data-ttu-id="d471c-131">型</span><span class="sxs-lookup"><span data-stu-id="d471c-131">Type</span></span>|<span data-ttu-id="d471c-132">説明</span><span class="sxs-lookup"><span data-stu-id="d471c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d471c-133">id</span><span class="sxs-lookup"><span data-stu-id="d471c-133">id</span></span>|<span data-ttu-id="d471c-134">String</span><span class="sxs-lookup"><span data-stu-id="d471c-134">String</span></span>|<span data-ttu-id="d471c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d471c-135">Key of the entity.</span></span> <span data-ttu-id="d471c-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d471c-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d471c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d471c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d471c-138">DateTimeOffset</span></span>|<span data-ttu-id="d471c-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d471c-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d471c-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d471c-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471c-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d471c-141">roleScopeTagIds</span></span>|<span data-ttu-id="d471c-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d471c-142">String collection</span></span>|<span data-ttu-id="d471c-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="d471c-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d471c-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d471c-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471c-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d471c-145">supportsScopeTags</span></span>|<span data-ttu-id="d471c-146">ブール値</span><span class="sxs-lookup"><span data-stu-id="d471c-146">Boolean</span></span>|<span data-ttu-id="d471c-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d471c-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d471c-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="d471c-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d471c-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="d471c-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d471c-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d471c-150">This property is read-only.</span></span> <span data-ttu-id="d471c-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d471c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471c-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d471c-152">createdDateTime</span></span>|<span data-ttu-id="d471c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d471c-153">DateTimeOffset</span></span>|<span data-ttu-id="d471c-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="d471c-154">DateTime the object was created.</span></span> <span data-ttu-id="d471c-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d471c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471c-156">説明</span><span class="sxs-lookup"><span data-stu-id="d471c-156">description</span></span>|<span data-ttu-id="d471c-157">String</span><span class="sxs-lookup"><span data-stu-id="d471c-157">String</span></span>|<span data-ttu-id="d471c-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="d471c-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d471c-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d471c-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471c-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d471c-160">displayName</span></span>|<span data-ttu-id="d471c-161">String</span><span class="sxs-lookup"><span data-stu-id="d471c-161">String</span></span>|<span data-ttu-id="d471c-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="d471c-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d471c-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d471c-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471c-164">version</span><span class="sxs-lookup"><span data-stu-id="d471c-164">version</span></span>|<span data-ttu-id="d471c-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d471c-165">Int32</span></span>|<span data-ttu-id="d471c-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="d471c-166">Version of the device configuration.</span></span> <span data-ttu-id="d471c-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d471c-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d471c-168">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="d471c-168">kioskProfiles</span></span>|<span data-ttu-id="d471c-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d471c-169">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="d471c-170">このポリシー設定は、構成のキオスクのキオスクのプロファイルの一覧を定義します。</span><span class="sxs-lookup"><span data-stu-id="d471c-170">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="d471c-171">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="d471c-171">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="d471c-172">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="d471c-172">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="d471c-173">String</span><span class="sxs-lookup"><span data-stu-id="d471c-173">String</span></span>|<span data-ttu-id="d471c-174">起動時にブラウザーが移動する必要があります既定の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="d471c-174">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="d471c-175">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="d471c-175">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="d471c-176">ブール値</span><span class="sxs-lookup"><span data-stu-id="d471c-176">Boolean</span></span>|<span data-ttu-id="d471c-177">キオスク ブラウザーの [ホーム] ボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="d471c-177">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="d471c-178">既定では、[ホーム] ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="d471c-178">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="d471c-179">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="d471c-179">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="d471c-180">ブール値</span><span class="sxs-lookup"><span data-stu-id="d471c-180">Boolean</span></span>|<span data-ttu-id="d471c-181">キオスク ブラウザーのナビゲーションの buttons(forward/back) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="d471c-181">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="d471c-182">既定では、ナビゲーション ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="d471c-182">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="d471c-183">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="d471c-183">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="d471c-184">ブール値</span><span class="sxs-lookup"><span data-stu-id="d471c-184">Boolean</span></span>|<span data-ttu-id="d471c-185">キオスク ブラウザーの最後のセッションのボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="d471c-185">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="d471c-186">既定では、セッションの終了] ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="d471c-186">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="d471c-187">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="d471c-187">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="d471c-188">Int32</span><span class="sxs-lookup"><span data-stu-id="d471c-188">Int32</span></span>|<span data-ttu-id="d471c-189">キオスク ブラウザーを最新の状態で再起動するまで、セッションがアイドル状態の分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="d471c-189">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="d471c-190">有効な値は、1 ~ 1440 です。</span><span class="sxs-lookup"><span data-stu-id="d471c-190">Valid values are 1-1440.</span></span> <span data-ttu-id="d471c-191">1 から 1440 の有効な値</span><span class="sxs-lookup"><span data-stu-id="d471c-191">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="d471c-192">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="d471c-192">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="d471c-193">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d471c-193">String collection</span></span>|<span data-ttu-id="d471c-194">キオスクのブラウザーの移動先のない Url を指定します。</span><span class="sxs-lookup"><span data-stu-id="d471c-194">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="d471c-195">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="d471c-195">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="d471c-196">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d471c-196">String collection</span></span>|<span data-ttu-id="d471c-197">キオスクのブラウザーに移動するのには許可されている Url を指定します。</span><span class="sxs-lookup"><span data-stu-id="d471c-197">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|



## <a name="response"></a><span data-ttu-id="d471c-198">応答</span><span class="sxs-lookup"><span data-stu-id="d471c-198">Response</span></span>
<span data-ttu-id="d471c-199">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d471c-199">If successful, this method returns a `201 Created` response code and a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d471c-200">例</span><span class="sxs-lookup"><span data-stu-id="d471c-200">Example</span></span>
### <a name="request"></a><span data-ttu-id="d471c-201">要求</span><span class="sxs-lookup"><span data-stu-id="d471c-201">Request</span></span>
<span data-ttu-id="d471c-202">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d471c-202">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1662

{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
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

### <a name="response"></a><span data-ttu-id="d471c-203">応答</span><span class="sxs-lookup"><span data-stu-id="d471c-203">Response</span></span>
<span data-ttu-id="d471c-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d471c-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





