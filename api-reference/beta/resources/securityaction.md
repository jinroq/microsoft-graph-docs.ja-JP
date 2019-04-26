---
title: securityAction リソースの種類
description: Microsoft Graph のセキュリティの securityAction エンティティを使用して、脅威から保護するためのアクションをただちに実行します。 セキュリティ アナリストが、悪意のあるファイル、URL、ドメイン、IP アドレスなどの新しいインジケーターを発見した場合、Microsoft のセキュリティ ソリューションでそれらに対する保護をすぐに有効にできます。 特定のプロバイダーのアクションを呼び出し、実行されるすべての操作を表示し、必要な場合は操作を取り消します。 Windows Defender ATP (近日公開) でセキュリティ アクションを実行し、アラートに表示されるプロパティまたは調査中に特定されるプロパティを使用して Windows のエンドポイントの悪意のあるアクティビティをブロックします。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 5aa99119f23baa4cd9450d48ee4955d7ce91f60d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343368"
---
# <a name="securityaction-resource-type"></a><span data-ttu-id="744cc-106">securityAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="744cc-106">securityAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="744cc-107">Microsoft Graph のセキュリティの securityAction エンティティを使用して、脅威から保護するためのアクションをただちに実行します。</span><span class="sxs-lookup"><span data-stu-id="744cc-107">Take immediate action to defend against threats using the Microsoft Graph Security securityAction entity.</span></span> <span data-ttu-id="744cc-108">セキュリティ アナリストが、悪意のあるファイル、URL、ドメイン、IP アドレスなどの新しいインジケーターを発見した場合、Microsoft のセキュリティ ソリューションでそれらに対する保護をすぐに有効にできます。</span><span class="sxs-lookup"><span data-stu-id="744cc-108">When a security analyst discovers a new indicator, such as a malicious file, URL, domain, or IP address, protection can be instantly enabled in your Microsoft security solutions.</span></span> <span data-ttu-id="744cc-109">特定のプロバイダーのアクションを呼び出し、実行されるすべての操作を表示し、必要な場合は操作を取り消します。</span><span class="sxs-lookup"><span data-stu-id="744cc-109">Invoke an action for a specific provider, see all actions taken, and cancel an action if needed.</span></span> <span data-ttu-id="744cc-110">[windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection)を使用してセキュリティアクションを試行し、警告で表示されたプロパティを使用して windows エンドポイント上の悪意のあるアクティビティをブロックするか、調査中に特定します。</span><span class="sxs-lookup"><span data-stu-id="744cc-110">Try security actions with [Windows Defender ATP](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection) to block malicious activity on your Windows endpoints using properties seen in alerts or identified during investigations.</span></span>

  > <span data-ttu-id="744cc-111">**注:** 現在、セキュリティアクションはアプリケーションのアクセス許可のみサポートしています。</span><span class="sxs-lookup"><span data-stu-id="744cc-111">**Note:** Currently security actions only support application permissions.</span></span>

## <a name="methods"></a><span data-ttu-id="744cc-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="744cc-112">Methods</span></span>

| <span data-ttu-id="744cc-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="744cc-113">Method</span></span>       | <span data-ttu-id="744cc-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="744cc-114">Return Type</span></span> | <span data-ttu-id="744cc-115">説明</span><span class="sxs-lookup"><span data-stu-id="744cc-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="744cc-116">セキュリティ アクションを取得する</span><span class="sxs-lookup"><span data-stu-id="744cc-116">Get security action</span></span>](../api/securityaction-get.md) | [<span data-ttu-id="744cc-117">securityAction</span><span class="sxs-lookup"><span data-stu-id="744cc-117">securityAction</span></span>](securityaction.md) | <span data-ttu-id="744cc-118">securityAction オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="744cc-118">Read properties and relationships of securityAction object.</span></span> |
| [<span data-ttu-id="744cc-119">セキュリティ アクションを作成する</span><span class="sxs-lookup"><span data-stu-id="744cc-119">Create security action</span></span>](../api/securityactions-post.md) | [<span data-ttu-id="744cc-120">securityAction</span><span class="sxs-lookup"><span data-stu-id="744cc-120">securityAction</span></span>](securityaction.md) | <span data-ttu-id="744cc-121">securityactions コレクションへの投稿によって新しい securityAction を作成します。</span><span class="sxs-lookup"><span data-stu-id="744cc-121">Create a new securityAction by posting to the securityActions collection.</span></span> |
| [<span data-ttu-id="744cc-122">セキュリティ アクションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="744cc-122">List security actions</span></span>](../api/securityactions-list.md) | <span data-ttu-id="744cc-123">[securityAction](securityaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="744cc-123">[securityAction](securityaction.md) collection</span></span> | <span data-ttu-id="744cc-124">securityAction オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="744cc-124">Get a securityAction object collection.</span></span> |
|[<span data-ttu-id="744cc-125">セキュリティ アクションをキャンセルする</span><span class="sxs-lookup"><span data-stu-id="744cc-125">Cancel security action</span></span>](../api/securityaction-cancelsecurityaction.md)|<span data-ttu-id="744cc-126">なし</span><span class="sxs-lookup"><span data-stu-id="744cc-126">None</span></span>|<span data-ttu-id="744cc-127">セキュリティ操作をキャンセルします。</span><span class="sxs-lookup"><span data-stu-id="744cc-127">Cancel a security operation.</span></span>|

## <a name="properties"></a><span data-ttu-id="744cc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="744cc-128">Properties</span></span>

| <span data-ttu-id="744cc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="744cc-129">Property</span></span>     | <span data-ttu-id="744cc-130">型</span><span class="sxs-lookup"><span data-stu-id="744cc-130">Type</span></span>        | <span data-ttu-id="744cc-131">説明</span><span class="sxs-lookup"><span data-stu-id="744cc-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="744cc-132">actionreason</span><span class="sxs-lookup"><span data-stu-id="744cc-132">actionReason</span></span>|<span data-ttu-id="744cc-133">String</span><span class="sxs-lookup"><span data-stu-id="744cc-133">String</span></span>|<span data-ttu-id="744cc-134">このアクションを起動する理由。</span><span class="sxs-lookup"><span data-stu-id="744cc-134">Reason for invoking this action.</span></span>|
|<span data-ttu-id="744cc-135">appId</span><span class="sxs-lookup"><span data-stu-id="744cc-135">appId</span></span>|<span data-ttu-id="744cc-136">String</span><span class="sxs-lookup"><span data-stu-id="744cc-136">String</span></span>|<span data-ttu-id="744cc-137">アクションを送信 (POST) した、呼び出し元アプリケーションのアプリケーション ID。</span><span class="sxs-lookup"><span data-stu-id="744cc-137">The Application ID of the calling application that submitted (POST) the action.</span></span> <span data-ttu-id="744cc-138">appId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。</span><span class="sxs-lookup"><span data-stu-id="744cc-138">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="744cc-139">azureTenantId</span><span class="sxs-lookup"><span data-stu-id="744cc-139">azureTenantId</span></span>|<span data-ttu-id="744cc-140">String</span><span class="sxs-lookup"><span data-stu-id="744cc-140">String</span></span>|<span data-ttu-id="744cc-141">エンティティが属しているテナントを判断するエンティティの Azure テナント ID (マルチテナントのサポート)。</span><span class="sxs-lookup"><span data-stu-id="744cc-141">Azure tenant ID of the entity to determine which tenant the entity belongs to (multi-tenancy support).</span></span> <span data-ttu-id="744cc-142">azureTenantId は、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。</span><span class="sxs-lookup"><span data-stu-id="744cc-142">The azureTenantId should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="744cc-143">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="744cc-143">completedDateTime</span></span>|<span data-ttu-id="744cc-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="744cc-144">DateTimeOffset</span></span>|<span data-ttu-id="744cc-145">アクションが完了したときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="744cc-145">Timestamp when the action was completed.</span></span> <span data-ttu-id="744cc-146">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="744cc-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="744cc-147">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="744cc-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="744cc-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="744cc-148">createdDateTime</span></span>|<span data-ttu-id="744cc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="744cc-149">DateTimeOffset</span></span>|<span data-ttu-id="744cc-150">アクションが作成されたときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="744cc-150">Timestamp when the action is created.</span></span> <span data-ttu-id="744cc-151">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="744cc-151">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="744cc-152">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="744cc-152">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="744cc-153">errorInfo</span><span class="sxs-lookup"><span data-stu-id="744cc-153">errorInfo</span></span>|[<span data-ttu-id="744cc-154">resultInfo</span><span class="sxs-lookup"><span data-stu-id="744cc-154">resultInfo</span></span>](resultinfo.md)| <span data-ttu-id="744cc-155">アクションが失敗した場合のエラー情報。</span><span class="sxs-lookup"><span data-stu-id="744cc-155">Error info when the action fails.</span></span>|
|<span data-ttu-id="744cc-156">id</span><span class="sxs-lookup"><span data-stu-id="744cc-156">id</span></span>|<span data-ttu-id="744cc-157">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="744cc-157">String</span></span>| <span data-ttu-id="744cc-158">アクションが取り込まれたの場合に、システムによって作成されます。</span><span class="sxs-lookup"><span data-stu-id="744cc-158">Created by the system when the action is ingested.</span></span> <span data-ttu-id="744cc-159">生成された GUID/一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="744cc-159">Generated GUID/unique identifier.</span></span> <span data-ttu-id="744cc-160">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="744cc-160">Read-only.</span></span>|
|<span data-ttu-id="744cc-161">lastactiondatetime</span><span class="sxs-lookup"><span data-stu-id="744cc-161">lastActionDateTime</span></span>|<span data-ttu-id="744cc-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="744cc-162">DateTimeOffset</span></span>| <span data-ttu-id="744cc-163">このアクションが最後に更新されたときのタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="744cc-163">Timestamp when this action was last updated.</span></span> <span data-ttu-id="744cc-164">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="744cc-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="744cc-165">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="744cc-165">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="744cc-166">name</span><span class="sxs-lookup"><span data-stu-id="744cc-166">name</span></span>|<span data-ttu-id="744cc-167">String</span><span class="sxs-lookup"><span data-stu-id="744cc-167">String</span></span>| <span data-ttu-id="744cc-168">アクション名。</span><span class="sxs-lookup"><span data-stu-id="744cc-168">Action name.</span></span>|
|<span data-ttu-id="744cc-169">parameters</span><span class="sxs-lookup"><span data-stu-id="744cc-169">parameters</span></span>|<span data-ttu-id="744cc-170">[keyValuePair](keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="744cc-170">[keyValuePair](keyvaluepair.md) collection</span></span>| <span data-ttu-id="744cc-171">アクションを呼び出すために必要なパラメーター (キーと値のペア) のコレクション (たとえば、ブロックする URL または filehash など)。</span><span class="sxs-lookup"><span data-stu-id="744cc-171">Collection of parameters (key-value pairs) necessary to invoke the action, e.g. URL or fileHash to block, etc.).</span></span> <span data-ttu-id="744cc-172">**必須**</span><span class="sxs-lookup"><span data-stu-id="744cc-172">**Required**</span></span>|
|<span data-ttu-id="744cc-173">示し</span><span class="sxs-lookup"><span data-stu-id="744cc-173">states</span></span>|<span data-ttu-id="744cc-174">[securityactionstate](securityactionstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="744cc-174">[securityActionState](securityactionstate.md) collection</span></span>|<span data-ttu-id="744cc-175">アクションの履歴を保持する securityactionstate のコレクション。</span><span class="sxs-lookup"><span data-stu-id="744cc-175">Collection of securityActionState to keep the history of an action.</span></span>|
|<span data-ttu-id="744cc-176">status</span><span class="sxs-lookup"><span data-stu-id="744cc-176">status</span></span>|<span data-ttu-id="744cc-177">string</span><span class="sxs-lookup"><span data-stu-id="744cc-177">string</span></span>| <span data-ttu-id="744cc-178">アクションの状態。</span><span class="sxs-lookup"><span data-stu-id="744cc-178">Status of the action.</span></span> <span data-ttu-id="744cc-179">使用可能な値は、`NotStarted`、`Running`、`Completed`、`Failed` です。</span><span class="sxs-lookup"><span data-stu-id="744cc-179">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="744cc-180">user</span><span class="sxs-lookup"><span data-stu-id="744cc-180">user</span></span>|<span data-ttu-id="744cc-181">String</span><span class="sxs-lookup"><span data-stu-id="744cc-181">String</span></span>| <span data-ttu-id="744cc-182">アクションを送信 (POST) した、サインインしているユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="744cc-182">The user principal name of the signed-in user that submitted  (POST) the action.</span></span> <span data-ttu-id="744cc-183">ユーザーは、認証トークンから抽出され、呼び出し元アプリケーションによって手動で入力されることはありません。</span><span class="sxs-lookup"><span data-stu-id="744cc-183">The user should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="744cc-184">vendorInformation</span><span class="sxs-lookup"><span data-stu-id="744cc-184">vendorInformation</span></span>|[<span data-ttu-id="744cc-185">securityVendorInformation</span><span class="sxs-lookup"><span data-stu-id="744cc-185">securityVendorInformation</span></span>](securityvendorinformation.md)|<span data-ttu-id="744cc-186">セキュリティ製品/サービスベンダー、プロバイダー、およびサブプロバイダに関する詳細を含む複合型 (ベンダー = Microsoft; provider = Windows Defender ATP; サブプロバイダ = AppLocker)。</span><span class="sxs-lookup"><span data-stu-id="744cc-186">Complex Type containing details about the Security product/service vendor, provider, and sub-provider (e.g. vendor=Microsoft; provider=Windows Defender ATP; sub-provider=AppLocker).</span></span>|

## <a name="relationships"></a><span data-ttu-id="744cc-187">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="744cc-187">Relationships</span></span>

<span data-ttu-id="744cc-188">なし</span><span class="sxs-lookup"><span data-stu-id="744cc-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="744cc-189">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="744cc-189">JSON representation</span></span>

<span data-ttu-id="744cc-190">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="744cc-190">The following is a JSON representation of the resource.</span></span>

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