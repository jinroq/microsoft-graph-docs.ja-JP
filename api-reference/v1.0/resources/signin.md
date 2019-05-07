---
title: サインイン リソースの種類
description: テナント (ディレクトリ) のユーザーおよびアプリケーションのサインインアクティビティについて説明します。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb73b843643c5ffba1b5cdac3d7fd519819109ba
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629244"
---
# <a name="signin-resource-type"></a><span data-ttu-id="75fed-103">サインイン リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75fed-103">signIn resource type</span></span>

<span data-ttu-id="75fed-104">テナント (ディレクトリ) のユーザーおよびアプリケーションのサインインアクティビティについて説明します。</span><span class="sxs-lookup"><span data-stu-id="75fed-104">Details user and application sign-in activity for a tenant (directory).</span></span>

## <a name="methods"></a><span data-ttu-id="75fed-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="75fed-105">Methods</span></span>

| <span data-ttu-id="75fed-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="75fed-106">Method</span></span>           | <span data-ttu-id="75fed-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="75fed-107">Return Type</span></span>    |<span data-ttu-id="75fed-108">説明</span><span class="sxs-lookup"><span data-stu-id="75fed-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="75fed-109">サインインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="75fed-109">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="75fed-110">サインイン</span><span class="sxs-lookup"><span data-stu-id="75fed-110">signIn</span></span>](signin.md) |<span data-ttu-id="75fed-111">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75fed-111">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="75fed-112">サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="75fed-112">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="75fed-113">サインイン</span><span class="sxs-lookup"><span data-stu-id="75fed-113">signIn</span></span>](signin.md) |<span data-ttu-id="75fed-114">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75fed-114">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75fed-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75fed-115">Properties</span></span>
| <span data-ttu-id="75fed-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75fed-116">Property</span></span>     | <span data-ttu-id="75fed-117">型</span><span class="sxs-lookup"><span data-stu-id="75fed-117">Type</span></span>   |<span data-ttu-id="75fed-118">説明</span><span class="sxs-lookup"><span data-stu-id="75fed-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="75fed-119">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="75fed-119">appDisplayName</span></span>|<span data-ttu-id="75fed-120">String</span><span class="sxs-lookup"><span data-stu-id="75fed-120">String</span></span>|<span data-ttu-id="75fed-121">Azure Portal に表示されるアプリ名。</span><span class="sxs-lookup"><span data-stu-id="75fed-121">App name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="75fed-122">appId</span><span class="sxs-lookup"><span data-stu-id="75fed-122">appId</span></span>|<span data-ttu-id="75fed-123">String</span><span class="sxs-lookup"><span data-stu-id="75fed-123">String</span></span>|<span data-ttu-id="75fed-124">Azure Active Directory のアプリ ID を表す一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="75fed-124">Unique GUID representing the app ID in the Azure Active Directory.</span></span>|
|<span data-ttu-id="75fed-125">appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="75fed-125">appliedConditionalAccessPolicy</span></span>|<span data-ttu-id="75fed-126">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="75fed-126">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection</span></span>|<span data-ttu-id="75fed-127">対応するサインイン アクティビティでトリガーされる条件付きアクセス ポリシーの一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="75fed-127">Provides a list of conditional access policies that are triggered by the corresponding sign-in activity.</span></span>|
|<span data-ttu-id="75fed-128">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="75fed-128">clientAppUsed</span></span>|<span data-ttu-id="75fed-129">String</span><span class="sxs-lookup"><span data-stu-id="75fed-129">String</span></span>|<span data-ttu-id="75fed-130">サインインアクティビティに使用されるレガシクライアントを識別します。</span><span class="sxs-lookup"><span data-stu-id="75fed-130">Identifies the legacy client used for sign-in activity.</span></span>  <span data-ttu-id="75fed-131">ブラウザー、Exchange アクティブ同期、モダンクライアント、IMAP、MAPI、SMTP、POP が含まれています。</span><span class="sxs-lookup"><span data-stu-id="75fed-131">Includes Browser, Exchange Active Sync, modern clients, IMAP, MAPI, SMTP, and POP.</span></span>|
|<span data-ttu-id="75fed-132">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="75fed-132">conditionalAccessStatus</span></span>|<span data-ttu-id="75fed-133">string</span><span class="sxs-lookup"><span data-stu-id="75fed-133">string</span></span>| <span data-ttu-id="75fed-134">アクティブ化された条件付きアクセスポリシーの状態を報告します。</span><span class="sxs-lookup"><span data-stu-id="75fed-134">Reports status of an activated conditional access policy.</span></span> <span data-ttu-id="75fed-135">可能な値は`success`、 `failure`、 `notApplied`、、 `unknownFutureValue`です。</span><span class="sxs-lookup"><span data-stu-id="75fed-135">Possible values are: `success`, `failure`, `notApplied`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="75fed-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="75fed-136">correlationId</span></span>|<span data-ttu-id="75fed-137">String</span><span class="sxs-lookup"><span data-stu-id="75fed-137">String</span></span>|<span data-ttu-id="75fed-138">サインインが開始されたときにクライアントから送信される要求 ID。サインインアクティビティのトラブルシューティングに使用されます。</span><span class="sxs-lookup"><span data-stu-id="75fed-138">The request ID sent from the client when the sign-in is initiated; used to troubleshoot sign-in activity.</span></span>|
|<span data-ttu-id="75fed-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75fed-139">createdDateTime</span></span>|<span data-ttu-id="75fed-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75fed-140">DateTimeOffset</span></span>|<span data-ttu-id="75fed-141">日付と時刻 (UTC) サインインが開始されました。</span><span class="sxs-lookup"><span data-stu-id="75fed-141">Date and time (UTC) the sign-in was initiated.</span></span> <span data-ttu-id="75fed-142">例: 2014 年1月1日午前0時`'2014-01-01T00:00:00Z'`にはと報告されます。</span><span class="sxs-lookup"><span data-stu-id="75fed-142">Example: midnight on Jan 1, 2014 is reported as `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="75fed-143">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="75fed-143">deviceDetail</span></span>|[<span data-ttu-id="75fed-144">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="75fed-144">deviceDetail</span></span>](devicedetail.md)|<span data-ttu-id="75fed-145">サインインが発生した場所からのデバイス情報。デバイス ID、オペレーティングシステム、およびブラウザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="75fed-145">Device information from where the sign-in occurred; includes device ID, operating system, and browser.</span></span> |
|<span data-ttu-id="75fed-146">id</span><span class="sxs-lookup"><span data-stu-id="75fed-146">id</span></span>|<span data-ttu-id="75fed-147">文字列</span><span class="sxs-lookup"><span data-stu-id="75fed-147">String</span></span>|<span data-ttu-id="75fed-148">サインインアクティビティを表す一意の ID。</span><span class="sxs-lookup"><span data-stu-id="75fed-148">Unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="75fed-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="75fed-149">ipAddress</span></span>|<span data-ttu-id="75fed-150">String</span><span class="sxs-lookup"><span data-stu-id="75fed-150">String</span></span>|<span data-ttu-id="75fed-151">サインインに使用されたクライアントの IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="75fed-151">IP address of the client used to sign in.</span></span>|
|<span data-ttu-id="75fed-152">isInteractive</span><span class="sxs-lookup"><span data-stu-id="75fed-152">isInteractive</span></span>|<span data-ttu-id="75fed-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="75fed-153">Boolean</span></span>|<span data-ttu-id="75fed-154">サインインが対話型であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="75fed-154">Indicates if a sign-in is interactive or not.</span></span>|
|<span data-ttu-id="75fed-155">location</span><span class="sxs-lookup"><span data-stu-id="75fed-155">location</span></span>|[<span data-ttu-id="75fed-156">signInLocation</span><span class="sxs-lookup"><span data-stu-id="75fed-156">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="75fed-157">サインインした場所の市区町村、都道府県、および国コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="75fed-157">Provides the city, state, and country code where the sign-in originated.</span></span>|
|<span data-ttu-id="75fed-158">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="75fed-158">resourceDisplayName</span></span>|<span data-ttu-id="75fed-159">String</span><span class="sxs-lookup"><span data-stu-id="75fed-159">String</span></span>|<span data-ttu-id="75fed-160">ユーザーがサインインしたリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="75fed-160">Name of the resource the user signed into.</span></span>|
|<span data-ttu-id="75fed-161">resourceId</span><span class="sxs-lookup"><span data-stu-id="75fed-161">resourceId</span></span>|<span data-ttu-id="75fed-162">String</span><span class="sxs-lookup"><span data-stu-id="75fed-162">String</span></span>|<span data-ttu-id="75fed-163">ユーザーがサインインしたリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="75fed-163">ID of the resource that the user signed into.</span></span>|
|<span data-ttu-id="75fed-164">riskDetail</span><span class="sxs-lookup"><span data-stu-id="75fed-164">riskDetail</span></span>|<span data-ttu-id="75fed-165">riskDetail</span><span class="sxs-lookup"><span data-stu-id="75fed-165">riskDetail</span></span>|<span data-ttu-id="75fed-166">リスクの高いユーザー、サインイン、リスク イベントのいずれかの特定の状態の背後にある「理由」について示します。</span><span class="sxs-lookup"><span data-stu-id="75fed-166">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="75fed-167">使用可能な値: `none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="75fed-167">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="75fed-168">値 `none` は、ユーザーについて実行されたアクションまたはサインインが今のところないことを意味しています。</span><span class="sxs-lookup"><span data-stu-id="75fed-168">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> <br><span data-ttu-id="75fed-169">**注:** このプロパティの詳細には、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="75fed-169">**Note:** Details for this property require an Azure AD Premium P2 license.</span></span> <span data-ttu-id="75fed-170">他のライセンスは値`hidden`を返します。</span><span class="sxs-lookup"><span data-stu-id="75fed-170">Other licenses return the value `hidden`.</span></span>|
|<span data-ttu-id="75fed-171">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="75fed-171">riskEventTypes</span></span>|<span data-ttu-id="75fed-172">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="75fed-172">riskEventTypes</span></span>|<span data-ttu-id="75fed-173">サインインに関連付けられているリスクイベントの種類。</span><span class="sxs-lookup"><span data-stu-id="75fed-173">Risk event types associated with the sign-in.</span></span> <span data-ttu-id="75fed-174">使用可能な値: `unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="75fed-174">The possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="75fed-175">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="75fed-175">riskLevelAggregated</span></span>|<span data-ttu-id="75fed-176">riskLevel</span><span class="sxs-lookup"><span data-stu-id="75fed-176">riskLevel</span></span>|<span data-ttu-id="75fed-177">集計リスクレベル。</span><span class="sxs-lookup"><span data-stu-id="75fed-177">Aggregated risk level.</span></span> <span data-ttu-id="75fed-178">使用可能な値: `none`、`low`、`medium`、`high`、`hidden`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="75fed-178">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="75fed-179">値 `hidden` は、ユーザーまたはサインインが Azure AD Identity Protection で有効になっていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="75fed-179">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="75fed-180">**注:** このプロパティの詳細は、Azure AD Premium P2 のお客様のみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="75fed-180">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="75fed-181">その他のお客様には `hidden` が返されます。</span><span class="sxs-lookup"><span data-stu-id="75fed-181">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="75fed-182">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="75fed-182">riskLevelDuringSignIn</span></span>|<span data-ttu-id="75fed-183">riskLevel</span><span class="sxs-lookup"><span data-stu-id="75fed-183">riskLevel</span></span>|<span data-ttu-id="75fed-184">サインイン中のリスクレベル。</span><span class="sxs-lookup"><span data-stu-id="75fed-184">Risk level during sign-in.</span></span> <span data-ttu-id="75fed-185">使用可能な値: `none`、`low`、`medium`、`high`、`hidden`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="75fed-185">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="75fed-186">値 `hidden` は、ユーザーまたはサインインが Azure AD Identity Protection で有効になっていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="75fed-186">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="75fed-187">**注:** このプロパティの詳細は、Azure AD Premium P2 のお客様のみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="75fed-187">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="75fed-188">その他のお客様には `hidden` が返されます。</span><span class="sxs-lookup"><span data-stu-id="75fed-188">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="75fed-189">riskState</span><span class="sxs-lookup"><span data-stu-id="75fed-189">riskState</span></span>|<span data-ttu-id="75fed-190">riskState</span><span class="sxs-lookup"><span data-stu-id="75fed-190">riskState</span></span>|<span data-ttu-id="75fed-191">危険なユーザー、サインイン、またはリスクイベントの状態を報告します。</span><span class="sxs-lookup"><span data-stu-id="75fed-191">Reports status of the risky user, sign-in, or a risk event.</span></span> <span data-ttu-id="75fed-192">使用可能な値: `none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="75fed-192">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="75fed-193">status</span><span class="sxs-lookup"><span data-stu-id="75fed-193">status</span></span>|[<span data-ttu-id="75fed-194">signInStatus</span><span class="sxs-lookup"><span data-stu-id="75fed-194">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="75fed-195">サインイン状態。</span><span class="sxs-lookup"><span data-stu-id="75fed-195">Sign-in status.</span></span> <span data-ttu-id="75fed-196">使用可能な値は、`Success`、`Failure` です。</span><span class="sxs-lookup"><span data-stu-id="75fed-196">Possible values include `Success` and `Failure`.</span></span>|
|<span data-ttu-id="75fed-197">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="75fed-197">userDisplayName</span></span>|<span data-ttu-id="75fed-198">String</span><span class="sxs-lookup"><span data-stu-id="75fed-198">String</span></span>|<span data-ttu-id="75fed-199">サインインを開始したユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="75fed-199">Display name of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="75fed-200">userId</span><span class="sxs-lookup"><span data-stu-id="75fed-200">userId</span></span>|<span data-ttu-id="75fed-201">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="75fed-201">String</span></span>|<span data-ttu-id="75fed-202">サインインを開始したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="75fed-202">ID of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="75fed-203">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="75fed-203">userPrincipalName</span></span>|<span data-ttu-id="75fed-204">String</span><span class="sxs-lookup"><span data-stu-id="75fed-204">String</span></span>|<span data-ttu-id="75fed-205">サインインを開始したユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="75fed-205">User principal name of the user that initiated the sign-in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75fed-206">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75fed-206">Relationships</span></span>

<span data-ttu-id="75fed-207">なし</span><span class="sxs-lookup"><span data-stu-id="75fed-207">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="75fed-208">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75fed-208">JSON representation</span></span>

<span data-ttu-id="75fed-209">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75fed-209">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signIn"
}-->
```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "appDisplayName": "String",
  "appId": "String",
  "ipAddress": "String",
  "clientAppUsed": "String",
  "correlationId": "String",
  "conditionalAccessStatus": "string",
  "appliedConditionalAccessPolicy": [{"@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"}],
  "isInteractive": "String",
  "deviceDetail": {"@odata.type": "microsoft.graph.deviceDetail"},
  "location": {"@odata.type": "microsoft.graph.signInLocation"},
  "riskDetail": "string",
  "riskLevelAggregated": "string",
  "riskLevelDuringSignIn": "string",
  "riskState": "string",
  "riskEventTypes": "string",
  "resourceDisplayName": "string",
  "resourceId": "string",
  "status": {"@odata.type": "microsoft.graph.signInStatus"},
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
