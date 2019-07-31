---
title: vppToken リソースの種類
description: ビジネス向けまたは教育向けの Apple Volume Purchase Program で iOS アプリのライセンスを複数購入した場合、 Apple の Web サイトから Apple VPP アカウントを設定し、Intune にビジネス向けまたは教育向けの Apple VPP トークンをアップロードする必要があります。 これにより、ボリューム購入情報を Intune と同期して、ボリューム購入したアプリの使用状況を追跡できます。 ビジネス向けまたは教育向けの Apple VPP トークンは複数アップロードできます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d5f8bd1453b0af02b7bdc58828f24660b46a9ff
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010673"
---
# <a name="vpptoken-resource-type"></a><span data-ttu-id="3256a-106">vppToken リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3256a-106">vppToken resource type</span></span>

> <span data-ttu-id="3256a-107">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3256a-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3256a-108">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3256a-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3256a-109">ビジネス向けまたは教育向けの Apple Volume Purchase Program で iOS アプリのライセンスを複数購入した場合、</span><span class="sxs-lookup"><span data-stu-id="3256a-109">You purchase multiple licenses for iOS apps through the Apple Volume Purchase Program for Business or Education.</span></span> <span data-ttu-id="3256a-110">Apple の Web サイトから Apple VPP アカウントを設定し、Intune にビジネス向けまたは教育向けの Apple VPP トークンをアップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3256a-110">This involves setting up an Apple VPP account from the Apple website and uploading the Apple VPP Business or Education token to Intune.</span></span> <span data-ttu-id="3256a-111">これにより、ボリューム購入情報を Intune と同期して、ボリューム購入したアプリの使用状況を追跡できます。</span><span class="sxs-lookup"><span data-stu-id="3256a-111">You can then synchronize your volume purchase information with Intune and track your volume-purchased app use.</span></span> <span data-ttu-id="3256a-112">ビジネス向けまたは教育向けの Apple VPP トークンは複数アップロードできます。</span><span class="sxs-lookup"><span data-stu-id="3256a-112">You can upload multiple Apple VPP Business or Education tokens.</span></span>

## <a name="methods"></a><span data-ttu-id="3256a-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="3256a-113">Methods</span></span>
|<span data-ttu-id="3256a-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="3256a-114">Method</span></span>|<span data-ttu-id="3256a-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3256a-115">Return Type</span></span>|<span data-ttu-id="3256a-116">説明</span><span class="sxs-lookup"><span data-stu-id="3256a-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3256a-117">vppToken のリスト</span><span class="sxs-lookup"><span data-stu-id="3256a-117">List vppTokens</span></span>](../api/intune-onboarding-vpptoken-list.md)|<span data-ttu-id="3256a-118">[vppToken](../resources/intune-onboarding-vpptoken.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3256a-118">[vppToken](../resources/intune-onboarding-vpptoken.md) collection</span></span>|<span data-ttu-id="3256a-119">[vppToken](../resources/intune-onboarding-vpptoken.md) オブジェクトのプロパティとリレーションシップのリストを作成します。</span><span class="sxs-lookup"><span data-stu-id="3256a-119">List properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) objects.</span></span>|
|[<span data-ttu-id="3256a-120">vppToken の取得</span><span class="sxs-lookup"><span data-stu-id="3256a-120">Get vppToken</span></span>](../api/intune-onboarding-vpptoken-get.md)|[<span data-ttu-id="3256a-121">vppToken</span><span class="sxs-lookup"><span data-stu-id="3256a-121">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="3256a-122">[vppToken](../resources/intune-onboarding-vpptoken.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3256a-122">Read properties and relationships of the [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="3256a-123">vppToken の作成</span><span class="sxs-lookup"><span data-stu-id="3256a-123">Create vppToken</span></span>](../api/intune-onboarding-vpptoken-create.md)|[<span data-ttu-id="3256a-124">vppToken</span><span class="sxs-lookup"><span data-stu-id="3256a-124">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="3256a-125">新規に[vppToken](../resources/intune-onboarding-vpptoken.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3256a-125">Create a new [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="3256a-126">vppToken の削除</span><span class="sxs-lookup"><span data-stu-id="3256a-126">Delete vppToken</span></span>](../api/intune-onboarding-vpptoken-delete.md)|<span data-ttu-id="3256a-127">なし</span><span class="sxs-lookup"><span data-stu-id="3256a-127">None</span></span>|<span data-ttu-id="3256a-128">[vppToken](../resources/intune-onboarding-vpptoken.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="3256a-128">Deletes a [vppToken](../resources/intune-onboarding-vpptoken.md).</span></span>|
|[<span data-ttu-id="3256a-129">vppToken の更新</span><span class="sxs-lookup"><span data-stu-id="3256a-129">Update vppToken</span></span>](../api/intune-onboarding-vpptoken-update.md)|[<span data-ttu-id="3256a-130">vppToken</span><span class="sxs-lookup"><span data-stu-id="3256a-130">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="3256a-131">[vppToken](../resources/intune-onboarding-vpptoken.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3256a-131">Update the properties of a [vppToken](../resources/intune-onboarding-vpptoken.md) object.</span></span>|
|[<span data-ttu-id="3256a-132">syncLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="3256a-132">syncLicenses action</span></span>](../api/intune-onboarding-vpptoken-synclicenses.md)|[<span data-ttu-id="3256a-133">vppToken</span><span class="sxs-lookup"><span data-stu-id="3256a-133">vppToken</span></span>](../resources/intune-onboarding-vpptoken.md)|<span data-ttu-id="3256a-134">特定の appleVolumePurchaseProgramToken に関連付けられたライセンスを同期します</span><span class="sxs-lookup"><span data-stu-id="3256a-134">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|
|[<span data-ttu-id="3256a-135">revokeLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="3256a-135">revokeLicenses action</span></span>](../api/intune-onboarding-vpptoken-revokelicenses.md)|<span data-ttu-id="3256a-136">None</span><span class="sxs-lookup"><span data-stu-id="3256a-136">None</span></span>|<span data-ttu-id="3256a-137">特定の appleVolumePurchaseProgramToken に関連付けられているライセンスを取り消す</span><span class="sxs-lookup"><span data-stu-id="3256a-137">Revoke licenses associated with a specific appleVolumePurchaseProgramToken</span></span>|
|[<span data-ttu-id="3256a-138">getLicensesForApp 関数</span><span class="sxs-lookup"><span data-stu-id="3256a-138">getLicensesForApp function</span></span>](../api/intune-onboarding-vpptoken-getlicensesforapp.md)|<span data-ttu-id="3256a-139">[Vpptokenlicensesummary](../resources/intune-onboarding-vpptokenlicensesummary.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3256a-139">[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection</span></span>|<span data-ttu-id="3256a-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3256a-140">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3256a-141">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3256a-141">Properties</span></span>
|<span data-ttu-id="3256a-142">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3256a-142">Property</span></span>|<span data-ttu-id="3256a-143">型</span><span class="sxs-lookup"><span data-stu-id="3256a-143">Type</span></span>|<span data-ttu-id="3256a-144">説明</span><span class="sxs-lookup"><span data-stu-id="3256a-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3256a-145">id</span><span class="sxs-lookup"><span data-stu-id="3256a-145">id</span></span>|<span data-ttu-id="3256a-146">文字列</span><span class="sxs-lookup"><span data-stu-id="3256a-146">String</span></span>|<span data-ttu-id="3256a-147">appleVolumePurchaseProgramToken 作成時に自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="3256a-147">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="3256a-148">エンティティのキーになります。</span><span class="sxs-lookup"><span data-stu-id="3256a-148">It is the Key of the entity.</span></span>|
|<span data-ttu-id="3256a-149">organizationName</span><span class="sxs-lookup"><span data-stu-id="3256a-149">organizationName</span></span>|<span data-ttu-id="3256a-150">String</span><span class="sxs-lookup"><span data-stu-id="3256a-150">String</span></span>|<span data-ttu-id="3256a-151">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="3256a-151">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="3256a-152">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3256a-152">vppTokenAccountType</span></span>|[<span data-ttu-id="3256a-153">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="3256a-153">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="3256a-154">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="3256a-154">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="3256a-155">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="3256a-155">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="3256a-156">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="3256a-156">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="3256a-157">appleId</span><span class="sxs-lookup"><span data-stu-id="3256a-157">appleId</span></span>|<span data-ttu-id="3256a-158">String</span><span class="sxs-lookup"><span data-stu-id="3256a-158">String</span></span>|<span data-ttu-id="3256a-159">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="3256a-159">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3256a-160">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3256a-160">expirationDateTime</span></span>|<span data-ttu-id="3256a-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3256a-161">DateTimeOffset</span></span>|<span data-ttu-id="3256a-162">Apple ボリューム購入プログラムのトークンの有効期限。</span><span class="sxs-lookup"><span data-stu-id="3256a-162">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3256a-163">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3256a-163">lastSyncDateTime</span></span>|<span data-ttu-id="3256a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3256a-164">DateTimeOffset</span></span>|<span data-ttu-id="3256a-165">Apple ボリューム購入プログラムのトークンを使用して、Apple ボリューム購入プログラム サービスと最後にアプリケーションの同期を行った日時。</span><span class="sxs-lookup"><span data-stu-id="3256a-165">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3256a-166">token</span><span class="sxs-lookup"><span data-stu-id="3256a-166">token</span></span>|<span data-ttu-id="3256a-167">String</span><span class="sxs-lookup"><span data-stu-id="3256a-167">String</span></span>|<span data-ttu-id="3256a-168">Apple ボリューム購入プログラムからダウンロードした Apple ボリューム購入プログラムのトークン文字列。</span><span class="sxs-lookup"><span data-stu-id="3256a-168">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="3256a-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3256a-169">lastModifiedDateTime</span></span>|<span data-ttu-id="3256a-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3256a-170">DateTimeOffset</span></span>|<span data-ttu-id="3256a-171">Apple ボリューム購入プログラムのトークンに関連付けられている最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="3256a-171">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3256a-172">state</span><span class="sxs-lookup"><span data-stu-id="3256a-172">state</span></span>|[<span data-ttu-id="3256a-173">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="3256a-173">vppTokenState</span></span>](../resources/intune-onboarding-vpptokenstate.md)|<span data-ttu-id="3256a-174">Apple ボリューム購入プログラムのトークンの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="3256a-174">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="3256a-175">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="3256a-175">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="3256a-176">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="3256a-176">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="3256a-177">tokenActionResults</span><span class="sxs-lookup"><span data-stu-id="3256a-177">tokenActionResults</span></span>|<span data-ttu-id="3256a-178">[Vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3256a-178">[vppTokenActionResult](../resources/intune-onboarding-vpptokenactionresult.md) collection</span></span>|<span data-ttu-id="3256a-179">Apple Volume Purchase Program トークンで実行されたアクションのステータスのコレクション。</span><span class="sxs-lookup"><span data-stu-id="3256a-179">The collection of statuses of the actions performed on the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="3256a-180">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="3256a-180">lastSyncStatus</span></span>|[<span data-ttu-id="3256a-181">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="3256a-181">vppTokenSyncStatus</span></span>](../resources/intune-onboarding-vpptokensyncstatus.md)|<span data-ttu-id="3256a-182">Apple ボリューム購入プログラム トークンを使用して行われた最後のアプリケーションの同期の現在の同期状態。</span><span class="sxs-lookup"><span data-stu-id="3256a-182">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="3256a-183">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="3256a-183">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="3256a-184">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="3256a-184">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="3256a-185">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="3256a-185">automaticallyUpdateApps</span></span>|<span data-ttu-id="3256a-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="3256a-186">Boolean</span></span>|<span data-ttu-id="3256a-187">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="3256a-187">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="3256a-188">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="3256a-188">countryOrRegion</span></span>|<span data-ttu-id="3256a-189">文字列</span><span class="sxs-lookup"><span data-stu-id="3256a-189">String</span></span>|<span data-ttu-id="3256a-190">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="3256a-190">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="3256a-191">dataSharingConsentGranted</span><span class="sxs-lookup"><span data-stu-id="3256a-191">dataSharingConsentGranted</span></span>|<span data-ttu-id="3256a-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="3256a-192">Boolean</span></span>|<span data-ttu-id="3256a-193">Apple Volume Purchase Program でのデータ共有に対して付与される同意。</span><span class="sxs-lookup"><span data-stu-id="3256a-193">Consent granted for data sharing with the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="3256a-194">displayName</span><span class="sxs-lookup"><span data-stu-id="3256a-194">displayName</span></span>|<span data-ttu-id="3256a-195">String</span><span class="sxs-lookup"><span data-stu-id="3256a-195">String</span></span>|<span data-ttu-id="3256a-196">管理者が指定したトークンのフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="3256a-196">An admin specified token friendly name.</span></span>|
|<span data-ttu-id="3256a-197">Msrtcsip-locationname</span><span class="sxs-lookup"><span data-stu-id="3256a-197">locationName</span></span>|<span data-ttu-id="3256a-198">String</span><span class="sxs-lookup"><span data-stu-id="3256a-198">String</span></span>|<span data-ttu-id="3256a-199">Apple VPP から返されるトークンの場所。</span><span class="sxs-lookup"><span data-stu-id="3256a-199">Token location returned from Apple VPP.</span></span>|
|<span data-ttu-id="3256a-200">claimTokenManagementFromExternalMdm</span><span class="sxs-lookup"><span data-stu-id="3256a-200">claimTokenManagementFromExternalMdm</span></span>|<span data-ttu-id="3256a-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="3256a-201">Boolean</span></span>|<span data-ttu-id="3256a-202">管理者の同意を得て、外部 MDM からのトークン管理を許可します。</span><span class="sxs-lookup"><span data-stu-id="3256a-202">Admin consent to allow claiming token management from external MDM.</span></span>|
|<span data-ttu-id="3256a-203">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3256a-203">roleScopeTagIds</span></span>|<span data-ttu-id="3256a-204">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3256a-204">String collection</span></span>|<span data-ttu-id="3256a-205">このエンティティに割り当てられているロールスコープタグ Id。</span><span class="sxs-lookup"><span data-stu-id="3256a-205">Role Scope Tags IDs assigned to this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3256a-206">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3256a-206">Relationships</span></span>
<span data-ttu-id="3256a-207">なし</span><span class="sxs-lookup"><span data-stu-id="3256a-207">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3256a-208">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3256a-208">JSON Representation</span></span>
<span data-ttu-id="3256a-209">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3256a-209">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String",
  "dataSharingConsentGranted": true,
  "displayName": "String",
  "locationName": "String",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```





