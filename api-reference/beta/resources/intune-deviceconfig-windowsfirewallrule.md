---
title: windowsFirewallRule リソースの種類
description: Windows ファイアウォールを介したトラフィックを制御するルール。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae5c51a2ce5b3f86f03e651162611e8d219e7da2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737665"
---
# <a name="windowsfirewallrule-resource-type"></a><span data-ttu-id="b8255-103">windowsFirewallRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8255-103">windowsFirewallRule resource type</span></span>

> <span data-ttu-id="b8255-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8255-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8255-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8255-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8255-106">Windows ファイアウォールを介したトラフィックを制御するルール。</span><span class="sxs-lookup"><span data-stu-id="b8255-106">A rule controlling traffic through the Windows Firewall.</span></span>

## <a name="properties"></a><span data-ttu-id="b8255-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8255-107">Properties</span></span>
|<span data-ttu-id="b8255-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8255-108">Property</span></span>|<span data-ttu-id="b8255-109">型</span><span class="sxs-lookup"><span data-stu-id="b8255-109">Type</span></span>|<span data-ttu-id="b8255-110">説明</span><span class="sxs-lookup"><span data-stu-id="b8255-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8255-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b8255-111">displayName</span></span>|<span data-ttu-id="b8255-112">String</span><span class="sxs-lookup"><span data-stu-id="b8255-112">String</span></span>|<span data-ttu-id="b8255-113">ルールの表示名。</span><span class="sxs-lookup"><span data-stu-id="b8255-113">The display name of the rule.</span></span> <span data-ttu-id="b8255-114">一意である必要はありません。</span><span class="sxs-lookup"><span data-stu-id="b8255-114">Does not need to be unique.</span></span>|
|<span data-ttu-id="b8255-115">description</span><span class="sxs-lookup"><span data-stu-id="b8255-115">description</span></span>|<span data-ttu-id="b8255-116">String</span><span class="sxs-lookup"><span data-stu-id="b8255-116">String</span></span>|<span data-ttu-id="b8255-117">ルールの説明。</span><span class="sxs-lookup"><span data-stu-id="b8255-117">The description of the rule.</span></span>|
|<span data-ttu-id="b8255-118">パッケージ Efamilyname</span><span class="sxs-lookup"><span data-stu-id="b8255-118">packageFamilyName</span></span>|<span data-ttu-id="b8255-119">String</span><span class="sxs-lookup"><span data-stu-id="b8255-119">String</span></span>|<span data-ttu-id="b8255-120">ファイアウォールルールの影響を受ける Microsoft Store アプリケーションのパッケージファミリー名。</span><span class="sxs-lookup"><span data-stu-id="b8255-120">The package family name of a Microsoft Store application that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="b8255-121">パス</span><span class="sxs-lookup"><span data-stu-id="b8255-121">filePath</span></span>|<span data-ttu-id="b8255-122">String</span><span class="sxs-lookup"><span data-stu-id="b8255-122">String</span></span>|<span data-ttu-id="b8255-123">ファイアウォールルールの影響を受けるアプリの完全なファイルパス。</span><span class="sxs-lookup"><span data-stu-id="b8255-123">The full file path of an app that's affected by the firewall rule.</span></span>|
|<span data-ttu-id="b8255-124">serviceName</span><span class="sxs-lookup"><span data-stu-id="b8255-124">serviceName</span></span>|<span data-ttu-id="b8255-125">String</span><span class="sxs-lookup"><span data-stu-id="b8255-125">String</span></span>|<span data-ttu-id="b8255-126">アプリケーションではなく、サービスがトラフィックを送受信している場合に使用される名前。</span><span class="sxs-lookup"><span data-stu-id="b8255-126">The name used in cases when a service, not an application, is sending or receiving traffic.</span></span>|
|<span data-ttu-id="b8255-127">プロトコール</span><span class="sxs-lookup"><span data-stu-id="b8255-127">protocol</span></span>|<span data-ttu-id="b8255-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b8255-128">Int32</span></span>|<span data-ttu-id="b8255-129">0-255 IP プロトコルを表す番号 (TCP = 6、UDP = 17)。</span><span class="sxs-lookup"><span data-stu-id="b8255-129">0-255 number representing the IP protocol (TCP = 6, UDP = 17).</span></span> <span data-ttu-id="b8255-130">指定しない場合、既定値は All です。</span><span class="sxs-lookup"><span data-stu-id="b8255-130">If not specified, the default is All.</span></span> <span data-ttu-id="b8255-131">有効な値は 0 ~ 255</span><span class="sxs-lookup"><span data-stu-id="b8255-131">Valid values 0 to 255</span></span>|
|<span data-ttu-id="b8255-132">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="b8255-132">localPortRanges</span></span>|<span data-ttu-id="b8255-133">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b8255-133">String collection</span></span>|<span data-ttu-id="b8255-134">ローカルポート範囲のリスト。</span><span class="sxs-lookup"><span data-stu-id="b8255-134">List of local port ranges.</span></span> <span data-ttu-id="b8255-135">たとえば、"100-120"、"200"、"300-320" などです。</span><span class="sxs-lookup"><span data-stu-id="b8255-135">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="b8255-136">指定しない場合、既定値は All です。</span><span class="sxs-lookup"><span data-stu-id="b8255-136">If not specified, the default is All.</span></span>|
|<span data-ttu-id="b8255-137">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="b8255-137">remotePortRanges</span></span>|<span data-ttu-id="b8255-138">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b8255-138">String collection</span></span>|<span data-ttu-id="b8255-139">リモートポート範囲の一覧。</span><span class="sxs-lookup"><span data-stu-id="b8255-139">List of remote port ranges.</span></span> <span data-ttu-id="b8255-140">たとえば、"100-120"、"200"、"300-320" などです。</span><span class="sxs-lookup"><span data-stu-id="b8255-140">For example, "100-120", "200", "300-320".</span></span> <span data-ttu-id="b8255-141">指定しない場合、既定値は All です。</span><span class="sxs-lookup"><span data-stu-id="b8255-141">If not specified, the default is All.</span></span>|
|<span data-ttu-id="b8255-142">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="b8255-142">localAddressRanges</span></span>|<span data-ttu-id="b8255-143">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b8255-143">String collection</span></span>|<span data-ttu-id="b8255-144">ルールでカバーされているローカルアドレスのリスト。</span><span class="sxs-lookup"><span data-stu-id="b8255-144">List of local addresses covered by the rule.</span></span> <span data-ttu-id="b8255-145">有効なトークンは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b8255-145">Valid tokens include:</span></span>
- <span data-ttu-id="b8255-146">"\*" はローカルアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="b8255-146">"\*" indicates any local address.</span></span> <span data-ttu-id="b8255-147">指定する場合は、このトークンのみが含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8255-147">If present, this must be the only token included.</span></span>
- <span data-ttu-id="b8255-148">サブネットは、サブネットマスクまたはネットワークプレフィックス表記のどちらかを使用して指定できます。</span><span class="sxs-lookup"><span data-stu-id="b8255-148">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="b8255-149">サブネットマスクもネットワークプレフィックスも指定されていない場合、サブネットマスクは既定で255.255.255.255 になります。</span><span class="sxs-lookup"><span data-stu-id="b8255-149">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="b8255-150">有効な IPv6 アドレス。</span><span class="sxs-lookup"><span data-stu-id="b8255-150">A valid IPv6 address.</span></span>
- <span data-ttu-id="b8255-151">スペースを含まない「開始アドレスと終了アドレス」の形式の IPv4 アドレス範囲。</span><span class="sxs-lookup"><span data-stu-id="b8255-151">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="b8255-152">「開始アドレス-終了アドレス」の形式の IPv6 アドレス範囲。スペースは含まれません。</span><span class="sxs-lookup"><span data-stu-id="b8255-152">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="b8255-153">既定は任意のアドレスです。 || remoteAddressRanges |文字列コレクション |ルールの対象となるリモートアドレスを指定するトークンの一覧です。</span><span class="sxs-lookup"><span data-stu-id="b8255-153">Default is any address.| |remoteAddressRanges|String collection|List of tokens specifying the remote addresses covered by the rule.</span></span> <span data-ttu-id="b8255-154">トークンの大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="b8255-154">Tokens are case insensitive.</span></span> <span data-ttu-id="b8255-155">有効なトークンは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b8255-155">Valid tokens include:</span></span>
- <span data-ttu-id="b8255-156">"\*" は任意のリモートアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="b8255-156">"\*" indicates any remote address.</span></span> <span data-ttu-id="b8255-157">指定する場合は、このトークンのみが含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8255-157">If present, this must be the only token included.</span></span>
- <span data-ttu-id="b8255-158">"Defaultgateway"</span><span class="sxs-lookup"><span data-stu-id="b8255-158">"Defaultgateway"</span></span>
- <span data-ttu-id="b8255-159">DHCP</span><span class="sxs-lookup"><span data-stu-id="b8255-159">"DHCP"</span></span>
- <span data-ttu-id="b8255-160">DSN</span><span class="sxs-lookup"><span data-stu-id="b8255-160">"DNS"</span></span>
- <span data-ttu-id="b8255-161">獲得</span><span class="sxs-lookup"><span data-stu-id="b8255-161">"WINS"</span></span>
- <span data-ttu-id="b8255-162">"Intranet" (Windows バージョンでサポートされている 1809 +)</span><span class="sxs-lookup"><span data-stu-id="b8255-162">"Intranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="b8255-163">"RmtIntranet" (Windows バージョンでサポートされている 1809 +)</span><span class="sxs-lookup"><span data-stu-id="b8255-163">"RmtIntranet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="b8255-164">"Internet" (Windows バージョンでサポートされている 1809 +)</span><span class="sxs-lookup"><span data-stu-id="b8255-164">"Internet" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="b8255-165">"Ply2Renders" (Windows バージョン1809以降でサポートされています)</span><span class="sxs-lookup"><span data-stu-id="b8255-165">"Ply2Renders" (supported on Windows versions 1809+)</span></span>
- <span data-ttu-id="b8255-166">"LocalSubnet" は、ローカルサブネット上のローカルアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="b8255-166">"LocalSubnet" indicates any local address on the local subnet.</span></span>
- <span data-ttu-id="b8255-167">サブネットは、サブネットマスクまたはネットワークプレフィックス表記のどちらかを使用して指定できます。</span><span class="sxs-lookup"><span data-stu-id="b8255-167">A subnet can be specified using either the subnet mask or network prefix notation.</span></span> <span data-ttu-id="b8255-168">サブネットマスクもネットワークプレフィックスも指定されていない場合、サブネットマスクは既定で255.255.255.255 になります。</span><span class="sxs-lookup"><span data-stu-id="b8255-168">If neither a subnet mask nor a network prefix is specified, the subnet mask defaults to 255.255.255.255.</span></span>
- <span data-ttu-id="b8255-169">有効な IPv6 アドレス。</span><span class="sxs-lookup"><span data-stu-id="b8255-169">A valid IPv6 address.</span></span>
- <span data-ttu-id="b8255-170">スペースを含まない「開始アドレスと終了アドレス」の形式の IPv4 アドレス範囲。</span><span class="sxs-lookup"><span data-stu-id="b8255-170">An IPv4 address range in the format of "start address - end address" with no spaces included.</span></span>
- <span data-ttu-id="b8255-171">「開始アドレス-終了アドレス」の形式の IPv6 アドレス範囲。スペースは含まれません。</span><span class="sxs-lookup"><span data-stu-id="b8255-171">An IPv6 address range in the format of "start address - end address" with no spaces included.</span></span>
<span data-ttu-id="b8255-172">既定は任意のアドレスです。 || profileTypes |[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|ルールが属するプロファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="b8255-172">Default is any address.| |profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Specifies the profiles to which the rule belongs.</span></span> <span data-ttu-id="b8255-173">指定しない場合、既定値は All です。</span><span class="sxs-lookup"><span data-stu-id="b8255-173">If not specified, the default is All.</span></span> <span data-ttu-id="b8255-174">可能な値: `notConfigured`、 `domain`、 `private`、 `public`。 || action |[Statemanagementsetting](../resources/intune-deviceconfig-statemanagementsetting.md)|ルールによって適用されるアクション。</span><span class="sxs-lookup"><span data-stu-id="b8255-174">Possible values are: `notConfigured`, `domain`, `private`, `public`.| |action|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|The action the rule enforces.</span></span> <span data-ttu-id="b8255-175">指定しない場合、既定値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b8255-175">If not specified, the default is Allowed.</span></span> <span data-ttu-id="b8255-176">可能な値: `notConfigured`、 `blocked`、 `allowed`. || trafficDirection |[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|ルールが有効になっているトラフィックの方向。</span><span class="sxs-lookup"><span data-stu-id="b8255-176">Possible values are: `notConfigured`, `blocked`, `allowed`.| |trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|The traffic direction that the rule is enabled for.</span></span> <span data-ttu-id="b8255-177">指定しない場合、既定値は "Out" です。可能な値: `notConfigured`、 `out`、 `in`. || interfaceTypes |[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|ルールのインターフェイスの種類。</span><span class="sxs-lookup"><span data-stu-id="b8255-177">If not specified, the default is Out. Possible values are: `notConfigured`, `out`, `in`.| |interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|The interface types of the rule.</span></span> <span data-ttu-id="b8255-178">可能な値: `notConfigured`、 `remoteAccess`、 `wireless`、 `lan`。 || edgeTraversal |[Statemanagementsetting](../resources/intune-deviceconfig-statemanagementsetting.md)|このルールに対してエッジトラバーサルを有効にするか無効にするかを示します。</span><span class="sxs-lookup"><span data-stu-id="b8255-178">Possible values are: `notConfigured`, `remoteAccess`, `wireless`, `lan`.| |edgeTraversal|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Indicates whether edge traversal is enabled or disabled for this rule.</span></span>
<span data-ttu-id="b8255-179">EdgeTraversal の設定は、特定の受信トラフィックで、Teredo トンネリングテクノロジを使用して Nat およびその他のエッジデバイスをトンネリングできることを示します。</span><span class="sxs-lookup"><span data-stu-id="b8255-179">The EdgeTraversal setting indicates that specific inbound traffic is allowed to tunnel through NATs and other edge devices using the Teredo tunneling technology.</span></span> <span data-ttu-id="b8255-180">この設定を正しく動作させるには、受信ファイアウォールルールを持つアプリケーションまたはサービスが IPv6 をサポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8255-180">In order for this setting to work correctly, the application or service with the inbound firewall rule needs to support IPv6.</span></span> <span data-ttu-id="b8255-181">この設定の主なアプリケーションにより、ホスト上のリスナーは Teredo IPv6 アドレスを使用してグローバルにアドレス可能にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b8255-181">The primary application of this setting allows listeners on the host to be globally addressable through a Teredo IPv6 address.</span></span>
<span data-ttu-id="b8255-182">新しいルールでは、EdgeTraversal プロパティは既定で無効になっています。</span><span class="sxs-lookup"><span data-stu-id="b8255-182">New rules have the EdgeTraversal property disabled by default.</span></span> <span data-ttu-id="b8255-183">可能な値: `notConfigured`、 `blocked`、 `allowed`. || localUserAuthorizations |文字列 |アプリコンテナーに対して承認されたローカルユーザーのリストを指定します。</span><span class="sxs-lookup"><span data-stu-id="b8255-183">Possible values are: `notConfigured`, `blocked`, `allowed`.| |localUserAuthorizations|String|Specifies the list of authorized local users for the app container.</span></span> <span data-ttu-id="b8255-184">これは、セキュリティ記述子定義言語 (SDDL) 形式の文字列です。 |</span><span class="sxs-lookup"><span data-stu-id="b8255-184">This is a string in Security Descriptor Definition Language (SDDL) format.|</span></span>

## <a name="relationships"></a><span data-ttu-id="b8255-185">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8255-185">Relationships</span></span>
<span data-ttu-id="b8255-186">なし</span><span class="sxs-lookup"><span data-stu-id="b8255-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8255-187">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8255-187">JSON Representation</span></span>
<span data-ttu-id="b8255-188">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8255-188">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "edgeTraversal": "String",
  "localUserAuthorizations": "String"
}
```





