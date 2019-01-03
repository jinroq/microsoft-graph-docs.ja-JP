---
title: networkIPv4ConfigurationManagementCondition リソースの種類
description: 構成ベースの管理条件を定義することも、デバイスが特定の IP を検出したときにトリガーとなる IPv4 ネットワークの設定です。 IP 構成の管理の条件だと考えてよい真のネットワーク接続がアクティブなときです。
author: tfitzmac
ms.openlocfilehash: eba20d0ef5db1667cad2ffb85b9477c9044b28b9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344262"
---
# <a name="networkipv4configurationmanagementcondition-resource-type"></a><span data-ttu-id="9c760-104">networkIPv4ConfigurationManagementCondition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9c760-104">networkIPv4ConfigurationManagementCondition resource type</span></span>

> <span data-ttu-id="9c760-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9c760-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c760-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c760-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c760-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c760-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c760-108">構成ベースの管理条件を定義することも、デバイスが特定の IP を検出したときにトリガーとなる IPv4 ネットワークの設定です。</span><span class="sxs-lookup"><span data-stu-id="9c760-108">IPv4 configuration-based management conditions may be defined that will trigger when a device detects certain IP network settings.</span></span> <span data-ttu-id="9c760-109">IP 構成の管理の条件だと考えてよい真のネットワーク接続がアクティブなときです。</span><span class="sxs-lookup"><span data-stu-id="9c760-109">An IP config management conditions will only be considered TRUE when the network connection is active.</span></span>

<span data-ttu-id="9c760-110">[NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="9c760-110">Inherits from [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)</span></span>

## <a name="methods"></a><span data-ttu-id="9c760-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c760-111">Methods</span></span>
|<span data-ttu-id="9c760-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="9c760-112">Method</span></span>|<span data-ttu-id="9c760-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9c760-113">Return Type</span></span>|<span data-ttu-id="9c760-114">説明</span><span class="sxs-lookup"><span data-stu-id="9c760-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9c760-115">リスト networkIPv4ConfigurationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="9c760-115">List networkIPv4ConfigurationManagementConditions</span></span>](../api/intune-fencing-networkipv4configurationmanagementcondition-list.md)|<span data-ttu-id="9c760-116">[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9c760-116">[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) collection</span></span>|<span data-ttu-id="9c760-117">[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9c760-117">List properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) objects.</span></span>|
|[<span data-ttu-id="9c760-118">NetworkIPv4ConfigurationManagementCondition を取得します。</span><span class="sxs-lookup"><span data-stu-id="9c760-118">Get networkIPv4ConfigurationManagementCondition</span></span>](../api/intune-fencing-networkipv4configurationmanagementcondition-get.md)|[<span data-ttu-id="9c760-119">networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9c760-119">networkIPv4ConfigurationManagementCondition</span></span>](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|<span data-ttu-id="9c760-120">[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c760-120">Read properties and relationships of the [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>|
|[<span data-ttu-id="9c760-121">NetworkIPv4ConfigurationManagementCondition を作成します。</span><span class="sxs-lookup"><span data-stu-id="9c760-121">Create networkIPv4ConfigurationManagementCondition</span></span>](../api/intune-fencing-networkipv4configurationmanagementcondition-create.md)|[<span data-ttu-id="9c760-122">networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9c760-122">networkIPv4ConfigurationManagementCondition</span></span>](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|<span data-ttu-id="9c760-123">新しい[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9c760-123">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>|
|[<span data-ttu-id="9c760-124">NetworkIPv4ConfigurationManagementCondition を削除します。</span><span class="sxs-lookup"><span data-stu-id="9c760-124">Delete networkIPv4ConfigurationManagementCondition</span></span>](../api/intune-fencing-networkipv4configurationmanagementcondition-delete.md)|<span data-ttu-id="9c760-125">なし</span><span class="sxs-lookup"><span data-stu-id="9c760-125">None</span></span>|<span data-ttu-id="9c760-126">の[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="9c760-126">Deletes a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md).</span></span>|
|[<span data-ttu-id="9c760-127">NetworkIPv4ConfigurationManagementCondition を更新します。</span><span class="sxs-lookup"><span data-stu-id="9c760-127">Update networkIPv4ConfigurationManagementCondition</span></span>](../api/intune-fencing-networkipv4configurationmanagementcondition-update.md)|[<span data-ttu-id="9c760-128">networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="9c760-128">networkIPv4ConfigurationManagementCondition</span></span>](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|<span data-ttu-id="9c760-129">[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9c760-129">Update the properties of a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c760-130">Properties</span><span class="sxs-lookup"><span data-stu-id="9c760-130">Properties</span></span>
|<span data-ttu-id="9c760-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c760-131">Property</span></span>|<span data-ttu-id="9c760-132">種類</span><span class="sxs-lookup"><span data-stu-id="9c760-132">Type</span></span>|<span data-ttu-id="9c760-133">説明</span><span class="sxs-lookup"><span data-stu-id="9c760-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c760-134">ID</span><span class="sxs-lookup"><span data-stu-id="9c760-134">id</span></span>|<span data-ttu-id="9c760-135">String</span><span class="sxs-lookup"><span data-stu-id="9c760-135">String</span></span>|<span data-ttu-id="9c760-136">管理条件の一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="9c760-136">Unique identifier for the management condition.</span></span> <span data-ttu-id="9c760-137">システムでは、作成時に割り当てられた値が生成されます。</span><span class="sxs-lookup"><span data-stu-id="9c760-137">System generated value assigned when created.</span></span> <span data-ttu-id="9c760-138">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9c760-138">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c760-139">一意な名前</span><span class="sxs-lookup"><span data-stu-id="9c760-139">uniqueName</span></span>|<span data-ttu-id="9c760-140">String</span><span class="sxs-lookup"><span data-stu-id="9c760-140">String</span></span>|<span data-ttu-id="9c760-141">管理条件の一意の名前です。</span><span class="sxs-lookup"><span data-stu-id="9c760-141">Unique name for the management condition.</span></span> <span data-ttu-id="9c760-142">管理条件式で使用されます。</span><span class="sxs-lookup"><span data-stu-id="9c760-142">Used in management condition expressions.</span></span> <span data-ttu-id="9c760-143">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9c760-143">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c760-144">displayName</span><span class="sxs-lookup"><span data-stu-id="9c760-144">displayName</span></span>|<span data-ttu-id="9c760-145">String</span><span class="sxs-lookup"><span data-stu-id="9c760-145">String</span></span>|<span data-ttu-id="9c760-146">管理者は、管理の条件の名前を定義します。</span><span class="sxs-lookup"><span data-stu-id="9c760-146">The admin defined name of the management condition.</span></span> <span data-ttu-id="9c760-147">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9c760-147">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c760-148">説明</span><span class="sxs-lookup"><span data-stu-id="9c760-148">description</span></span>|<span data-ttu-id="9c760-149">String</span><span class="sxs-lookup"><span data-stu-id="9c760-149">String</span></span>|<span data-ttu-id="9c760-150">管理者は、管理状態の説明を定義します。</span><span class="sxs-lookup"><span data-stu-id="9c760-150">The admin defined description of the management condition.</span></span> <span data-ttu-id="9c760-151">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9c760-151">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c760-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c760-152">createdDateTime</span></span>|<span data-ttu-id="9c760-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c760-153">DateTimeOffset</span></span>|<span data-ttu-id="9c760-154">管理条件が作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="9c760-154">The time the management condition was created.</span></span> <span data-ttu-id="9c760-155">サービス側が生成されます。</span><span class="sxs-lookup"><span data-stu-id="9c760-155">Generated service side.</span></span> <span data-ttu-id="9c760-156">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9c760-156">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c760-157">変更された日時</span><span class="sxs-lookup"><span data-stu-id="9c760-157">modifiedDateTime</span></span>|<span data-ttu-id="9c760-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c760-158">DateTimeOffset</span></span>|<span data-ttu-id="9c760-159">管理条件が最後に修正された時間です。</span><span class="sxs-lookup"><span data-stu-id="9c760-159">The time the management condition was last modified.</span></span> <span data-ttu-id="9c760-160">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="9c760-160">Updated service side.</span></span> <span data-ttu-id="9c760-161">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9c760-161">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c760-162">eTag</span><span class="sxs-lookup"><span data-stu-id="9c760-162">eTag</span></span>|<span data-ttu-id="9c760-163">String</span><span class="sxs-lookup"><span data-stu-id="9c760-163">String</span></span>|<span data-ttu-id="9c760-164">管理条件の ETag。</span><span class="sxs-lookup"><span data-stu-id="9c760-164">ETag of the management condition.</span></span> <span data-ttu-id="9c760-165">サービス側を更新します。</span><span class="sxs-lookup"><span data-stu-id="9c760-165">Updated service side.</span></span> <span data-ttu-id="9c760-166">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9c760-166">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c760-167">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="9c760-167">applicablePlatforms</span></span>|<span data-ttu-id="9c760-168">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9c760-168">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="9c760-169">この管理条件に該当するプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="9c760-169">The applicable platforms for this management condition.</span></span> <span data-ttu-id="9c760-170">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9c760-170">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="9c760-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="9c760-171">ipV4Prefix</span></span>|<span data-ttu-id="9c760-172">String</span><span class="sxs-lookup"><span data-stu-id="9c760-172">String</span></span>|<span data-ttu-id="9c760-173">接続されている IPv4 サブネットです。</span><span class="sxs-lookup"><span data-stu-id="9c760-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="9c760-174">10.0.0.0/8 など</span><span class="sxs-lookup"><span data-stu-id="9c760-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="9c760-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="9c760-175">ipV4Gateway</span></span>|<span data-ttu-id="9c760-176">String</span><span class="sxs-lookup"><span data-stu-id="9c760-176">String</span></span>|<span data-ttu-id="9c760-177">ゲートウェイの IPv4 アドレス。</span><span class="sxs-lookup"><span data-stu-id="9c760-177">The IPv4 gateway address.</span></span> <span data-ttu-id="9c760-178">10.0.0.0 など</span><span class="sxs-lookup"><span data-stu-id="9c760-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="9c760-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="9c760-179">ipV4DHCPServer</span></span>|<span data-ttu-id="9c760-180">String</span><span class="sxs-lookup"><span data-stu-id="9c760-180">String</span></span>|<span data-ttu-id="9c760-181">アダプターの DHCP サーバーの IPv4 アドレスです。</span><span class="sxs-lookup"><span data-stu-id="9c760-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="9c760-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="9c760-182">ipV4DNSServerList</span></span>|<span data-ttu-id="9c760-183">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9c760-183">String collection</span></span>|<span data-ttu-id="9c760-184">アダプターに対して構成されている IPv4 DNS サーバーです。</span><span class="sxs-lookup"><span data-stu-id="9c760-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="9c760-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="9c760-185">dnsSuffixList</span></span>|<span data-ttu-id="9c760-186">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9c760-186">String collection</span></span>|<span data-ttu-id="9c760-187">現在のネットワークの有効な DNS サフィックスです。</span><span class="sxs-lookup"><span data-stu-id="9c760-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="9c760-188">例: seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="9c760-188">e.g. seattle.contoso.com</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c760-189">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9c760-189">Relationships</span></span>
|<span data-ttu-id="9c760-190">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9c760-190">Relationship</span></span>|<span data-ttu-id="9c760-191">型</span><span class="sxs-lookup"><span data-stu-id="9c760-191">Type</span></span>|<span data-ttu-id="9c760-192">説明</span><span class="sxs-lookup"><span data-stu-id="9c760-192">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c760-193">managementConditionStatements</span><span class="sxs-lookup"><span data-stu-id="9c760-193">managementConditionStatements</span></span>|<span data-ttu-id="9c760-194">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="9c760-194">[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) collection</span></span>|<span data-ttu-id="9c760-195">管理条件に関連付けられている管理の条件ステートメントです。</span><span class="sxs-lookup"><span data-stu-id="9c760-195">The management condition statements associated to the management condition.</span></span> <span data-ttu-id="9c760-196">[ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="9c760-196">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c760-197">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c760-197">JSON Representation</span></span>
<span data-ttu-id="9c760-198">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9c760-198">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv4ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "ipV4Prefix": "String",
  "ipV4Gateway": "String",
  "ipV4DHCPServer": "String",
  "ipV4DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```




