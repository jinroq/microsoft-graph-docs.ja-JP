---
title: mobileApp リソースの種類
description: Intune モバイル アプリの基本プロパティを含む抽象クラスです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d937495f44fc511b260ee6feb322043bcf9cff7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986138"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="7098f-103">mobileApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7098f-103">mobileApp resource type</span></span>

> <span data-ttu-id="7098f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7098f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7098f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7098f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7098f-106">Intune モバイル アプリの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="7098f-106">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="7098f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="7098f-107">Methods</span></span>
|<span data-ttu-id="7098f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7098f-108">Method</span></span>|<span data-ttu-id="7098f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7098f-109">Return Type</span></span>|<span data-ttu-id="7098f-110">説明</span><span class="sxs-lookup"><span data-stu-id="7098f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7098f-111">mobileApps のリスト</span><span class="sxs-lookup"><span data-stu-id="7098f-111">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="7098f-112">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7098f-112">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="7098f-113">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7098f-113">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="7098f-114">MobileApp の取得</span><span class="sxs-lookup"><span data-stu-id="7098f-114">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="7098f-115">mobileApp</span><span class="sxs-lookup"><span data-stu-id="7098f-115">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="7098f-116">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7098f-116">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="7098f-117">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="7098f-117">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="7098f-118">なし</span><span class="sxs-lookup"><span data-stu-id="7098f-118">None</span></span>|<span data-ttu-id="7098f-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7098f-119">Not yet documented</span></span>|
|[<span data-ttu-id="7098f-120">getMobileAppCount 関数</span><span class="sxs-lookup"><span data-stu-id="7098f-120">getMobileAppCount function</span></span>](../api/intune-apps-mobileapp-getmobileappcount.md)|<span data-ttu-id="7098f-121">Int64</span><span class="sxs-lookup"><span data-stu-id="7098f-121">Int64</span></span>|<span data-ttu-id="7098f-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7098f-122">Not yet documented</span></span>|
|[<span data-ttu-id="7098f-123">getTopMobileApps 関数</span><span class="sxs-lookup"><span data-stu-id="7098f-123">getTopMobileApps function</span></span>](../api/intune-apps-mobileapp-gettopmobileapps.md)|<span data-ttu-id="7098f-124">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7098f-124">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="7098f-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7098f-125">Not yet documented</span></span>|
|[<span data-ttu-id="7098f-126">updateRelationships アクション</span><span class="sxs-lookup"><span data-stu-id="7098f-126">updateRelationships action</span></span>](../api/intune-apps-mobileapp-updaterelationships.md)|<span data-ttu-id="7098f-127">なし</span><span class="sxs-lookup"><span data-stu-id="7098f-127">None</span></span>|<span data-ttu-id="7098f-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7098f-128">Not yet documented</span></span>|
|[<span data-ttu-id="7098f-129">Getの Appstates 関数</span><span class="sxs-lookup"><span data-stu-id="7098f-129">getRelatedAppStates function</span></span>](../api/intune-apps-mobileapp-getrelatedappstates.md)|<span data-ttu-id="7098f-130">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7098f-130">[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection</span></span>|<span data-ttu-id="7098f-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7098f-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="7098f-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7098f-132">Properties</span></span>
|<span data-ttu-id="7098f-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7098f-133">Property</span></span>|<span data-ttu-id="7098f-134">型</span><span class="sxs-lookup"><span data-stu-id="7098f-134">Type</span></span>|<span data-ttu-id="7098f-135">説明</span><span class="sxs-lookup"><span data-stu-id="7098f-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7098f-136">id</span><span class="sxs-lookup"><span data-stu-id="7098f-136">id</span></span>|<span data-ttu-id="7098f-137">文字列</span><span class="sxs-lookup"><span data-stu-id="7098f-137">String</span></span>|<span data-ttu-id="7098f-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7098f-138">Key of the entity.</span></span>|
|<span data-ttu-id="7098f-139">displayName</span><span class="sxs-lookup"><span data-stu-id="7098f-139">displayName</span></span>|<span data-ttu-id="7098f-140">文字列</span><span class="sxs-lookup"><span data-stu-id="7098f-140">String</span></span>|<span data-ttu-id="7098f-141">管理者が提供またはインポートしたアプリのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="7098f-141">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="7098f-142">description</span><span class="sxs-lookup"><span data-stu-id="7098f-142">description</span></span>|<span data-ttu-id="7098f-143">String</span><span class="sxs-lookup"><span data-stu-id="7098f-143">String</span></span>|<span data-ttu-id="7098f-144">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7098f-144">The description of the app.</span></span>|
|<span data-ttu-id="7098f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7098f-145">publisher</span></span>|<span data-ttu-id="7098f-146">String</span><span class="sxs-lookup"><span data-stu-id="7098f-146">String</span></span>|<span data-ttu-id="7098f-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="7098f-147">The publisher of the app.</span></span>|
|<span data-ttu-id="7098f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7098f-148">largeIcon</span></span>|[<span data-ttu-id="7098f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7098f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7098f-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="7098f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="7098f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7098f-151">createdDateTime</span></span>|<span data-ttu-id="7098f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7098f-152">DateTimeOffset</span></span>|<span data-ttu-id="7098f-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7098f-153">The date and time the app was created.</span></span>|
|<span data-ttu-id="7098f-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7098f-154">lastModifiedDateTime</span></span>|<span data-ttu-id="7098f-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7098f-155">DateTimeOffset</span></span>|<span data-ttu-id="7098f-156">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="7098f-156">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="7098f-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7098f-157">isFeatured</span></span>|<span data-ttu-id="7098f-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="7098f-158">Boolean</span></span>|<span data-ttu-id="7098f-159">アプリが管理者のおすすめとしてマークされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7098f-159">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="7098f-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7098f-160">privacyInformationUrl</span></span>|<span data-ttu-id="7098f-161">String</span><span class="sxs-lookup"><span data-stu-id="7098f-161">String</span></span>|<span data-ttu-id="7098f-162">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="7098f-162">The privacy statement Url.</span></span>|
|<span data-ttu-id="7098f-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7098f-163">informationUrl</span></span>|<span data-ttu-id="7098f-164">String</span><span class="sxs-lookup"><span data-stu-id="7098f-164">String</span></span>|<span data-ttu-id="7098f-165">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="7098f-165">The more information Url.</span></span>|
|<span data-ttu-id="7098f-166">owner</span><span class="sxs-lookup"><span data-stu-id="7098f-166">owner</span></span>|<span data-ttu-id="7098f-167">String</span><span class="sxs-lookup"><span data-stu-id="7098f-167">String</span></span>|<span data-ttu-id="7098f-168">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="7098f-168">The owner of the app.</span></span>|
|<span data-ttu-id="7098f-169">developer</span><span class="sxs-lookup"><span data-stu-id="7098f-169">developer</span></span>|<span data-ttu-id="7098f-170">String</span><span class="sxs-lookup"><span data-stu-id="7098f-170">String</span></span>|<span data-ttu-id="7098f-171">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="7098f-171">The developer of the app.</span></span>|
|<span data-ttu-id="7098f-172">notes</span><span class="sxs-lookup"><span data-stu-id="7098f-172">notes</span></span>|<span data-ttu-id="7098f-173">String</span><span class="sxs-lookup"><span data-stu-id="7098f-173">String</span></span>|<span data-ttu-id="7098f-174">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="7098f-174">Notes for the app.</span></span>|
|<span data-ttu-id="7098f-175">uploadState</span><span class="sxs-lookup"><span data-stu-id="7098f-175">uploadState</span></span>|<span data-ttu-id="7098f-176">Int32</span><span class="sxs-lookup"><span data-stu-id="7098f-176">Int32</span></span>|<span data-ttu-id="7098f-177">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="7098f-177">The upload state.</span></span>|
|<span data-ttu-id="7098f-178">publishingState</span><span class="sxs-lookup"><span data-stu-id="7098f-178">publishingState</span></span>|[<span data-ttu-id="7098f-179">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7098f-179">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7098f-180">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="7098f-180">The publishing state for the app.</span></span> <span data-ttu-id="7098f-181">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="7098f-181">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7098f-182">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="7098f-182">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7098f-183">isAssigned</span><span class="sxs-lookup"><span data-stu-id="7098f-183">isAssigned</span></span>|<span data-ttu-id="7098f-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="7098f-184">Boolean</span></span>|<span data-ttu-id="7098f-185">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="7098f-185">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="7098f-186">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7098f-186">roleScopeTagIds</span></span>|<span data-ttu-id="7098f-187">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="7098f-187">String collection</span></span>|<span data-ttu-id="7098f-188">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="7098f-188">List of scope tag ids for this mobile app.</span></span>|
|<span data-ttu-id="7098f-189">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="7098f-189">dependentAppCount</span></span>|<span data-ttu-id="7098f-190">Int32</span><span class="sxs-lookup"><span data-stu-id="7098f-190">Int32</span></span>|<span data-ttu-id="7098f-191">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="7098f-191">The total number of dependencies the child app has.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7098f-192">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7098f-192">Relationships</span></span>
|<span data-ttu-id="7098f-193">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7098f-193">Relationship</span></span>|<span data-ttu-id="7098f-194">型</span><span class="sxs-lookup"><span data-stu-id="7098f-194">Type</span></span>|<span data-ttu-id="7098f-195">説明</span><span class="sxs-lookup"><span data-stu-id="7098f-195">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7098f-196">categories</span><span class="sxs-lookup"><span data-stu-id="7098f-196">categories</span></span>|<span data-ttu-id="7098f-197">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7098f-197">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="7098f-198">このアプリのカテゴリのリストです。</span><span class="sxs-lookup"><span data-stu-id="7098f-198">The list of categories for this app.</span></span>|
|<span data-ttu-id="7098f-199">assignments</span><span class="sxs-lookup"><span data-stu-id="7098f-199">assignments</span></span>|<span data-ttu-id="7098f-200">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7098f-200">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="7098f-201">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="7098f-201">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="7098f-202">installSummary</span><span class="sxs-lookup"><span data-stu-id="7098f-202">installSummary</span></span>|[<span data-ttu-id="7098f-203">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="7098f-203">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="7098f-204">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="7098f-204">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="7098f-205">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="7098f-205">deviceStatuses</span></span>|<span data-ttu-id="7098f-206">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7098f-206">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="7098f-207">このモバイルアプリのインストール状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="7098f-207">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="7098f-208">userStatuses</span><span class="sxs-lookup"><span data-stu-id="7098f-208">userStatuses</span></span>|<span data-ttu-id="7098f-209">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7098f-209">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="7098f-210">このモバイルアプリのインストール状態のリスト。</span><span class="sxs-lookup"><span data-stu-id="7098f-210">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="7098f-211">関連性</span><span class="sxs-lookup"><span data-stu-id="7098f-211">relationships</span></span>|<span data-ttu-id="7098f-212">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7098f-212">[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md) collection</span></span>|<span data-ttu-id="7098f-213">このモバイルアプリのリレーションシップのリスト。</span><span class="sxs-lookup"><span data-stu-id="7098f-213">List of relationships for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7098f-214">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7098f-214">JSON Representation</span></span>
<span data-ttu-id="7098f-215">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7098f-215">Here is a JSON representation of the resource.</span></span>
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





