---
title: windowsKioskConfiguration リソースの種類
description: このエンティティは、宣言されたメソッド、プロパティおよびキオスクのリソースによって公開されているリレーションシップの説明を提供します。
ms.openlocfilehash: 94e1f7ee29b97e3ea87cec285a33b86eed989bd4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069575"
---
# <a name="windowskioskconfiguration-resource-type"></a><span data-ttu-id="8717b-103">windowsKioskConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8717b-103">windowsKioskConfiguration resource type</span></span>

> <span data-ttu-id="8717b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8717b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8717b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8717b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8717b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8717b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8717b-107">このエンティティは、宣言されたメソッド、プロパティおよびキオスクのリソースによって公開されているリレーションシップの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="8717b-107">This entity provides descriptions of the declared methods, properties and relationships exposed by the kiosk resource.</span></span>

<span data-ttu-id="8717b-108">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-108">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8717b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8717b-109">Methods</span></span>
|<span data-ttu-id="8717b-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="8717b-110">Method</span></span>|<span data-ttu-id="8717b-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8717b-111">Return Type</span></span>|<span data-ttu-id="8717b-112">説明</span><span class="sxs-lookup"><span data-stu-id="8717b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8717b-113">リスト windowsKioskConfigurations</span><span class="sxs-lookup"><span data-stu-id="8717b-113">List windowsKioskConfigurations</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|<span data-ttu-id="8717b-114">[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-114">[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) collection</span></span>|<span data-ttu-id="8717b-115">[WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8717b-115">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="8717b-116">WindowsKioskConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="8717b-116">Get windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[<span data-ttu-id="8717b-117">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="8717b-117">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="8717b-118">[WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8717b-118">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8717b-119">WindowsKioskConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="8717b-119">Create windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[<span data-ttu-id="8717b-120">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="8717b-120">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="8717b-121">新しい[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8717b-121">Create a new [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|
|[<span data-ttu-id="8717b-122">WindowsKioskConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="8717b-122">Delete windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|<span data-ttu-id="8717b-123">なし</span><span class="sxs-lookup"><span data-stu-id="8717b-123">None</span></span>|<span data-ttu-id="8717b-124">の[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8717b-124">Deletes a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md).</span></span>|
|[<span data-ttu-id="8717b-125">WindowsKioskConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="8717b-125">Update windowsKioskConfiguration</span></span>](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[<span data-ttu-id="8717b-126">windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="8717b-126">windowsKioskConfiguration</span></span>](../resources/intune-deviceconfig-windowskioskconfiguration.md)|<span data-ttu-id="8717b-127">[WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8717b-127">Update the properties of a [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8717b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8717b-128">Properties</span></span>
|<span data-ttu-id="8717b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8717b-129">Property</span></span>|<span data-ttu-id="8717b-130">型</span><span class="sxs-lookup"><span data-stu-id="8717b-130">Type</span></span>|<span data-ttu-id="8717b-131">説明</span><span class="sxs-lookup"><span data-stu-id="8717b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8717b-132">id</span><span class="sxs-lookup"><span data-stu-id="8717b-132">id</span></span>|<span data-ttu-id="8717b-133">String</span><span class="sxs-lookup"><span data-stu-id="8717b-133">String</span></span>|<span data-ttu-id="8717b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8717b-134">Key of the entity.</span></span> <span data-ttu-id="8717b-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8717b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8717b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8717b-137">DateTimeOffset</span></span>|<span data-ttu-id="8717b-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8717b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8717b-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8717b-140">roleScopeTagIds</span></span>|<span data-ttu-id="8717b-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-141">String collection</span></span>|<span data-ttu-id="8717b-142">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="8717b-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8717b-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8717b-144">supportsScopeTags</span></span>|<span data-ttu-id="8717b-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717b-145">Boolean</span></span>|<span data-ttu-id="8717b-146">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8717b-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8717b-147">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="8717b-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8717b-148">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="8717b-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8717b-149">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8717b-149">This property is read-only.</span></span> <span data-ttu-id="8717b-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8717b-151">createdDateTime</span></span>|<span data-ttu-id="8717b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8717b-152">DateTimeOffset</span></span>|<span data-ttu-id="8717b-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8717b-153">DateTime the object was created.</span></span> <span data-ttu-id="8717b-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-155">説明</span><span class="sxs-lookup"><span data-stu-id="8717b-155">description</span></span>|<span data-ttu-id="8717b-156">String</span><span class="sxs-lookup"><span data-stu-id="8717b-156">String</span></span>|<span data-ttu-id="8717b-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="8717b-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8717b-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8717b-159">displayName</span></span>|<span data-ttu-id="8717b-160">String</span><span class="sxs-lookup"><span data-stu-id="8717b-160">String</span></span>|<span data-ttu-id="8717b-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="8717b-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8717b-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-163">version</span><span class="sxs-lookup"><span data-stu-id="8717b-163">version</span></span>|<span data-ttu-id="8717b-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8717b-164">Int32</span></span>|<span data-ttu-id="8717b-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8717b-165">Version of the device configuration.</span></span> <span data-ttu-id="8717b-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-167">kioskProfiles</span><span class="sxs-lookup"><span data-stu-id="8717b-167">kioskProfiles</span></span>|<span data-ttu-id="8717b-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-168">[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md) collection</span></span>|<span data-ttu-id="8717b-169">このポリシー設定は、構成のキオスクのキオスクのプロファイルの一覧を定義します。</span><span class="sxs-lookup"><span data-stu-id="8717b-169">This policy setting allows to define a list of Kiosk profiles for a Kiosk configuration.</span></span> <span data-ttu-id="8717b-170">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="8717b-170">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="8717b-171">kioskBrowserDefaultUrl</span><span class="sxs-lookup"><span data-stu-id="8717b-171">kioskBrowserDefaultUrl</span></span>|<span data-ttu-id="8717b-172">String</span><span class="sxs-lookup"><span data-stu-id="8717b-172">String</span></span>|<span data-ttu-id="8717b-173">起動時にブラウザーが移動する必要があります既定の URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="8717b-173">Specify the default URL the browser should navigate to on launch.</span></span>|
|<span data-ttu-id="8717b-174">kioskBrowserEnableHomeButton</span><span class="sxs-lookup"><span data-stu-id="8717b-174">kioskBrowserEnableHomeButton</span></span>|<span data-ttu-id="8717b-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717b-175">Boolean</span></span>|<span data-ttu-id="8717b-176">キオスク ブラウザーの [ホーム] ボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="8717b-176">Enable the kiosk browser's home button.</span></span> <span data-ttu-id="8717b-177">既定では、[ホーム] ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="8717b-177">By default, the home button is disabled.</span></span>|
|<span data-ttu-id="8717b-178">kioskBrowserEnableNavigationButtons</span><span class="sxs-lookup"><span data-stu-id="8717b-178">kioskBrowserEnableNavigationButtons</span></span>|<span data-ttu-id="8717b-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717b-179">Boolean</span></span>|<span data-ttu-id="8717b-180">キオスク ブラウザーのナビゲーションの buttons(forward/back) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="8717b-180">Enable the kiosk browser's navigation buttons(forward/back).</span></span> <span data-ttu-id="8717b-181">既定では、ナビゲーション ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="8717b-181">By default, the navigation buttons are disabled.</span></span>|
|<span data-ttu-id="8717b-182">kioskBrowserEnableEndSessionButton</span><span class="sxs-lookup"><span data-stu-id="8717b-182">kioskBrowserEnableEndSessionButton</span></span>|<span data-ttu-id="8717b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="8717b-183">Boolean</span></span>|<span data-ttu-id="8717b-184">キオスク ブラウザーの最後のセッションのボタンを有効にします。</span><span class="sxs-lookup"><span data-stu-id="8717b-184">Enable the kiosk browser's end session button.</span></span> <span data-ttu-id="8717b-185">既定では、セッションの終了] ボタンは無効になります。</span><span class="sxs-lookup"><span data-stu-id="8717b-185">By default, the end session button is disabled.</span></span>|
|<span data-ttu-id="8717b-186">kioskBrowserRestartOnIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="8717b-186">kioskBrowserRestartOnIdleTimeInMinutes</span></span>|<span data-ttu-id="8717b-187">Int32</span><span class="sxs-lookup"><span data-stu-id="8717b-187">Int32</span></span>|<span data-ttu-id="8717b-188">キオスク ブラウザーを最新の状態で再起動するまで、セッションがアイドル状態の分数を指定します。</span><span class="sxs-lookup"><span data-stu-id="8717b-188">Specify the number of minutes the session is idle until the kiosk browser restarts in a fresh state.</span></span>  <span data-ttu-id="8717b-189">有効な値は、1 ~ 1440 です。</span><span class="sxs-lookup"><span data-stu-id="8717b-189">Valid values are 1-1440.</span></span> <span data-ttu-id="8717b-190">1 から 1440 の有効な値</span><span class="sxs-lookup"><span data-stu-id="8717b-190">Valid values 1 to 1440</span></span>|
|<span data-ttu-id="8717b-191">kioskBrowserBlockedURLs</span><span class="sxs-lookup"><span data-stu-id="8717b-191">kioskBrowserBlockedURLs</span></span>|<span data-ttu-id="8717b-192">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-192">String collection</span></span>|<span data-ttu-id="8717b-193">キオスクのブラウザーの移動先のない Url を指定します。</span><span class="sxs-lookup"><span data-stu-id="8717b-193">Specify URLs that the kiosk browsers should not navigate to</span></span>|
|<span data-ttu-id="8717b-194">kioskBrowserBlockedUrlExceptions</span><span class="sxs-lookup"><span data-stu-id="8717b-194">kioskBrowserBlockedUrlExceptions</span></span>|<span data-ttu-id="8717b-195">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-195">String collection</span></span>|<span data-ttu-id="8717b-196">キオスクのブラウザーに移動するのには許可されている Url を指定します。</span><span class="sxs-lookup"><span data-stu-id="8717b-196">Specify URLs that the kiosk browser is allowed to navigate to</span></span>|

## <a name="relationships"></a><span data-ttu-id="8717b-197">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8717b-197">Relationships</span></span>
|<span data-ttu-id="8717b-198">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8717b-198">Relationship</span></span>|<span data-ttu-id="8717b-199">型</span><span class="sxs-lookup"><span data-stu-id="8717b-199">Type</span></span>|<span data-ttu-id="8717b-200">説明</span><span class="sxs-lookup"><span data-stu-id="8717b-200">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8717b-201">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="8717b-201">groupAssignments</span></span>|<span data-ttu-id="8717b-202">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-202">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="8717b-203">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="8717b-203">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="8717b-204">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-204">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-205">assignments</span><span class="sxs-lookup"><span data-stu-id="8717b-205">assignments</span></span>|<span data-ttu-id="8717b-206">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-206">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="8717b-207">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="8717b-207">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="8717b-208">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-208">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-209">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="8717b-209">deviceStatuses</span></span>|<span data-ttu-id="8717b-210">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-210">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="8717b-211">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="8717b-211">Device configuration installation status by device.</span></span> <span data-ttu-id="8717b-212">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-212">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-213">userStatuses</span><span class="sxs-lookup"><span data-stu-id="8717b-213">userStatuses</span></span>|<span data-ttu-id="8717b-214">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-214">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="8717b-215">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="8717b-215">Device configuration installation status by user.</span></span> <span data-ttu-id="8717b-216">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8717b-216">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-217">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8717b-217">deviceStatusOverview</span></span>|[<span data-ttu-id="8717b-218">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="8717b-218">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="8717b-219">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="8717b-219">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-220">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="8717b-220">userStatusOverview</span></span>|[<span data-ttu-id="8717b-221">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="8717b-221">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="8717b-222">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="8717b-222">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8717b-223">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="8717b-223">deviceSettingStateSummaries</span></span>|<span data-ttu-id="8717b-224">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8717b-224">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="8717b-225">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="8717b-225">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8717b-226">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8717b-226">JSON Representation</span></span>
<span data-ttu-id="8717b-227">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8717b-227">Here is a JSON representation of the resource.</span></span>
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
            "appUserModelId": "String",
            "appId": "String",
            "containedAppId": "String"
          }
        ],
        "showTaskBar": true,
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
  ]
}
```




