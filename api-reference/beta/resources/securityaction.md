---
title: securityAction リソースの種類
description: Microsoft Graph Security securityAction エンティティを使用して脅威から防御するために、直ちにアクションを実行します。 セキュリティアナリストが、悪意のあるファイル、URL、ドメイン、または IP アドレスなどの新しい指標を見つけた場合、保護を Microsoft セキュリティソリューションですぐに有効にすることができます。 特定のプロバイダーに対してアクションを起動し、実行されたすべてのアクションを表示し、必要に応じて操作をキャンセルします。 windows Defender ATP (近日中) と共にセキュリティアクションを試行して、警告で表示されたプロパティまたは調査中に識別されたプロパティを使用して、windows エンドポイント上の悪意のあるアクティビティをブロックします。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 405f12c2cf484651f8bcefc791c9dd24dae410bd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366988"
---
# <a name="securityaction-resource-type"></a><span data-ttu-id="f661f-106">securityAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f661f-106">securityAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f661f-107">Microsoft Graph Security securityAction エンティティを使用して脅威から防御するために、直ちにアクションを実行します。</span><span class="sxs-lookup"><span data-stu-id="f661f-107">Take immediate action to defend against threats using the Microsoft Graph Security securityAction entity.</span></span> <span data-ttu-id="f661f-108">セキュリティアナリストが、悪意のあるファイル、URL、ドメイン、または IP アドレスなどの新しい指標を見つけた場合、保護を Microsoft セキュリティソリューションですぐに有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f661f-108">When a security analyst discovers a new indicator, such as a malicious file, URL, domain, or IP address, protection can be instantly enabled in your Microsoft security solutions.</span></span> <span data-ttu-id="f661f-109">特定のプロバイダーに対してアクションを起動し、実行されたすべてのアクションを表示し、必要に応じて操作をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="f661f-109">Invoke an action for a specific provider, see all actions taken, and cancel an action if needed.</span></span> <span data-ttu-id="f661f-110">[windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) (近日中) と共にセキュリティアクションを試行して、警告で表示されたプロパティまたは調査中に識別されたプロパティを使用して、windows エンドポイント上の悪意のあるアクティビティをブロックします。</span><span class="sxs-lookup"><span data-stu-id="f661f-110">Try security actions with [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) (coming soon) to block malicious activity on your Windows endpoints using properties seen in alerts or identified during investigations.</span></span>

## <a name="methods"></a><span data-ttu-id="f661f-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="f661f-111">Methods</span></span>

| <span data-ttu-id="f661f-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="f661f-112">Method</span></span>       | <span data-ttu-id="f661f-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f661f-113">Return Type</span></span> | <span data-ttu-id="f661f-114">説明</span><span class="sxs-lookup"><span data-stu-id="f661f-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f661f-115">securityAction を取得する</span><span class="sxs-lookup"><span data-stu-id="f661f-115">Get securityAction</span></span>](../api/securityaction-get.md) | [<span data-ttu-id="f661f-116">securityAction</span><span class="sxs-lookup"><span data-stu-id="f661f-116">securityAction</span></span>](securityaction.md) | <span data-ttu-id="f661f-117">securityAction オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f661f-117">Read properties and relationships of securityAction object.</span></span> |
| [<span data-ttu-id="f661f-118">securityAction を作成する</span><span class="sxs-lookup"><span data-stu-id="f661f-118">Create securityAction</span></span>](../api/securityactions-post.md) | [<span data-ttu-id="f661f-119">securityAction</span><span class="sxs-lookup"><span data-stu-id="f661f-119">securityAction</span></span>](securityaction.md) | <span data-ttu-id="f661f-120">securityactions コレクションへの投稿によって新しい securityAction を作成します。</span><span class="sxs-lookup"><span data-stu-id="f661f-120">Create a new securityAction by posting to the securityActions collection.</span></span> |
| [<span data-ttu-id="f661f-121">セキュリティアクションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f661f-121">List securityActions</span></span>](../api/securityactions-list.md) | <span data-ttu-id="f661f-122">[securityAction](securityaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f661f-122">[securityAction](securityaction.md) collection</span></span> | <span data-ttu-id="f661f-123">securityAction オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="f661f-123">Get a securityAction object collection.</span></span> |
|[<span data-ttu-id="f661f-124">securityAction のキャンセル</span><span class="sxs-lookup"><span data-stu-id="f661f-124">Cancel securityAction</span></span>](../api/securityaction-cancelsecurityaction.md)|<span data-ttu-id="f661f-125">なし</span><span class="sxs-lookup"><span data-stu-id="f661f-125">None</span></span>|<span data-ttu-id="f661f-126">セキュリティ操作をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="f661f-126">Cancel a security operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="f661f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f661f-127">Properties</span></span>

| <span data-ttu-id="f661f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f661f-128">Property</span></span>     | <span data-ttu-id="f661f-129">型</span><span class="sxs-lookup"><span data-stu-id="f661f-129">Type</span></span>        | <span data-ttu-id="f661f-130">説明</span><span class="sxs-lookup"><span data-stu-id="f661f-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f661f-131">actionreason</span><span class="sxs-lookup"><span data-stu-id="f661f-131">actionReason</span></span>|<span data-ttu-id="f661f-132">String</span><span class="sxs-lookup"><span data-stu-id="f661f-132">String</span></span>|<span data-ttu-id="f661f-133">このアクションを起動する理由。</span><span class="sxs-lookup"><span data-stu-id="f661f-133">Reason for invoking this action.</span></span>|
|<span data-ttu-id="f661f-134">appId</span><span class="sxs-lookup"><span data-stu-id="f661f-134">appId</span></span>|<span data-ttu-id="f661f-135">String</span><span class="sxs-lookup"><span data-stu-id="f661f-135">String</span></span>|<span data-ttu-id="f661f-136">アクションを送信 (POST) した、呼び出し元アプリケーションのアプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="f661f-136">The Application ID of the calling application that submitted (POST) the action.</span></span> <span data-ttu-id="f661f-137">appId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。</span><span class="sxs-lookup"><span data-stu-id="f661f-137">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="f661f-138">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="f661f-138">azureTenantId</span></span>|<span data-ttu-id="f661f-139">String</span><span class="sxs-lookup"><span data-stu-id="f661f-139">String</span></span>|<span data-ttu-id="f661f-140">エンティティが属しているテナントを判断するエンティティの Azure テナント ID (マルチテナントのサポート)。</span><span class="sxs-lookup"><span data-stu-id="f661f-140">Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).</span></span> <span data-ttu-id="f661f-141">azureTenantId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。</span><span class="sxs-lookup"><span data-stu-id="f661f-141">The azureTenantId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="f661f-142">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="f661f-142">completedDateTime</span></span>|<span data-ttu-id="f661f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f661f-143">DateTimeOffset</span></span>|<span data-ttu-id="f661f-144">アクションが完了したときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="f661f-144">Timestamp when the action was completed.</span></span> <span data-ttu-id="f661f-145">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f661f-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f661f-146">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f661f-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f661f-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f661f-147">createdDateTime</span></span>|<span data-ttu-id="f661f-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f661f-148">DateTimeOffset</span></span>|<span data-ttu-id="f661f-149">アクションが作成されたときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="f661f-149">Timestamp when the action is created.</span></span> <span data-ttu-id="f661f-150">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f661f-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f661f-151">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f661f-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f661f-152">errorInfo</span><span class="sxs-lookup"><span data-stu-id="f661f-152">errorInfo</span></span>|[<span data-ttu-id="f661f-153">resultInfo</span><span class="sxs-lookup"><span data-stu-id="f661f-153">resultInfo</span></span>](resultinfo.md)| <span data-ttu-id="f661f-154">アクションが失敗した場合のエラー情報。</span><span class="sxs-lookup"><span data-stu-id="f661f-154">Error info when the action fails.</span></span>|
|<span data-ttu-id="f661f-155">id</span><span class="sxs-lookup"><span data-stu-id="f661f-155">id</span></span>|<span data-ttu-id="f661f-156">String</span><span class="sxs-lookup"><span data-stu-id="f661f-156">String</span></span>| <span data-ttu-id="f661f-157">アクションが取り込まれたの場合に、システムによって作成されます。</span><span class="sxs-lookup"><span data-stu-id="f661f-157">Created by the system when the action is ingested.</span></span> <span data-ttu-id="f661f-158">生成された GUID/一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="f661f-158">Generated GUID/unique identifier.</span></span> <span data-ttu-id="f661f-159">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f661f-159">Read-only.</span></span>|
|<span data-ttu-id="f661f-160">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="f661f-160">lastActionDateTime</span></span>|<span data-ttu-id="f661f-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f661f-161">DateTimeOffset</span></span>| <span data-ttu-id="f661f-162">このアクションが最後に更新されたときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="f661f-162">Timestamp when this action was last updated.</span></span> <span data-ttu-id="f661f-163">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f661f-163">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f661f-164">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f661f-164">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f661f-165">name</span><span class="sxs-lookup"><span data-stu-id="f661f-165">name</span></span>|<span data-ttu-id="f661f-166">String</span><span class="sxs-lookup"><span data-stu-id="f661f-166">String</span></span>| <span data-ttu-id="f661f-167">アクション名。</span><span class="sxs-lookup"><span data-stu-id="f661f-167">Action name.</span></span>|
|<span data-ttu-id="f661f-168">parameters</span><span class="sxs-lookup"><span data-stu-id="f661f-168">parameters</span></span>|<span data-ttu-id="f661f-169">[keyValuePair](keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f661f-169">[keyValuePair](keyvaluepair.md) collection</span></span>| <span data-ttu-id="f661f-170">アクションを呼び出すために必要なパラメーター (キーと値のペア) のコレクション (たとえば、ブロックする URL または filehash など)。</span><span class="sxs-lookup"><span data-stu-id="f661f-170">Collection of parameters (key-value pairs) necessary to invoke the action, e.g. URL or fileHash to block, etc.).</span></span> <span data-ttu-id="f661f-171">**Required**</span><span class="sxs-lookup"><span data-stu-id="f661f-171">**Required**</span></span>|
|<span data-ttu-id="f661f-172">示し</span><span class="sxs-lookup"><span data-stu-id="f661f-172">states</span></span>|<span data-ttu-id="f661f-173">[securityactionstate](securityactionstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f661f-173">[securityActionState](securityactionstate.md) collection</span></span>|<span data-ttu-id="f661f-174">アクションの履歴を保持する securityactionstate のコレクション。</span><span class="sxs-lookup"><span data-stu-id="f661f-174">Collection of securityActionState to keep the history of an action.</span></span>|
|<span data-ttu-id="f661f-175">status</span><span class="sxs-lookup"><span data-stu-id="f661f-175">status</span></span>|<span data-ttu-id="f661f-176">string</span><span class="sxs-lookup"><span data-stu-id="f661f-176">string</span></span>| <span data-ttu-id="f661f-177">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="f661f-177">Status of the action.</span></span> <span data-ttu-id="f661f-178">使用可能な値は、`NotStarted`、`Running`、`Completed`、`Failed` です。</span><span class="sxs-lookup"><span data-stu-id="f661f-178">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="f661f-179">user</span><span class="sxs-lookup"><span data-stu-id="f661f-179">user</span></span>|<span data-ttu-id="f661f-180">String</span><span class="sxs-lookup"><span data-stu-id="f661f-180">String</span></span>| <span data-ttu-id="f661f-181">アクションを送信 (POST) した、サインインしているユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="f661f-181">The user principal name of the signed-in user that submitted  (POST) the action.</span></span> <span data-ttu-id="f661f-182">ユーザーは、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。</span><span class="sxs-lookup"><span data-stu-id="f661f-182">The user should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="f661f-183">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="f661f-183">vendorInformation</span></span>|[<span data-ttu-id="f661f-184">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="f661f-184">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="f661f-185">セキュリティ製品/サービスベンダー、プロバイダー、およびサブプロバイダに関する詳細を含む複合型 (ベンダー = Microsoft; provider = Windows Defender ATP; サブプロバイダ = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="f661f-185">Complex Type containing details about the Security product/service vendor, provider, and sub-provider (e.g. vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f661f-186">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f661f-186">Relationships</span></span>

<span data-ttu-id="f661f-187">なし</span><span class="sxs-lookup"><span data-stu-id="f661f-187">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f661f-188">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f661f-188">JSON representation</span></span>

<span data-ttu-id="f661f-189">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f661f-189">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityAction",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "actionReason": "String",
  "appId": "String",
  "azureTenantId": "String",
  "clientContext": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "errorInfo": {"@odata.type": "microsoft.graph.resultInfo"},
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.keyValuePair"}],
  "states": [{"@odata.type": "microsoft.graph.securityActionState"}],
  "status": "string",
  "user": "String",
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->