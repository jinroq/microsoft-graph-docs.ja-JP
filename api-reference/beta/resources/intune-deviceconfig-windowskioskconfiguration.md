---
title: windowsKioskConfiguration リソースの種類
description: このエンティティは、kiosk リソースが公開する宣言されたメソッド、プロパティ、リレーションシップについて説明します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d11812d885d6be772c8ecf058658446a56eb99b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370930"
---
# <a name="windowskioskconfiguration-resource-type"></a><span data-ttu-id="95362-103">windowsKioskConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95362-103">windowsKioskConfiguration resource type</span></span>

> <span data-ttu-id="95362-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95362-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95362-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95362-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95362-106">このエンティティは、kiosk リソースが公開する宣言されたメソッド、プロパティ、リレーションシップについて説明します。</span><span class="sxs-lookup"><span data-stu-id="95362-106">This entity provides descriptions of the declared methods, properties and relationships exposed by the kiosk resource.</span></span>


<span data-ttu-id="95362-107">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="95362-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="95362-108">Methods</span></span>
|<span data-ttu-id="95362-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="95362-109">Method</span></span>|<span data-ttu-id="95362-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="95362-110">Return Type</span></span>|<span data-ttu-id="95362-111">説明</span><span class="sxs-lookup"><span data-stu-id="95362-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="95362-112">WindowsKioskConfigurations を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="95362-112">List windowsKioskConfigurations</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|<span data-ttu-id="95362-113">[Windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-113">[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) collection</span></span>|<span data-ttu-id="95362-114">[Windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="95362-114">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="95362-115">WindowsKioskConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="95362-115">Get windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[<span data-ttu-id="95362-116">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="95362-116">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="95362-117">[Windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="95362-117">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="95362-118">WindowsKioskConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="95362-118">Create windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[<span data-ttu-id="95362-119">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="95362-119">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="95362-120">新しい[Windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="95362-120">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="95362-121">WindowsKioskConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="95362-121">Delete windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|<span data-ttu-id="95362-122">None</span><span class="sxs-lookup"><span data-stu-id="95362-122">None</span></span>|<span data-ttu-id="95362-123">[Windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="95362-123">Deletes a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>|
|[<span data-ttu-id="95362-124">WindowsKioskConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="95362-124">Update windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[<span data-ttu-id="95362-125">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="95362-125">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="95362-126">[Windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="95362-126">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="95362-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95362-127">Properties</span></span>
|<span data-ttu-id="95362-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95362-128">Property</span></span>|<span data-ttu-id="95362-129">型</span><span class="sxs-lookup"><span data-stu-id="95362-129">Type</span></span>|<span data-ttu-id="95362-130">説明</span><span class="sxs-lookup"><span data-stu-id="95362-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95362-131">id</span><span class="sxs-lookup"><span data-stu-id="95362-131">id</span></span>|<span data-ttu-id="95362-132">文字列</span><span class="sxs-lookup"><span data-stu-id="95362-132">String</span></span>|<span data-ttu-id="95362-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="95362-133">Key of the entity.</span></span> <span data-ttu-id="95362-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95362-135">lastModifiedDateTime</span></span>|<span data-ttu-id="95362-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95362-136">DateTimeOffset</span></span>|<span data-ttu-id="95362-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="95362-137">DateTime the object was last modified.</span></span> <span data-ttu-id="95362-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95362-139">roleScopeTagIds</span></span>|<span data-ttu-id="95362-140">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-140">String collection</span></span>|<span data-ttu-id="95362-141">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="95362-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95362-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-143">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95362-143">supportsScopeTags</span></span>|<span data-ttu-id="95362-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="95362-144">Boolean</span></span>|<span data-ttu-id="95362-145">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="95362-145">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95362-146">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="95362-146">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95362-147">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="95362-147">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95362-148">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="95362-148">This property is read-only.</span></span> <span data-ttu-id="95362-149">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-149">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-150">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95362-150">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="95362-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="95362-151">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="95362-152">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="95362-152">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="95362-153">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-154">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95362-154">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="95362-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="95362-155">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="95362-156">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="95362-156">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="95362-157">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-158">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="95362-158">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="95362-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="95362-159">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="95362-160">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="95362-160">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="95362-161">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95362-162">createdDateTime</span></span>|<span data-ttu-id="95362-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95362-163">DateTimeOffset</span></span>|<span data-ttu-id="95362-164">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="95362-164">DateTime the object was created.</span></span> <span data-ttu-id="95362-165">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-165">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-166">description</span><span class="sxs-lookup"><span data-stu-id="95362-166">description</span></span>|<span data-ttu-id="95362-167">String</span><span class="sxs-lookup"><span data-stu-id="95362-167">String</span></span>|<span data-ttu-id="95362-168">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="95362-168">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95362-169">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-169">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-170">displayName</span><span class="sxs-lookup"><span data-stu-id="95362-170">displayName</span></span>|<span data-ttu-id="95362-171">String</span><span class="sxs-lookup"><span data-stu-id="95362-171">String</span></span>|<span data-ttu-id="95362-172">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="95362-172">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95362-173">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-173">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-174">version</span><span class="sxs-lookup"><span data-stu-id="95362-174">version</span></span>|<span data-ttu-id="95362-175">Int32</span><span class="sxs-lookup"><span data-stu-id="95362-175">Int32</span></span>|<span data-ttu-id="95362-176">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="95362-176">Version of the device configuration.</span></span> <span data-ttu-id="95362-177">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-177">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-178">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="95362-178">kioskProfiles</span></span>|<span data-ttu-id="95362-179">[Windowskioskprofile](../resources/intune-deviceconfig-windowskioskprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-179">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="95362-180">このポリシー設定を使用すると、キオスクの構成のキオスクプロファイルの一覧を定義できます。</span><span class="sxs-lookup"><span data-stu-id="95362-180">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="95362-181">このコレクションには、最大3つの要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="95362-181">This collection can contain a maximum of 3 elements.</span></span>|
|<span data-ttu-id="95362-182">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="95362-182">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="95362-183">String</span><span class="sxs-lookup"><span data-stu-id="95362-183">String</span></span>|<span data-ttu-id="95362-184">ブラウザーが起動時に移動する既定の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="95362-184">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="95362-185">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="95362-185">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="95362-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="95362-186">Boolean</span></span>|<span data-ttu-id="95362-187">キオスクブラウザーの [ホーム] ボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="95362-187">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="95362-188">既定では、[ホーム] ボタンは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="95362-188">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="95362-189">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="95362-189">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="95362-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="95362-190">Boolean</span></span>|<span data-ttu-id="95362-191">キオスクブラウザーのナビゲーションボタン (前方/後方) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="95362-191">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="95362-192">既定では、ナビゲーションボタンは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="95362-192">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="95362-193">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="95362-193">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="95362-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="95362-194">Boolean</span></span>|<span data-ttu-id="95362-195">キオスクブラウザーの [セッションの終了] ボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="95362-195">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="95362-196">既定では、[セッションの終了] ボタンは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="95362-196">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="95362-197">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="95362-197">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="95362-198">Int32</span><span class="sxs-lookup"><span data-stu-id="95362-198">Int32</span></span>|<span data-ttu-id="95362-199">キオスクブラウザーが新しい状態で再起動するまで、セッションがアイドル状態になっている時間 (分) を指定します。</span><span class="sxs-lookup"><span data-stu-id="95362-199">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="95362-200">有効な値は1-1440 です。</span><span class="sxs-lookup"><span data-stu-id="95362-200">Valid values are 1-1440.</span></span> <span data-ttu-id="95362-201">有効な値は 1 ~ 1440</span><span class="sxs-lookup"><span data-stu-id="95362-201">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="95362-202">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="95362-202">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="95362-203">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-203">String collection</span></span>|<span data-ttu-id="95362-204">キオスクブラウザーが移動しない Url を指定する</span><span class="sxs-lookup"><span data-stu-id="95362-204">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="95362-205">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="95362-205">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="95362-206">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-206">String collection</span></span>|<span data-ttu-id="95362-207">キオスクブラウザーでの移動が許可されている Url を指定する</span><span class="sxs-lookup"><span data-stu-id="95362-207">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|
|<span data-ttu-id="95362-208">edgeKioskEnablePublicBrowsing</span><span class="sxs-lookup"><span data-stu-id="95362-208">edgeKioskEnablePublicBrowsing</span></span>|<span data-ttu-id="95362-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="95362-209">Boolean</span></span>|<span data-ttu-id="95362-210">Microsoft Edge ブラウザーのパブリックブラウズキオスクモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="95362-210">Enable public browsing kiosk mode for the Microsoft Edge browser.</span></span> <span data-ttu-id="95362-211">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="95362-211">The Default is false.</span></span>|
|<span data-ttu-id="95362-212">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="95362-212">windowsKioskForceUpdateSchedule</span></span>|[<span data-ttu-id="95362-213">windowsKioskForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="95362-213">windowsKioskForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windowskioskforceupdateschedule.md)|<span data-ttu-id="95362-214">キオスクデバイスの更新スケジュールを強制します。</span><span class="sxs-lookup"><span data-stu-id="95362-214">force update schedule for Kiosk devices.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95362-215">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95362-215">Relationships</span></span>
|<span data-ttu-id="95362-216">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95362-216">Relationship</span></span>|<span data-ttu-id="95362-217">型</span><span class="sxs-lookup"><span data-stu-id="95362-217">Type</span></span>|<span data-ttu-id="95362-218">説明</span><span class="sxs-lookup"><span data-stu-id="95362-218">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95362-219">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="95362-219">groupAssignments</span></span>|<span data-ttu-id="95362-220">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-220">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="95362-221">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="95362-221">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="95362-222">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-222">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-223">assignments</span><span class="sxs-lookup"><span data-stu-id="95362-223">assignments</span></span>|<span data-ttu-id="95362-224">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-224">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="95362-225">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="95362-225">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="95362-226">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-226">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-227">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="95362-227">deviceStatuses</span></span>|<span data-ttu-id="95362-228">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-228">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="95362-229">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="95362-229">Device configuration installation status by device.</span></span> <span data-ttu-id="95362-230">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-230">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-231">userStatuses</span><span class="sxs-lookup"><span data-stu-id="95362-231">userStatuses</span></span>|<span data-ttu-id="95362-232">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-232">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="95362-233">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="95362-233">Device configuration installation status by user.</span></span> <span data-ttu-id="95362-234">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="95362-234">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-235">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="95362-235">deviceStatusOverview</span></span>|[<span data-ttu-id="95362-236">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="95362-236">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="95362-237">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="95362-237">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-238">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="95362-238">userStatusOverview</span></span>|[<span data-ttu-id="95362-239">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="95362-239">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="95362-240">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="95362-240">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95362-241">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="95362-241">deviceSettingStateSummaries</span></span>|<span data-ttu-id="95362-242">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="95362-242">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="95362-243">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="95362-243">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95362-244">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95362-244">JSON Representation</span></span>
<span data-ttu-id="95362-245">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95362-245">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsKioskConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "String",
      "profileName": "String",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "String",
            "name": "String",
            "appType": "String",
            "autoLaunch": true,
            "appUserModelId": "String",
            "appId": "String",
            "containedAppId": "String"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "binary"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "String",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 1024,
  "kioskBrowserBlockedURLs": [
    "String"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "String"
  ],
  "edgeKioskEnablePublicBrowsing": true,
  "windowsKioskForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
    "startDateTime": "String (timestamp)",
    "recurrence": "String",
    "dayofWeek": "String",
    "dayofMonth": 1024,
    "runImmediatelyIfAfterStartDateTime": true
  }
}
```



