---
title: androidForWorkWiFiConfiguration リソースの種類
description: このプロファイルの構成を提供することで、必要な Wi-fi のエンドポイントに接続する作業のデバイスの Android を指示できます。 指定する認証方法とセキュリティの種類必要 Wi-fi エンドポイントで行うことができます Wi-fi 接続シームレスなエンド ・ ユーザーのです。 このプロファイルは、エンタープライズ Wi-fi プロファイルよりも制限し、簡単なセキュリティの種類を提供します。
author: tfitzmac
ms.openlocfilehash: f97ede18744ea357e07f741b59ad2af22a0cee6e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337066"
---
# <a name="androidforworkwificonfiguration-resource-type"></a><span data-ttu-id="7391d-105">androidForWorkWiFiConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7391d-105">androidForWorkWiFiConfiguration resource type</span></span>

> <span data-ttu-id="7391d-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7391d-106">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7391d-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7391d-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7391d-108">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7391d-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7391d-109">このプロファイルの構成を提供することで、必要な Wi-fi のエンドポイントに接続する作業のデバイスの Android を指示できます。</span><span class="sxs-lookup"><span data-stu-id="7391d-109">By providing the configurations in this profile you can instruct the Android for Work device to connect to desired Wi-Fi endpoint.</span></span> <span data-ttu-id="7391d-110">指定する認証方法とセキュリティの種類必要 Wi-fi エンドポイントで行うことができます Wi-fi 接続シームレスなエンド ・ ユーザーのです。</span><span class="sxs-lookup"><span data-stu-id="7391d-110">By specifying the authentication method and security types expected by Wi-Fi endpoint you can make the Wi-Fi connection seamless for end user.</span></span> <span data-ttu-id="7391d-111">このプロファイルは、エンタープライズ Wi-fi プロファイルよりも制限し、簡単なセキュリティの種類を提供します。</span><span class="sxs-lookup"><span data-stu-id="7391d-111">This profile provides limited and simpler security types than Enterprise Wi-Fi profile.</span></span>

<span data-ttu-id="7391d-112">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-112">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7391d-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="7391d-113">Methods</span></span>
|<span data-ttu-id="7391d-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="7391d-114">Method</span></span>|<span data-ttu-id="7391d-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7391d-115">Return Type</span></span>|<span data-ttu-id="7391d-116">説明</span><span class="sxs-lookup"><span data-stu-id="7391d-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7391d-117">リスト androidForWorkWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="7391d-117">List androidForWorkWiFiConfigurations</span></span>](../api/intune-deviceconfig-androidforworkwificonfiguration-list.md)|<span data-ttu-id="7391d-118">[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7391d-118">[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) collection</span></span>|<span data-ttu-id="7391d-119">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7391d-119">List properties and relationships of the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) objects.</span></span>|
|[<span data-ttu-id="7391d-120">AndroidForWorkWiFiConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="7391d-120">Get androidForWorkWiFiConfiguration</span></span>](../api/intune-deviceconfig-androidforworkwificonfiguration-get.md)|[<span data-ttu-id="7391d-121">androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="7391d-121">androidForWorkWiFiConfiguration</span></span>](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|<span data-ttu-id="7391d-122">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7391d-122">Read properties and relationships of the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>|
|[<span data-ttu-id="7391d-123">AndroidForWorkWiFiConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="7391d-123">Create androidForWorkWiFiConfiguration</span></span>](../api/intune-deviceconfig-androidforworkwificonfiguration-create.md)|[<span data-ttu-id="7391d-124">androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="7391d-124">androidForWorkWiFiConfiguration</span></span>](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|<span data-ttu-id="7391d-125">新しい[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7391d-125">Create a new [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>|
|[<span data-ttu-id="7391d-126">AndroidForWorkWiFiConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="7391d-126">Delete androidForWorkWiFiConfiguration</span></span>](../api/intune-deviceconfig-androidforworkwificonfiguration-delete.md)|<span data-ttu-id="7391d-127">なし</span><span class="sxs-lookup"><span data-stu-id="7391d-127">None</span></span>|<span data-ttu-id="7391d-128">の[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="7391d-128">Deletes a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>|
|[<span data-ttu-id="7391d-129">AndroidForWorkWiFiConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="7391d-129">Update androidForWorkWiFiConfiguration</span></span>](../api/intune-deviceconfig-androidforworkwificonfiguration-update.md)|[<span data-ttu-id="7391d-130">androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="7391d-130">androidForWorkWiFiConfiguration</span></span>](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)|<span data-ttu-id="7391d-131">[AndroidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7391d-131">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7391d-132">Properties</span><span class="sxs-lookup"><span data-stu-id="7391d-132">Properties</span></span>
|<span data-ttu-id="7391d-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7391d-133">Property</span></span>|<span data-ttu-id="7391d-134">種類</span><span class="sxs-lookup"><span data-stu-id="7391d-134">Type</span></span>|<span data-ttu-id="7391d-135">説明</span><span class="sxs-lookup"><span data-stu-id="7391d-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7391d-136">ID</span><span class="sxs-lookup"><span data-stu-id="7391d-136">id</span></span>|<span data-ttu-id="7391d-137">String</span><span class="sxs-lookup"><span data-stu-id="7391d-137">String</span></span>|<span data-ttu-id="7391d-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7391d-138">Key of the entity.</span></span> <span data-ttu-id="7391d-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7391d-140">lastModifiedDateTime</span></span>|<span data-ttu-id="7391d-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7391d-141">DateTimeOffset</span></span>|<span data-ttu-id="7391d-142">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7391d-142">DateTime the object was last modified.</span></span> <span data-ttu-id="7391d-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-144">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7391d-144">roleScopeTagIds</span></span>|<span data-ttu-id="7391d-145">String コレクション</span><span class="sxs-lookup"><span data-stu-id="7391d-145">String collection</span></span>|<span data-ttu-id="7391d-146">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="7391d-146">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7391d-147">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-148">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7391d-148">supportsScopeTags</span></span>|<span data-ttu-id="7391d-149">ブール型</span><span class="sxs-lookup"><span data-stu-id="7391d-149">Boolean</span></span>|<span data-ttu-id="7391d-150">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7391d-150">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7391d-151">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="7391d-151">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7391d-152">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="7391d-152">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7391d-153">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7391d-153">This property is read-only.</span></span> <span data-ttu-id="7391d-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7391d-155">createdDateTime</span></span>|<span data-ttu-id="7391d-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7391d-156">DateTimeOffset</span></span>|<span data-ttu-id="7391d-157">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="7391d-157">DateTime the object was created.</span></span> <span data-ttu-id="7391d-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-159">説明</span><span class="sxs-lookup"><span data-stu-id="7391d-159">description</span></span>|<span data-ttu-id="7391d-160">String</span><span class="sxs-lookup"><span data-stu-id="7391d-160">String</span></span>|<span data-ttu-id="7391d-161">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="7391d-161">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7391d-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-163">displayName</span><span class="sxs-lookup"><span data-stu-id="7391d-163">displayName</span></span>|<span data-ttu-id="7391d-164">String</span><span class="sxs-lookup"><span data-stu-id="7391d-164">String</span></span>|<span data-ttu-id="7391d-165">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="7391d-165">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7391d-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-167">version</span><span class="sxs-lookup"><span data-stu-id="7391d-167">version</span></span>|<span data-ttu-id="7391d-168">Int32</span><span class="sxs-lookup"><span data-stu-id="7391d-168">Int32</span></span>|<span data-ttu-id="7391d-169">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="7391d-169">Version of the device configuration.</span></span> <span data-ttu-id="7391d-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-171">ネットワーク名リソース</span><span class="sxs-lookup"><span data-stu-id="7391d-171">networkName</span></span>|<span data-ttu-id="7391d-172">String</span><span class="sxs-lookup"><span data-stu-id="7391d-172">String</span></span>|<span data-ttu-id="7391d-173">ネットワーク名</span><span class="sxs-lookup"><span data-stu-id="7391d-173">Network Name</span></span>|
|<span data-ttu-id="7391d-174">ssid</span><span class="sxs-lookup"><span data-stu-id="7391d-174">ssid</span></span>|<span data-ttu-id="7391d-175">String</span><span class="sxs-lookup"><span data-stu-id="7391d-175">String</span></span>|<span data-ttu-id="7391d-176">これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。</span><span class="sxs-lookup"><span data-stu-id="7391d-176">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="7391d-177">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="7391d-177">connectAutomatically</span></span>|<span data-ttu-id="7391d-178">ブール型</span><span class="sxs-lookup"><span data-stu-id="7391d-178">Boolean</span></span>|<span data-ttu-id="7391d-179">このネットワークが範囲内にすると自動的に接続します。</span><span class="sxs-lookup"><span data-stu-id="7391d-179">Connect automatically when this network is in range.</span></span> <span data-ttu-id="7391d-180">これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。</span><span class="sxs-lookup"><span data-stu-id="7391d-180">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="7391d-181">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="7391d-181">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="7391d-182">ブール型</span><span class="sxs-lookup"><span data-stu-id="7391d-182">Boolean</span></span>|<span data-ttu-id="7391d-183">True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。</span><span class="sxs-lookup"><span data-stu-id="7391d-183">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="7391d-184">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="7391d-184">wiFiSecurityType</span></span>|[<span data-ttu-id="7391d-185">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="7391d-185">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="7391d-186">Wi-fi エンドポイントがベースの EAP セキュリティ タイプを使用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7391d-186">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="7391d-187">可能な値: `open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="7391d-187">Possible values are: `open`, `wpaEnterprise`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7391d-188">関係</span><span class="sxs-lookup"><span data-stu-id="7391d-188">Relationships</span></span>
|<span data-ttu-id="7391d-189">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7391d-189">Relationship</span></span>|<span data-ttu-id="7391d-190">型</span><span class="sxs-lookup"><span data-stu-id="7391d-190">Type</span></span>|<span data-ttu-id="7391d-191">説明</span><span class="sxs-lookup"><span data-stu-id="7391d-191">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7391d-192">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="7391d-192">groupAssignments</span></span>|<span data-ttu-id="7391d-193">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7391d-193">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="7391d-194">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="7391d-194">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="7391d-195">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-195">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-196">assignments</span><span class="sxs-lookup"><span data-stu-id="7391d-196">assignments</span></span>|<span data-ttu-id="7391d-197">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7391d-197">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="7391d-198">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="7391d-198">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="7391d-199">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-199">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-200">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7391d-200">deviceStatuses</span></span>|<span data-ttu-id="7391d-201">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7391d-201">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="7391d-202">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="7391d-202">Device configuration installation status by device.</span></span> <span data-ttu-id="7391d-203">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-203">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-204">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7391d-204">userStatuses</span></span>|<span data-ttu-id="7391d-205">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7391d-205">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="7391d-206">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="7391d-206">Device configuration installation status by user.</span></span> <span data-ttu-id="7391d-207">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7391d-207">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-208">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7391d-208">deviceStatusOverview</span></span>|[<span data-ttu-id="7391d-209">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="7391d-209">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="7391d-210">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="7391d-210">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-211">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="7391d-211">userStatusOverview</span></span>|[<span data-ttu-id="7391d-212">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="7391d-212">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="7391d-213">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="7391d-213">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7391d-214">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="7391d-214">deviceSettingStateSummaries</span></span>|<span data-ttu-id="7391d-215">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7391d-215">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="7391d-216">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="7391d-216">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7391d-217">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7391d-217">JSON Representation</span></span>
<span data-ttu-id="7391d-218">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7391d-218">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String"
}
```




