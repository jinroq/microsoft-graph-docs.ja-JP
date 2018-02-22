# <a name="windowsfirewallnetworkprofile-resource-type"></a><span data-ttu-id="92c68-101">windowsFirewallNetworkProfile リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="92c68-101">windowsFirewallNetworkProfile resource type</span></span>

> <span data-ttu-id="92c68-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="92c68-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="92c68-103">Windows ファイアウォールのプロファイルのポリシーです。</span><span class="sxs-lookup"><span data-stu-id="92c68-103">Windows Firewall Profile Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="92c68-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92c68-104">Properties</span></span>
|<span data-ttu-id="92c68-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92c68-105">Property</span></span>|<span data-ttu-id="92c68-106">型</span><span class="sxs-lookup"><span data-stu-id="92c68-106">Type</span></span>|<span data-ttu-id="92c68-107">説明</span><span class="sxs-lookup"><span data-stu-id="92c68-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92c68-108">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="92c68-108">firewallEnabled</span></span>|<span data-ttu-id="92c68-109">String</span><span class="sxs-lookup"><span data-stu-id="92c68-109">String</span></span>|<span data-ttu-id="92c68-110">ファイアウォールと高度なセキュリティの実行をオンにします。可能な値は、`notConfigured`、`blocked`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="92c68-110">Turn on the firewall and advanced security enforcement Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="92c68-111">stealthModeBlocked</span><span class="sxs-lookup"><span data-stu-id="92c68-111">stealthModeBlocked</span></span>|<span data-ttu-id="92c68-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-112">Boolean</span></span>|<span data-ttu-id="92c68-113">サーバーがステルス モードで動作するのを防ぎます</span><span class="sxs-lookup"><span data-stu-id="92c68-113">Prevent the server from operating in stealth mode</span></span>|
|<span data-ttu-id="92c68-114">incomingTrafficBlocked</span><span class="sxs-lookup"><span data-stu-id="92c68-114">incomingTrafficBlocked</span></span>|<span data-ttu-id="92c68-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-115">Boolean</span></span>|<span data-ttu-id="92c68-116">他のポリシーの設定に関係なく、すべての受信トラフィックをブロックするようにファイアウォールを構成します</span><span class="sxs-lookup"><span data-stu-id="92c68-116">Configures the firewall to block all incoming traffic regardless of other policy settings</span></span>|
|<span data-ttu-id="92c68-117">unicastResponsesToMulticastBroadcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="92c68-117">unicastResponsesToMulticastBroadcastsBlocked</span></span>|<span data-ttu-id="92c68-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-118">Boolean</span></span>|<span data-ttu-id="92c68-119">マルチキャスト ブロードキャスト トラフィックへのユニキャスト応答をブロックするようにファイアウォールを構成します</span><span class="sxs-lookup"><span data-stu-id="92c68-119">Configures the firewall to block unicast responses to multicast broadcast traffic</span></span>|
|<span data-ttu-id="92c68-120">inboundNotificationsBlocked</span><span class="sxs-lookup"><span data-stu-id="92c68-120">inboundNotificationsBlocked</span></span>|<span data-ttu-id="92c68-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-121">Boolean</span></span>|<span data-ttu-id="92c68-122">アプリケーションがポートでリッスンしないようにブロックされているときに、ファイアウォールによる通知を表示しないようにします</span><span class="sxs-lookup"><span data-stu-id="92c68-122">Prevents the firewall from displaying notifications when an application is blocked from listening on a port</span></span>|
|<span data-ttu-id="92c68-123">authorizedApplicationRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="92c68-123">authorizedApplicationRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="92c68-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-124">Boolean</span></span>|<span data-ttu-id="92c68-125">ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからの承認済みのアプリケーションに関する規則とローカル ストアからの規則を統合するように構成します</span><span class="sxs-lookup"><span data-stu-id="92c68-125">Configures the firewall to merge authorized application rules from group policy with those from local store instead of ignoring the local store rules</span></span>|
|<span data-ttu-id="92c68-126">globalPortRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="92c68-126">globalPortRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="92c68-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-127">Boolean</span></span>|<span data-ttu-id="92c68-128">ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからのグローバル ポートの規則と、ローカル ストアからの規則を統合するように構成します</span><span class="sxs-lookup"><span data-stu-id="92c68-128">Configures the firewall to merge global port rules from group policy with those from local store instead of ignoring the local store rules</span></span>|
|<span data-ttu-id="92c68-129">connectionSecurityRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="92c68-129">connectionSecurityRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="92c68-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-130">Boolean</span></span>|<span data-ttu-id="92c68-131">ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからの接続セキュリティの規則と、ローカル ストアからの規則を統合するように構成します</span><span class="sxs-lookup"><span data-stu-id="92c68-131">Configures the firewall to merge connection security rules from group policy with those from local store instead of ignoring the local store rules</span></span>|
|<span data-ttu-id="92c68-132">outboundConnectionsBlocked</span><span class="sxs-lookup"><span data-stu-id="92c68-132">outboundConnectionsBlocked</span></span>|<span data-ttu-id="92c68-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-133">Boolean</span></span>|<span data-ttu-id="92c68-134">既定で、ファイアウォールがすべての送信接続をブロックするように構成します</span><span class="sxs-lookup"><span data-stu-id="92c68-134">Configures the firewall to block all outgoing connections by default</span></span>|
|<span data-ttu-id="92c68-135">inboundConnectionsBlocked</span><span class="sxs-lookup"><span data-stu-id="92c68-135">inboundConnectionsBlocked</span></span>|<span data-ttu-id="92c68-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-136">Boolean</span></span>|<span data-ttu-id="92c68-137">既定で、ファイアウォールがすべての受信接続をブロックするように構成します</span><span class="sxs-lookup"><span data-stu-id="92c68-137">Configures the firewall to block all incoming connections by default</span></span>|
|<span data-ttu-id="92c68-138">securedPacketExemptionAllowed</span><span class="sxs-lookup"><span data-stu-id="92c68-138">securedPacketExemptionAllowed</span></span>|<span data-ttu-id="92c68-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-139">Boolean</span></span>|<span data-ttu-id="92c68-140">stealthModeBlocked が true に設定されている場合でも、ホスト コンピューターが要請していないネットワーク トラフィックに応答し、トラフィックが IPSec によって保護されるように、ファイアウォールを構成します</span><span class="sxs-lookup"><span data-stu-id="92c68-140">Configures the firewall to allow the host computer to respond to unsolicited network traffic of that traffic is secured by IPSec even when stealthModeBlocked is set to true</span></span>|
|<span data-ttu-id="92c68-141">policyRulesFromGroupPolicyMerged</span><span class="sxs-lookup"><span data-stu-id="92c68-141">policyRulesFromGroupPolicyMerged</span></span>|<span data-ttu-id="92c68-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="92c68-142">Boolean</span></span>|<span data-ttu-id="92c68-143">ファイアウォールが、ローカル ストアの規則を無視することなく、グループ ポリシーからのファイアウォール規則のポリシーと、ローカル ストアからのポリシーを統合するように構成します</span><span class="sxs-lookup"><span data-stu-id="92c68-143">Configures the firewall to merge Firewall Rule policies from group policy with those from local store instead of ignoring the local store rules</span></span>|

## <a name="relationships"></a><span data-ttu-id="92c68-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92c68-144">Relationships</span></span>
<span data-ttu-id="92c68-145">なし</span><span class="sxs-lookup"><span data-stu-id="92c68-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="92c68-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92c68-146">JSON Representation</span></span>
<span data-ttu-id="92c68-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92c68-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallNetworkProfile",
  "firewallEnabled": "String",
  "stealthModeBlocked": true,
  "incomingTrafficBlocked": true,
  "unicastResponsesToMulticastBroadcastsBlocked": true,
  "inboundNotificationsBlocked": true,
  "authorizedApplicationRulesFromGroupPolicyMerged": true,
  "globalPortRulesFromGroupPolicyMerged": true,
  "connectionSecurityRulesFromGroupPolicyMerged": true,
  "outboundConnectionsBlocked": true,
  "inboundConnectionsBlocked": true,
  "securedPacketExemptionAllowed": true,
  "policyRulesFromGroupPolicyMerged": true
}
```



