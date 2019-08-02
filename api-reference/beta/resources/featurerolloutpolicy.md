---
title: featureRolloutPolicy リソースの種類
description: ディレクトリオブジェクトに関連付けられている機能ロールアウトポリシーを表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50d54ae046ef5a0283f5eb2e474fd0faab781687
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062164"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="b784b-103">featureRolloutPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b784b-103">featureRolloutPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b784b-104">ディレクトリオブジェクトに関連付けられている機能ロールアウトポリシーを表します。</span><span class="sxs-lookup"><span data-stu-id="b784b-104">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="b784b-105">機能ロールアウトポリシーを作成すると、テナント管理者は、組織全体に対して機能を有効にする前に、特定のグループを使用して Azure AD の機能を試験的に実行できます。</span><span class="sxs-lookup"><span data-stu-id="b784b-105">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="b784b-106">これにより、影響が最小限に抑えられ、管理者が認証関連機能を徐々にテストおよびロールアウトできるようになります。</span><span class="sxs-lookup"><span data-stu-id="b784b-106">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="b784b-107">機能のロールアウトには、次の制限があります。</span><span class="sxs-lookup"><span data-stu-id="b784b-107">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="b784b-108">各機能では、最大10個のグループがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="b784b-108">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="b784b-109">**AppliesTo**フィールドは、グループのみをサポートします。</span><span class="sxs-lookup"><span data-stu-id="b784b-109">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="b784b-110">動的グループとネストされたグループはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b784b-110">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="b784b-111">このロールアウトポリシーを使用して、現在 suported に展開されている各機能の前提条件は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="b784b-111">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="b784b-112">パススルー認証</span><span class="sxs-lookup"><span data-stu-id="b784b-112">Passthrough Authentication</span></span>

* <span data-ttu-id="b784b-113">[認証](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta)エージェントを実行する Windows Server 2012 R2 以降を実行しているサーバーを特定します。</span><span class="sxs-lookup"><span data-stu-id="b784b-113">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="b784b-114">サーバーがドメインに参加しており、Active Directory を使用して選択したユーザーを認証できること、および送信ポート/Url で Azure AD と通信できることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b784b-114"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="b784b-115">サーバーに Microsoft Azure AD Connect 認証エージェントを[ダウンロード](https://aka.ms/getauthagent)& インストールします。</span><span class="sxs-lookup"><span data-stu-id="b784b-115">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="b784b-116">高可用性を有効にするには、[ここ](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)に記載されているように、他のサーバーに追加の認証エージェントをインストールします。</span><span class="sxs-lookup"><span data-stu-id="b784b-116">To enable high availability, install additional Authentication Agents on other servers as described [here](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="b784b-117">[スマートロックアウト](https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-password-smart-lockout)設定が適切に構成されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b784b-117">Ensure that you have configured your [Smart Lockout](https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="b784b-118">これは、ユーザーのオンプレミスの Active Directory アカウントが不正な俳優によってロックアウトされないようにするためです。</span><span class="sxs-lookup"><span data-stu-id="b784b-118">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="b784b-119">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="b784b-119">SeamlessSso</span></span>

* <span data-ttu-id="b784b-120">[次](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)の手順に従って、AD フォレストの[SeamlessSso](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-sso)を有効にします。</span><span class="sxs-lookup"><span data-stu-id="b784b-120">Enable [SeamlessSso](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="b784b-121">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="b784b-121">PasswordHashSync</span></span>

* <span data-ttu-id="b784b-122">Azure AD Connect の [オプション機能] ページで [PasswordHashSync](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-phs) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="b784b-122">Enable [PasswordHashSync](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

## <a name="methods"></a><span data-ttu-id="b784b-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="b784b-123">Methods</span></span>

| <span data-ttu-id="b784b-124">メソッド</span><span class="sxs-lookup"><span data-stu-id="b784b-124">Method</span></span>       | <span data-ttu-id="b784b-125">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b784b-125">Return Type</span></span> | <span data-ttu-id="b784b-126">説明</span><span class="sxs-lookup"><span data-stu-id="b784b-126">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b784b-127">リスト featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="b784b-127">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="b784b-128">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="b784b-128">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="b784b-129">FeatureRolloutPolicy オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="b784b-129">Retrieve a list of featureRolloutPolicy objects.</span></span> |
| [<span data-ttu-id="b784b-130">FeatureRolloutPolicy を取得する</span><span class="sxs-lookup"><span data-stu-id="b784b-130">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="b784b-131">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="b784b-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="b784b-132">Featurerolloutpolicy オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="b784b-132">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> ||
| [<span data-ttu-id="b784b-133">FeatureRolloutPolicy を作成する</span><span class="sxs-lookup"><span data-stu-id="b784b-133">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="b784b-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="b784b-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="b784b-135">新しい featureRolloutPolicy オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b784b-135">Create a new featureRolloutPolicy object.</span></span>
| [<span data-ttu-id="b784b-136">FeatureRolloutPolicy の更新</span><span class="sxs-lookup"><span data-stu-id="b784b-136">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="b784b-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="b784b-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="b784b-138">Featurerolloutpolicy オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b784b-138">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="b784b-139">FeatureRolloutPolicy の削除</span><span class="sxs-lookup"><span data-stu-id="b784b-139">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="b784b-140">None</span><span class="sxs-lookup"><span data-stu-id="b784b-140">None</span></span> | <span data-ttu-id="b784b-141">FeatureRolloutPolicy オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="b784b-141">Delete a featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="b784b-142">AppliesTo を割り当てる</span><span class="sxs-lookup"><span data-stu-id="b784b-142">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md) | [<span data-ttu-id="b784b-143">directoryObject</span><span class="sxs-lookup"><span data-stu-id="b784b-143">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="b784b-144">機能のロールアウトに directoryObject を割り当てます。</span><span class="sxs-lookup"><span data-stu-id="b784b-144">Assign a directoryObject to feature rollout.</span></span> |
| [<span data-ttu-id="b784b-145">AppliesTo の削除</span><span class="sxs-lookup"><span data-stu-id="b784b-145">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md) | <span data-ttu-id="b784b-146">None</span><span class="sxs-lookup"><span data-stu-id="b784b-146">None</span></span> | <span data-ttu-id="b784b-147">機能ロールアウトから directoryObject を削除します。</span><span class="sxs-lookup"><span data-stu-id="b784b-147">Remove a directoryObject from feature rollout.</span></span> |

## <a name="properties"></a><span data-ttu-id="b784b-148">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b784b-148">Properties</span></span>

| <span data-ttu-id="b784b-149">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b784b-149">Property</span></span>     | <span data-ttu-id="b784b-150">型</span><span class="sxs-lookup"><span data-stu-id="b784b-150">Type</span></span>        | <span data-ttu-id="b784b-151">説明</span><span class="sxs-lookup"><span data-stu-id="b784b-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b784b-152">description</span><span class="sxs-lookup"><span data-stu-id="b784b-152">description</span></span>|<span data-ttu-id="b784b-153">String</span><span class="sxs-lookup"><span data-stu-id="b784b-153">String</span></span>|<span data-ttu-id="b784b-154">この機能ロールアウトポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="b784b-154">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="b784b-155">displayName</span><span class="sxs-lookup"><span data-stu-id="b784b-155">displayName</span></span>|<span data-ttu-id="b784b-156">String</span><span class="sxs-lookup"><span data-stu-id="b784b-156">String</span></span>|<span data-ttu-id="b784b-157">この機能ロールアウトポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="b784b-157">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="b784b-158">特徴</span><span class="sxs-lookup"><span data-stu-id="b784b-158">feature</span></span>|<span data-ttu-id="b784b-159">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="b784b-159">stagedFeatureName</span></span>| <span data-ttu-id="b784b-160">使用可能な値は、`passthroughAuthentication`、`seamlessSso`、`passwordHashSync`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="b784b-160">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="b784b-161">id</span><span class="sxs-lookup"><span data-stu-id="b784b-161">id</span></span>|<span data-ttu-id="b784b-162">String</span><span class="sxs-lookup"><span data-stu-id="b784b-162">String</span></span>| <span data-ttu-id="b784b-163">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b784b-163">Read-only.</span></span>|
|<span data-ttu-id="b784b-164">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="b784b-164">isAppliedToOrganization</span></span>|<span data-ttu-id="b784b-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="b784b-165">Boolean</span></span>|<span data-ttu-id="b784b-166">この機能ロールアウトポリシーを組織全体に適用する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b784b-166">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="b784b-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b784b-167">isEnabled</span></span>|<span data-ttu-id="b784b-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="b784b-168">Boolean</span></span>|<span data-ttu-id="b784b-169">機能ロールアウトが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b784b-169">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b784b-170">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b784b-170">Relationships</span></span>

| <span data-ttu-id="b784b-171">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b784b-171">Relationship</span></span> | <span data-ttu-id="b784b-172">型</span><span class="sxs-lookup"><span data-stu-id="b784b-172">Type</span></span>        | <span data-ttu-id="b784b-173">説明</span><span class="sxs-lookup"><span data-stu-id="b784b-173">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b784b-174">appliesTo</span><span class="sxs-lookup"><span data-stu-id="b784b-174">appliesTo</span></span>|<span data-ttu-id="b784b-175">[directoryObject](directoryobject.md) collection</span><span class="sxs-lookup"><span data-stu-id="b784b-175">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="b784b-176">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="b784b-176">Nullable.</span></span> <span data-ttu-id="b784b-177">機能が有効になっている directoryObjects のリストを指定します。</span><span class="sxs-lookup"><span data-stu-id="b784b-177">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b784b-178">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b784b-178">JSON representation</span></span>

<span data-ttu-id="b784b-179">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b784b-179">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "feature": "string",
  "id": "String (identifier)",
  "isAppliedToOrganization": false,
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "featureRolloutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
