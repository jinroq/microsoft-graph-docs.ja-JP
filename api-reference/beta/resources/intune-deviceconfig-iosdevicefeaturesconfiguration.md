---
title: iosDeviceFeaturesConfiguration リソースの種類
description: iOS デバイス機能構成のプロファイル。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1a3ac4ef0d2743a81ac5b3f02822677c264e02fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835491"
---
# <a name="iosdevicefeaturesconfiguration-resource-type"></a><span data-ttu-id="51245-103">iosDeviceFeaturesConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51245-103">iosDeviceFeaturesConfiguration resource type</span></span>

> <span data-ttu-id="51245-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51245-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51245-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51245-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51245-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="51245-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51245-107">iOS デバイス機能構成のプロファイル。</span><span class="sxs-lookup"><span data-stu-id="51245-107">iOS Device Features Configuration Profile.</span></span>

<span data-ttu-id="51245-108">[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-108">Inherits from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="51245-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="51245-109">Methods</span></span>
|<span data-ttu-id="51245-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="51245-110">Method</span></span>|<span data-ttu-id="51245-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="51245-111">Return Type</span></span>|<span data-ttu-id="51245-112">説明</span><span class="sxs-lookup"><span data-stu-id="51245-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="51245-113">iosDeviceFeaturesConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="51245-113">List iosDeviceFeaturesConfigurations</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-list.md)|<span data-ttu-id="51245-114">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-114">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) collection</span></span>|<span data-ttu-id="51245-115">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="51245-115">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="51245-116">iosDeviceFeaturesConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="51245-116">Get iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-get.md)|[<span data-ttu-id="51245-117">iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="51245-117">iosDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)|<span data-ttu-id="51245-118">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="51245-118">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="51245-119">iosDeviceFeaturesConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="51245-119">Create iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-create.md)|[<span data-ttu-id="51245-120">iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="51245-120">iosDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)|<span data-ttu-id="51245-121">新しい [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="51245-121">Create a new [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>|
|[<span data-ttu-id="51245-122">iosDeviceFeaturesConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="51245-122">Delete iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-delete.md)|<span data-ttu-id="51245-123">なし</span><span class="sxs-lookup"><span data-stu-id="51245-123">None</span></span>|<span data-ttu-id="51245-124">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="51245-124">Deletes a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span></span>|
|[<span data-ttu-id="51245-125">iosDeviceFeaturesConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="51245-125">Update iosDeviceFeaturesConfiguration</span></span>](../api/intune-deviceconfig-iosdevicefeaturesconfiguration-update.md)|[<span data-ttu-id="51245-126">iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="51245-126">iosDeviceFeaturesConfiguration</span></span>](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md)|<span data-ttu-id="51245-127">[iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="51245-127">Update the properties of a [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="51245-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51245-128">Properties</span></span>
|<span data-ttu-id="51245-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51245-129">Property</span></span>|<span data-ttu-id="51245-130">種類</span><span class="sxs-lookup"><span data-stu-id="51245-130">Type</span></span>|<span data-ttu-id="51245-131">説明</span><span class="sxs-lookup"><span data-stu-id="51245-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51245-132">ID</span><span class="sxs-lookup"><span data-stu-id="51245-132">id</span></span>|<span data-ttu-id="51245-133">String</span><span class="sxs-lookup"><span data-stu-id="51245-133">String</span></span>|<span data-ttu-id="51245-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="51245-134">Key of the entity.</span></span> <span data-ttu-id="51245-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51245-136">lastModifiedDateTime</span></span>|<span data-ttu-id="51245-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51245-137">DateTimeOffset</span></span>|<span data-ttu-id="51245-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="51245-138">DateTime the object was last modified.</span></span> <span data-ttu-id="51245-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51245-140">roleScopeTagIds</span></span>|<span data-ttu-id="51245-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-141">String collection</span></span>|<span data-ttu-id="51245-142">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="51245-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="51245-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="51245-144">supportsScopeTags</span></span>|<span data-ttu-id="51245-145">ブール型</span><span class="sxs-lookup"><span data-stu-id="51245-145">Boolean</span></span>|<span data-ttu-id="51245-146">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="51245-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="51245-147">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="51245-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="51245-148">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="51245-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="51245-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="51245-149">This property is read-only.</span></span> <span data-ttu-id="51245-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51245-151">createdDateTime</span></span>|<span data-ttu-id="51245-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51245-152">DateTimeOffset</span></span>|<span data-ttu-id="51245-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="51245-153">DateTime the object was created.</span></span> <span data-ttu-id="51245-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-155">説明</span><span class="sxs-lookup"><span data-stu-id="51245-155">description</span></span>|<span data-ttu-id="51245-156">String</span><span class="sxs-lookup"><span data-stu-id="51245-156">String</span></span>|<span data-ttu-id="51245-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="51245-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51245-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-159">displayName</span><span class="sxs-lookup"><span data-stu-id="51245-159">displayName</span></span>|<span data-ttu-id="51245-160">String</span><span class="sxs-lookup"><span data-stu-id="51245-160">String</span></span>|<span data-ttu-id="51245-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="51245-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51245-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-163">version</span><span class="sxs-lookup"><span data-stu-id="51245-163">version</span></span>|<span data-ttu-id="51245-164">Int32</span><span class="sxs-lookup"><span data-stu-id="51245-164">Int32</span></span>|<span data-ttu-id="51245-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="51245-165">Version of the device configuration.</span></span> <span data-ttu-id="51245-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="51245-167">airPrintDestinations</span></span>|<span data-ttu-id="51245-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="51245-169">常に表示されている必要があります AirPrint プリンターの配列。</span><span class="sxs-lookup"><span data-stu-id="51245-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="51245-170">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="51245-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="51245-171">[AppleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="51245-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|
|<span data-ttu-id="51245-172">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="51245-172">assetTagTemplate</span></span>|<span data-ttu-id="51245-173">String</span><span class="sxs-lookup"><span data-stu-id="51245-173">String</span></span>|<span data-ttu-id="51245-174">ログイン ウィンドウとロック画面に表示される、デバイスの資産タグ情報です。</span><span class="sxs-lookup"><span data-stu-id="51245-174">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="51245-175">contentFilterSettings</span><span class="sxs-lookup"><span data-stu-id="51245-175">contentFilterSettings</span></span>|[<span data-ttu-id="51245-176">iosWebContentFilterBase</span><span class="sxs-lookup"><span data-stu-id="51245-176">iosWebContentFilterBase</span></span>](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)|<span data-ttu-id="51245-177">Web コンテンツ フィルター設定、コールを管理モードでのみを設定するには、iOS を取得または</span><span class="sxs-lookup"><span data-stu-id="51245-177">Gets or sets iOS Web Content Filter settings, supervised mode only</span></span>|
|<span data-ttu-id="51245-178">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="51245-178">lockScreenFootnote</span></span>|<span data-ttu-id="51245-179">String</span><span class="sxs-lookup"><span data-stu-id="51245-179">String</span></span>|<span data-ttu-id="51245-180">ログイン ウィンドウとロック画面に表示される脚注です。</span><span class="sxs-lookup"><span data-stu-id="51245-180">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="51245-181">IOS 9.3.1 以降で利用可能です。</span><span class="sxs-lookup"><span data-stu-id="51245-181">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="51245-182">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="51245-182">homeScreenDockIcons</span></span>|<span data-ttu-id="51245-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-183">[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="51245-184">ホーム画面ドックに表示されるアプリとフォルダーのリスト。</span><span class="sxs-lookup"><span data-stu-id="51245-184">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="51245-185">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="51245-185">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="51245-186">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="51245-186">homeScreenPages</span></span>|<span data-ttu-id="51245-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-187">[iosHomeScreenPage](../resources/intune-deviceconfig-ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="51245-188">ホーム画面上のページのリスト。</span><span class="sxs-lookup"><span data-stu-id="51245-188">A list of pages on the Home Screen.</span></span> <span data-ttu-id="51245-189">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="51245-189">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="51245-190">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="51245-190">notificationSettings</span></span>|<span data-ttu-id="51245-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-191">[iosNotificationSettings](../resources/intune-deviceconfig-iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="51245-192">各バンドル ID ごとの通知設定。監視モードのデバイスにのみ (iOS 9.3 以降) 適用されます。</span><span class="sxs-lookup"><span data-stu-id="51245-192">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="51245-193">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="51245-193">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="51245-194">singleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="51245-194">singleSignOnSettings</span></span>|[<span data-ttu-id="51245-195">iosSingleSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="51245-195">iosSingleSignOnSettings</span></span>](../resources/intune-deviceconfig-iossinglesignonsettings.md)|<span data-ttu-id="51245-196">受信認証をスムーズにするためにデバイス上のアプリを有効にする Kerberos ログインの設定です。</span><span class="sxs-lookup"><span data-stu-id="51245-196">The Kerberos login settings that enable apps on receiving devices to authenticate smoothly.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51245-197">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="51245-197">Relationships</span></span>
|<span data-ttu-id="51245-198">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="51245-198">Relationship</span></span>|<span data-ttu-id="51245-199">型</span><span class="sxs-lookup"><span data-stu-id="51245-199">Type</span></span>|<span data-ttu-id="51245-200">説明</span><span class="sxs-lookup"><span data-stu-id="51245-200">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51245-201">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="51245-201">groupAssignments</span></span>|<span data-ttu-id="51245-202">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-202">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="51245-203">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="51245-203">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="51245-204">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-204">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-205">assignments</span><span class="sxs-lookup"><span data-stu-id="51245-205">assignments</span></span>|<span data-ttu-id="51245-206">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-206">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="51245-207">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="51245-207">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="51245-208">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-208">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-209">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="51245-209">deviceStatuses</span></span>|<span data-ttu-id="51245-210">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-210">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="51245-211">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="51245-211">Device configuration installation status by device.</span></span> <span data-ttu-id="51245-212">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-212">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-213">userStatuses</span><span class="sxs-lookup"><span data-stu-id="51245-213">userStatuses</span></span>|<span data-ttu-id="51245-214">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-214">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="51245-215">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="51245-215">Device configuration installation status by user.</span></span> <span data-ttu-id="51245-216">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51245-216">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-217">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="51245-217">deviceStatusOverview</span></span>|[<span data-ttu-id="51245-218">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="51245-218">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="51245-219">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="51245-219">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-220">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="51245-220">userStatusOverview</span></span>|[<span data-ttu-id="51245-221">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="51245-221">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="51245-222">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="51245-222">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-223">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="51245-223">deviceSettingStateSummaries</span></span>|<span data-ttu-id="51245-224">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51245-224">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="51245-225">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="51245-225">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51245-226">identityCertificateForClientAuthentication</span><span class="sxs-lookup"><span data-stu-id="51245-226">identityCertificateForClientAuthentication</span></span>|[<span data-ttu-id="51245-227">iosCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="51245-227">iosCertificateProfileBase</span></span>](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|<span data-ttu-id="51245-228">シングル サインオンの設定で使用される Kerberos チケットの更新のための id の証明書です。</span><span class="sxs-lookup"><span data-stu-id="51245-228">Identity Certificate for the renewal of Kerberos ticket used in single sign-on settings.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51245-229">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51245-229">JSON Representation</span></span>
<span data-ttu-id="51245-230">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="51245-230">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosDeviceFeaturesConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "String",
      "resourcePath": "String",
      "port": 1024,
      "forceTls": true
    }
  ],
  "assetTagTemplate": "String",
  "contentFilterSettings": {
    "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
    "specificWebsitesOnly": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "String",
        "bookmarkFolder": "String",
        "displayName": "String"
      }
    ],
    "websiteList": [
      {
        "@odata.type": "microsoft.graph.iosBookmark",
        "url": "String",
        "bookmarkFolder": "String",
        "displayName": "String"
      }
    ]
  },
  "lockScreenFootnote": "String",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "String",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "String",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "String",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "String",
                  "bundleID": "String"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "String",
      "appName": "String",
      "publisher": "String",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "String",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ],
  "singleSignOnSettings": {
    "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
    "allowedAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "String",
        "publisher": "String",
        "appStoreUrl": "String",
        "appId": "String"
      }
    ],
    "allowedUrls": [
      "String"
    ],
    "displayName": "String",
    "kerberosPrincipalName": "String",
    "kerberosRealm": "String"
  }
}
```





