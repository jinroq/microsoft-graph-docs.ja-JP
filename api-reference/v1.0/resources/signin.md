---
title: サインイン リソースの種類
description: テナント (ディレクトリ) のユーザーおよびアプリケーションのサインインアクティビティについて説明します。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 735f7cc453a15ebf36aabc0e4d6a7a845a6c416c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034231"
---
# <a name="signin-resource-type"></a><span data-ttu-id="e398f-103">サインイン リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e398f-103">signIn resource type</span></span>

<span data-ttu-id="e398f-104">テナント (ディレクトリ) のユーザーおよびアプリケーションのサインインアクティビティについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e398f-104">Details user and application sign-in activity for a tenant (directory).</span></span>

## <a name="methods"></a><span data-ttu-id="e398f-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="e398f-105">Methods</span></span>

| <span data-ttu-id="e398f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e398f-106">Method</span></span>           | <span data-ttu-id="e398f-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e398f-107">Return Type</span></span>    |<span data-ttu-id="e398f-108">説明</span><span class="sxs-lookup"><span data-stu-id="e398f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e398f-109">サインインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e398f-109">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="e398f-110">サインイン</span><span class="sxs-lookup"><span data-stu-id="e398f-110">signIn</span></span>](signin.md) |<span data-ttu-id="e398f-111">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e398f-111">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="e398f-112">サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="e398f-112">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="e398f-113">サインイン</span><span class="sxs-lookup"><span data-stu-id="e398f-113">signIn</span></span>](signin.md) |<span data-ttu-id="e398f-114">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e398f-114">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e398f-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e398f-115">Properties</span></span>
| <span data-ttu-id="e398f-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e398f-116">Property</span></span>     | <span data-ttu-id="e398f-117">型</span><span class="sxs-lookup"><span data-stu-id="e398f-117">Type</span></span>   |<span data-ttu-id="e398f-118">説明</span><span class="sxs-lookup"><span data-stu-id="e398f-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e398f-119">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="e398f-119">appDisplayName</span></span>|<span data-ttu-id="e398f-120">String</span><span class="sxs-lookup"><span data-stu-id="e398f-120">String</span></span>|<span data-ttu-id="e398f-121">Azure Portal に表示されるアプリ名。</span><span class="sxs-lookup"><span data-stu-id="e398f-121">App name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="e398f-122">appId</span><span class="sxs-lookup"><span data-stu-id="e398f-122">appId</span></span>|<span data-ttu-id="e398f-123">String</span><span class="sxs-lookup"><span data-stu-id="e398f-123">String</span></span>|<span data-ttu-id="e398f-124">Azure Active Directory のアプリ ID を表す一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="e398f-124">Unique GUID representing the app ID in the Azure Active Directory.</span></span>|
|<span data-ttu-id="e398f-125">appliedConditionalAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="e398f-125">appliedConditionalAccessPolicy</span></span>|<span data-ttu-id="e398f-126">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e398f-126">[appliedConditionalAccessPolicy](appliedconditionalaccesspolicy.md) collection</span></span>|<span data-ttu-id="e398f-127">対応するサインイン アクティビティでトリガーされる条件付きアクセス ポリシーの一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="e398f-127">Provides a list of conditional access policies that are triggered by the corresponding sign-in activity.</span></span>|
|<span data-ttu-id="e398f-128">clientAppUsed</span><span class="sxs-lookup"><span data-stu-id="e398f-128">clientAppUsed</span></span>|<span data-ttu-id="e398f-129">String</span><span class="sxs-lookup"><span data-stu-id="e398f-129">String</span></span>|<span data-ttu-id="e398f-130">サインインアクティビティに使用されるレガシクライアントを識別します。</span><span class="sxs-lookup"><span data-stu-id="e398f-130">Identifies the legacy client used for sign-in activity.</span></span>  <span data-ttu-id="e398f-131">ブラウザー、Exchange アクティブ同期、モダンクライアント、IMAP、MAPI、SMTP、POP が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e398f-131">Includes Browser, Exchange Active Sync, modern clients, IMAP, MAPI, SMTP, and POP.</span></span>|
|<span data-ttu-id="e398f-132">conditionalAccessStatus</span><span class="sxs-lookup"><span data-stu-id="e398f-132">conditionalAccessStatus</span></span>|<span data-ttu-id="e398f-133">string</span><span class="sxs-lookup"><span data-stu-id="e398f-133">string</span></span>| <span data-ttu-id="e398f-134">アクティブ化された条件付きアクセスポリシーの状態を報告します。</span><span class="sxs-lookup"><span data-stu-id="e398f-134">Reports status of an activated conditional access policy.</span></span> <span data-ttu-id="e398f-135">可能な値は`success`、 `failure`、 `notApplied`、、 `unknownFutureValue`です。</span><span class="sxs-lookup"><span data-stu-id="e398f-135">Possible values are: `success`, `failure`, `notApplied`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e398f-136">correlationId</span><span class="sxs-lookup"><span data-stu-id="e398f-136">correlationId</span></span>|<span data-ttu-id="e398f-137">String</span><span class="sxs-lookup"><span data-stu-id="e398f-137">String</span></span>|<span data-ttu-id="e398f-138">サインインが開始されたときにクライアントから送信される要求 ID。サインインアクティビティのトラブルシューティングに使用されます。</span><span class="sxs-lookup"><span data-stu-id="e398f-138">The request ID sent from the client when the sign-in is initiated; used to troubleshoot sign-in activity.</span></span>|
|<span data-ttu-id="e398f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e398f-139">createdDateTime</span></span>|<span data-ttu-id="e398f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e398f-140">DateTimeOffset</span></span>|<span data-ttu-id="e398f-141">日付と時刻 (UTC) サインインが開始されました。</span><span class="sxs-lookup"><span data-stu-id="e398f-141">Date and time (UTC) the sign-in was initiated.</span></span> <span data-ttu-id="e398f-142">例: 2014 年1月1日午前0時`'2014-01-01T00:00:00Z'`にはと報告されます。</span><span class="sxs-lookup"><span data-stu-id="e398f-142">Example: midnight on Jan 1, 2014 is reported as `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e398f-143">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="e398f-143">deviceDetail</span></span>|[<span data-ttu-id="e398f-144">deviceDetail</span><span class="sxs-lookup"><span data-stu-id="e398f-144">deviceDetail</span></span>](devicedetail.md)|<span data-ttu-id="e398f-145">サインインが発生した場所からのデバイス情報。デバイス ID、オペレーティングシステム、およびブラウザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e398f-145">Device information from where the sign-in occurred; includes device ID, operating system, and browser.</span></span> |
|<span data-ttu-id="e398f-146">id</span><span class="sxs-lookup"><span data-stu-id="e398f-146">id</span></span>|<span data-ttu-id="e398f-147">文字列</span><span class="sxs-lookup"><span data-stu-id="e398f-147">String</span></span>|<span data-ttu-id="e398f-148">サインインアクティビティを表す一意の ID。</span><span class="sxs-lookup"><span data-stu-id="e398f-148">Unique ID representing the sign-in activity.</span></span>|
|<span data-ttu-id="e398f-149">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e398f-149">ipAddress</span></span>|<span data-ttu-id="e398f-150">String</span><span class="sxs-lookup"><span data-stu-id="e398f-150">String</span></span>|<span data-ttu-id="e398f-151">サインインに使用されたクライアントの IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="e398f-151">IP address of the client used to sign in.</span></span>|
|<span data-ttu-id="e398f-152">isInteractive</span><span class="sxs-lookup"><span data-stu-id="e398f-152">isInteractive</span></span>|<span data-ttu-id="e398f-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="e398f-153">Boolean</span></span>|<span data-ttu-id="e398f-154">サインインが対話型であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e398f-154">Indicates if a sign-in is interactive or not.</span></span>|
|<span data-ttu-id="e398f-155">location</span><span class="sxs-lookup"><span data-stu-id="e398f-155">location</span></span>|[<span data-ttu-id="e398f-156">signInLocation</span><span class="sxs-lookup"><span data-stu-id="e398f-156">signInLocation</span></span>](signinlocation.md)|<span data-ttu-id="e398f-157">サインインした場所の市区町村、都道府県、および国コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="e398f-157">Provides the city, state, and country code where the sign-in originated.</span></span>|
|<span data-ttu-id="e398f-158">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e398f-158">resourceDisplayName</span></span>|<span data-ttu-id="e398f-159">String</span><span class="sxs-lookup"><span data-stu-id="e398f-159">String</span></span>|<span data-ttu-id="e398f-160">ユーザーがサインインしたリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="e398f-160">Name of the resource the user signed into.</span></span>|
|<span data-ttu-id="e398f-161">resourceId</span><span class="sxs-lookup"><span data-stu-id="e398f-161">resourceId</span></span>|<span data-ttu-id="e398f-162">String</span><span class="sxs-lookup"><span data-stu-id="e398f-162">String</span></span>|<span data-ttu-id="e398f-163">ユーザーがサインインしたリソースの ID。</span><span class="sxs-lookup"><span data-stu-id="e398f-163">ID of the resource that the user signed into.</span></span>|
|<span data-ttu-id="e398f-164">riskDetail</span><span class="sxs-lookup"><span data-stu-id="e398f-164">riskDetail</span></span>|<span data-ttu-id="e398f-165">riskDetail</span><span class="sxs-lookup"><span data-stu-id="e398f-165">riskDetail</span></span>|<span data-ttu-id="e398f-166">リスクの高いユーザー、サインイン、リスク イベントのいずれかの特定の状態の背後にある「理由」について示します。</span><span class="sxs-lookup"><span data-stu-id="e398f-166">Provides the 'reason' behind a specific state of a risky user, sign-in or a risk event.</span></span> <span data-ttu-id="e398f-167">使用可能な値: `none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e398f-167">The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`.</span></span> <span data-ttu-id="e398f-168">値 `none` は、ユーザーについて実行されたアクションまたはサインインが今のところないことを意味しています。</span><span class="sxs-lookup"><span data-stu-id="e398f-168">The value `none` means that no action has been performed on the user or sign-in so far.</span></span> <br><span data-ttu-id="e398f-169">**注:** このプロパティの詳細には、Azure AD Premium P2 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="e398f-169">**Note:** Details for this property require an Azure AD Premium P2 license.</span></span> <span data-ttu-id="e398f-170">他のライセンスは値`hidden`を返します。</span><span class="sxs-lookup"><span data-stu-id="e398f-170">Other licenses return the value `hidden`.</span></span>|
|<span data-ttu-id="e398f-171">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="e398f-171">riskEventTypes</span></span>|<span data-ttu-id="e398f-172">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="e398f-172">riskEventTypes</span></span>|<span data-ttu-id="e398f-173">サインインに関連付けられているリスクイベントの種類。</span><span class="sxs-lookup"><span data-stu-id="e398f-173">Risk event types associated with the sign-in.</span></span> <span data-ttu-id="e398f-174">使用可能な値: `unlikelyTravel`、`anonymizedIPAddress`、`maliciousIPAddress`、`unfamiliarFeatures`、`malwareInfectedIPAddress`、`suspiciousIPAddress`、`leakedCredentials`、`investigationsThreatIntelligence`、`generic`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e398f-174">The possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`,  `generic`, and `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e398f-175">riskLevelAggregated</span><span class="sxs-lookup"><span data-stu-id="e398f-175">riskLevelAggregated</span></span>|<span data-ttu-id="e398f-176">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e398f-176">riskLevel</span></span>|<span data-ttu-id="e398f-177">集計リスクレベル。</span><span class="sxs-lookup"><span data-stu-id="e398f-177">Aggregated risk level.</span></span> <span data-ttu-id="e398f-178">使用可能な値: `none`、`low`、`medium`、`high`、`hidden`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e398f-178">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="e398f-179">値 `hidden` は、ユーザーまたはサインインが Azure AD Identity Protection で有効になっていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="e398f-179">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="e398f-180">**注:** このプロパティの詳細は、Azure AD Premium P2 のお客様のみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="e398f-180">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="e398f-181">その他のお客様には `hidden` が返されます。</span><span class="sxs-lookup"><span data-stu-id="e398f-181">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="e398f-182">riskLevelDuringSignIn</span><span class="sxs-lookup"><span data-stu-id="e398f-182">riskLevelDuringSignIn</span></span>|<span data-ttu-id="e398f-183">riskLevel</span><span class="sxs-lookup"><span data-stu-id="e398f-183">riskLevel</span></span>|<span data-ttu-id="e398f-184">サインイン中のリスクレベル。</span><span class="sxs-lookup"><span data-stu-id="e398f-184">Risk level during sign-in.</span></span> <span data-ttu-id="e398f-185">使用可能な値: `none`、`low`、`medium`、`high`、`hidden`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e398f-185">The possible values are: `none`, `low`, `medium`, `high`, `hidden`, and `unknownFutureValue`.</span></span> <span data-ttu-id="e398f-186">値 `hidden` は、ユーザーまたはサインインが Azure AD Identity Protection で有効になっていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="e398f-186">The value `hidden` means the user or sign-in was not enabled for Azure AD Identity Protection.</span></span> <span data-ttu-id="e398f-187">**注:** このプロパティの詳細は、Azure AD Premium P2 のお客様のみ利用可能です。</span><span class="sxs-lookup"><span data-stu-id="e398f-187">**Note:** Details for this property are only available for Azure AD Premium P2 customers.</span></span> <span data-ttu-id="e398f-188">その他のお客様には `hidden` が返されます。</span><span class="sxs-lookup"><span data-stu-id="e398f-188">All other customers will be returned `hidden`.</span></span>|
|<span data-ttu-id="e398f-189">riskState</span><span class="sxs-lookup"><span data-stu-id="e398f-189">riskState</span></span>|<span data-ttu-id="e398f-190">riskState</span><span class="sxs-lookup"><span data-stu-id="e398f-190">riskState</span></span>|<span data-ttu-id="e398f-191">危険なユーザー、サインイン、またはリスクイベントの状態を報告します。</span><span class="sxs-lookup"><span data-stu-id="e398f-191">Reports status of the risky user, sign-in, or a risk event.</span></span> <span data-ttu-id="e398f-192">使用可能な値: `none`、`confirmedSafe`、`remediated`、`dismissed`、`atRisk`、`confirmedCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e398f-192">The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e398f-193">status</span><span class="sxs-lookup"><span data-stu-id="e398f-193">status</span></span>|[<span data-ttu-id="e398f-194">signInStatus</span><span class="sxs-lookup"><span data-stu-id="e398f-194">signInStatus</span></span>](signinstatus.md)|<span data-ttu-id="e398f-195">サインイン状態。</span><span class="sxs-lookup"><span data-stu-id="e398f-195">Sign-in status.</span></span> <span data-ttu-id="e398f-196">使用可能な値は、`Success`、`Failure` です。</span><span class="sxs-lookup"><span data-stu-id="e398f-196">Possible values include `Success` and `Failure`.</span></span>|
|<span data-ttu-id="e398f-197">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e398f-197">userDisplayName</span></span>|<span data-ttu-id="e398f-198">String</span><span class="sxs-lookup"><span data-stu-id="e398f-198">String</span></span>|<span data-ttu-id="e398f-199">サインインを開始したユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="e398f-199">Display name of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="e398f-200">userId</span><span class="sxs-lookup"><span data-stu-id="e398f-200">userId</span></span>|<span data-ttu-id="e398f-201">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e398f-201">String</span></span>|<span data-ttu-id="e398f-202">サインインを開始したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="e398f-202">ID of the user that initiated the sign-in.</span></span>|
|<span data-ttu-id="e398f-203">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e398f-203">userPrincipalName</span></span>|<span data-ttu-id="e398f-204">String</span><span class="sxs-lookup"><span data-stu-id="e398f-204">String</span></span>|<span data-ttu-id="e398f-205">サインインを開始したユーザーのユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="e398f-205">User principal name of the user that initiated the sign-in.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e398f-206">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e398f-206">Relationships</span></span>

<span data-ttu-id="e398f-207">なし</span><span class="sxs-lookup"><span data-stu-id="e398f-207">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e398f-208">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e398f-208">JSON representation</span></span>

<span data-ttu-id="e398f-209">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e398f-209">Here is a JSON representation of the resource.</span></span>

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
