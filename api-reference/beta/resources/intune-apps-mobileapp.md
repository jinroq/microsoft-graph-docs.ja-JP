---
title: mobileApp リソースの種類
description: Intune モバイル アプリの基本プロパティを含む抽象クラスです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e634a02afaabb945109aba93bb0a668124f7daba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364923"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="0a2a2-103">mobileApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a2a2-103">mobileApp resource type</span></span>

> <span data-ttu-id="0a2a2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a2a2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a2a2-106">Intune モバイル アプリの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="0a2a2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a2a2-107">Methods</span></span>
|<span data-ttu-id="0a2a2-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a2a2-108">Method</span></span>|<span data-ttu-id="0a2a2-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0a2a2-109">Return Type</span></span>|<span data-ttu-id="0a2a2-110">説明</span><span class="sxs-lookup"><span data-stu-id="0a2a2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0a2a2-111">mobileApps のリスト</span><span class="sxs-lookup"><span data-stu-id="0a2a2-111">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="0a2a2-112">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-112">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="0a2a2-113">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-113">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="0a2a2-114">MobileApp の取得</span><span class="sxs-lookup"><span data-stu-id="0a2a2-114">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="0a2a2-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="0a2a2-115">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="0a2a2-116">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-116">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="0a2a2-117">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="0a2a2-117">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="0a2a2-118">なし</span><span class="sxs-lookup"><span data-stu-id="0a2a2-118">None</span></span>|<span data-ttu-id="0a2a2-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0a2a2-119">Not yet documented</span></span>|
|[<span data-ttu-id="0a2a2-120">getMobileAppCount 関数</span><span class="sxs-lookup"><span data-stu-id="0a2a2-120">getMobileAppCount function</span></span>](../api/intune-apps-mobileapp-getmobileappcount.md)|<span data-ttu-id="0a2a2-121">Int64</span><span class="sxs-lookup"><span data-stu-id="0a2a2-121">Int64</span></span>|<span data-ttu-id="0a2a2-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0a2a2-122">Not yet documented</span></span>|
|[<span data-ttu-id="0a2a2-123">getTopMobileApps 関数</span><span class="sxs-lookup"><span data-stu-id="0a2a2-123">getTopMobileApps function</span></span>](../api/intune-apps-mobileapp-gettopmobileapps.md)|<span data-ttu-id="0a2a2-124">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-124">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="0a2a2-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0a2a2-125">Not yet documented</span></span>|
|[<span data-ttu-id="0a2a2-126">updateRelationships アクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-126">updateRelationships action</span></span>](../api/intune-apps-mobileapp-updaterelationships.md)|<span data-ttu-id="0a2a2-127">なし</span><span class="sxs-lookup"><span data-stu-id="0a2a2-127">None</span></span>|<span data-ttu-id="0a2a2-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0a2a2-128">Not yet documented</span></span>|
|[<span data-ttu-id="0a2a2-129">Getの Appstates 関数</span><span class="sxs-lookup"><span data-stu-id="0a2a2-129">getRelatedAppStates function</span></span>](../api/intune-apps-mobileapp-getrelatedappstates.md)|<span data-ttu-id="0a2a2-130">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-130">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection</span></span>|<span data-ttu-id="0a2a2-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0a2a2-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="0a2a2-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a2a2-132">Properties</span></span>
|<span data-ttu-id="0a2a2-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a2a2-133">Property</span></span>|<span data-ttu-id="0a2a2-134">型</span><span class="sxs-lookup"><span data-stu-id="0a2a2-134">Type</span></span>|<span data-ttu-id="0a2a2-135">説明</span><span class="sxs-lookup"><span data-stu-id="0a2a2-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a2a2-136">id</span><span class="sxs-lookup"><span data-stu-id="0a2a2-136">id</span></span>|<span data-ttu-id="0a2a2-137">文字列</span><span class="sxs-lookup"><span data-stu-id="0a2a2-137">String</span></span>|<span data-ttu-id="0a2a2-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-138">Key of the entity.</span></span>|
|<span data-ttu-id="0a2a2-139">displayName</span><span class="sxs-lookup"><span data-stu-id="0a2a2-139">displayName</span></span>|<span data-ttu-id="0a2a2-140">文字列</span><span class="sxs-lookup"><span data-stu-id="0a2a2-140">String</span></span>|<span data-ttu-id="0a2a2-141">管理者が提供またはインポートしたアプリのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-141">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="0a2a2-142">description</span><span class="sxs-lookup"><span data-stu-id="0a2a2-142">description</span></span>|<span data-ttu-id="0a2a2-143">String</span><span class="sxs-lookup"><span data-stu-id="0a2a2-143">String</span></span>|<span data-ttu-id="0a2a2-144">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-144">The description of the app.</span></span>|
|<span data-ttu-id="0a2a2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="0a2a2-145">publisher</span></span>|<span data-ttu-id="0a2a2-146">String</span><span class="sxs-lookup"><span data-stu-id="0a2a2-146">String</span></span>|<span data-ttu-id="0a2a2-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-147">The publisher of the app.</span></span>|
|<span data-ttu-id="0a2a2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0a2a2-148">largeIcon</span></span>|[<span data-ttu-id="0a2a2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0a2a2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0a2a2-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="0a2a2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0a2a2-151">createdDateTime</span></span>|<span data-ttu-id="0a2a2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a2a2-152">DateTimeOffset</span></span>|<span data-ttu-id="0a2a2-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-153">The date and time the app was created.</span></span>|
|<span data-ttu-id="0a2a2-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0a2a2-154">lastModifiedDateTime</span></span>|<span data-ttu-id="0a2a2-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0a2a2-155">DateTimeOffset</span></span>|<span data-ttu-id="0a2a2-156">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-156">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="0a2a2-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0a2a2-157">isFeatured</span></span>|<span data-ttu-id="0a2a2-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2a2-158">Boolean</span></span>|<span data-ttu-id="0a2a2-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-159">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="0a2a2-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0a2a2-160">privacyInformationUrl</span></span>|<span data-ttu-id="0a2a2-161">String</span><span class="sxs-lookup"><span data-stu-id="0a2a2-161">String</span></span>|<span data-ttu-id="0a2a2-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-162">The privacy statement Url.</span></span>|
|<span data-ttu-id="0a2a2-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0a2a2-163">informationUrl</span></span>|<span data-ttu-id="0a2a2-164">String</span><span class="sxs-lookup"><span data-stu-id="0a2a2-164">String</span></span>|<span data-ttu-id="0a2a2-165">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-165">The more information Url.</span></span>|
|<span data-ttu-id="0a2a2-166">owner</span><span class="sxs-lookup"><span data-stu-id="0a2a2-166">owner</span></span>|<span data-ttu-id="0a2a2-167">String</span><span class="sxs-lookup"><span data-stu-id="0a2a2-167">String</span></span>|<span data-ttu-id="0a2a2-168">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-168">The owner of the app.</span></span>|
|<span data-ttu-id="0a2a2-169">developer</span><span class="sxs-lookup"><span data-stu-id="0a2a2-169">developer</span></span>|<span data-ttu-id="0a2a2-170">String</span><span class="sxs-lookup"><span data-stu-id="0a2a2-170">String</span></span>|<span data-ttu-id="0a2a2-171">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-171">The developer of the app.</span></span>|
|<span data-ttu-id="0a2a2-172">notes</span><span class="sxs-lookup"><span data-stu-id="0a2a2-172">notes</span></span>|<span data-ttu-id="0a2a2-173">String</span><span class="sxs-lookup"><span data-stu-id="0a2a2-173">String</span></span>|<span data-ttu-id="0a2a2-174">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-174">Notes for the app.</span></span>|
|<span data-ttu-id="0a2a2-175">uploadState</span><span class="sxs-lookup"><span data-stu-id="0a2a2-175">uploadState</span></span>|<span data-ttu-id="0a2a2-176">Int32</span><span class="sxs-lookup"><span data-stu-id="0a2a2-176">Int32</span></span>|<span data-ttu-id="0a2a2-177">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-177">The upload state.</span></span>|
|<span data-ttu-id="0a2a2-178">publishingState</span><span class="sxs-lookup"><span data-stu-id="0a2a2-178">publishingState</span></span>|[<span data-ttu-id="0a2a2-179">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0a2a2-179">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0a2a2-180">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-180">The publishing state for the app.</span></span> <span data-ttu-id="0a2a2-181">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-181">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0a2a2-182">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-182">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0a2a2-183">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0a2a2-183">isAssigned</span></span>|<span data-ttu-id="0a2a2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a2a2-184">Boolean</span></span>|<span data-ttu-id="0a2a2-185">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-185">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="0a2a2-186">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0a2a2-186">roleScopeTagIds</span></span>|<span data-ttu-id="0a2a2-187">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-187">String collection</span></span>|<span data-ttu-id="0a2a2-188">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-188">List of scope tag ids for this mobile app.</span></span>|
|<span data-ttu-id="0a2a2-189">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0a2a2-189">dependentAppCount</span></span>|<span data-ttu-id="0a2a2-190">Int32</span><span class="sxs-lookup"><span data-stu-id="0a2a2-190">Int32</span></span>|<span data-ttu-id="0a2a2-191">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-191">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a2a2-192">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a2a2-192">Relationships</span></span>
|<span data-ttu-id="0a2a2-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a2a2-193">Relationship</span></span>|<span data-ttu-id="0a2a2-194">型</span><span class="sxs-lookup"><span data-stu-id="0a2a2-194">Type</span></span>|<span data-ttu-id="0a2a2-195">説明</span><span class="sxs-lookup"><span data-stu-id="0a2a2-195">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a2a2-196">categories</span><span class="sxs-lookup"><span data-stu-id="0a2a2-196">categories</span></span>|<span data-ttu-id="0a2a2-197">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-197">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="0a2a2-198">このアプリのカテゴリのリストです。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-198">The list of categories for this app.</span></span>|
|<span data-ttu-id="0a2a2-199">assignments</span><span class="sxs-lookup"><span data-stu-id="0a2a2-199">assignments</span></span>|<span data-ttu-id="0a2a2-200">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-200">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="0a2a2-201">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-201">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="0a2a2-202">installSummary</span><span class="sxs-lookup"><span data-stu-id="0a2a2-202">installSummary</span></span>|[<span data-ttu-id="0a2a2-203">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="0a2a2-203">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="0a2a2-204">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-204">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="0a2a2-205">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0a2a2-205">deviceStatuses</span></span>|<span data-ttu-id="0a2a2-206">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-206">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="0a2a2-207">このモバイルアプリのインストール状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-207">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="0a2a2-208">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0a2a2-208">userStatuses</span></span>|<span data-ttu-id="0a2a2-209">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-209">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="0a2a2-210">このモバイルアプリのインストール状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-210">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="0a2a2-211">関連性</span><span class="sxs-lookup"><span data-stu-id="0a2a2-211">relationships</span></span>|<span data-ttu-id="0a2a2-212">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0a2a2-212">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="0a2a2-213">このモバイルアプリのリレーションシップのリスト。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-213">List of relationships for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0a2a2-214">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a2a2-214">JSON Representation</span></span>
<span data-ttu-id="0a2a2-215">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a2a2-215">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "isAssigned": true,
  "roleScopeTagIds": [
    "String"
  ],
  "dependentAppCount": 1024
}
```



