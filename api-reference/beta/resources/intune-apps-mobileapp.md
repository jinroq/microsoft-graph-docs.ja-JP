---
title: mobileApp リソースの種類
description: Intune モバイル アプリの基本プロパティを含む抽象クラスです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0e1e68ede0e4beef689d753aca9af8292812d64c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408335"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="e9f91-103">mobileApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9f91-103">mobileApp resource type</span></span>

> <span data-ttu-id="e9f91-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e9f91-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e9f91-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e9f91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9f91-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e9f91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9f91-107">Intune モバイル アプリの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="e9f91-107">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="e9f91-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e9f91-108">Methods</span></span>
|<span data-ttu-id="e9f91-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e9f91-109">Method</span></span>|<span data-ttu-id="e9f91-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e9f91-110">Return Type</span></span>|<span data-ttu-id="e9f91-111">説明</span><span class="sxs-lookup"><span data-stu-id="e9f91-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e9f91-112">mobileApps のリスト</span><span class="sxs-lookup"><span data-stu-id="e9f91-112">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="e9f91-113">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e9f91-113">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="e9f91-114">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e9f91-114">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="e9f91-115">MobileApp の取得</span><span class="sxs-lookup"><span data-stu-id="e9f91-115">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="e9f91-116">mobileApp</span><span class="sxs-lookup"><span data-stu-id="e9f91-116">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="e9f91-117">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e9f91-117">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="e9f91-118">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="e9f91-118">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="e9f91-119">なし</span><span class="sxs-lookup"><span data-stu-id="e9f91-119">None</span></span>|<span data-ttu-id="e9f91-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e9f91-120">Not yet documented</span></span>|
|[<span data-ttu-id="e9f91-121">getMobileAppCount 関数</span><span class="sxs-lookup"><span data-stu-id="e9f91-121">getMobileAppCount function</span></span>](../api/intune-apps-mobileapp-getmobileappcount.md)|<span data-ttu-id="e9f91-122">Int64</span><span class="sxs-lookup"><span data-stu-id="e9f91-122">Int64</span></span>|<span data-ttu-id="e9f91-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e9f91-123">Not yet documented</span></span>|
|[<span data-ttu-id="e9f91-124">getTopMobileApps 関数</span><span class="sxs-lookup"><span data-stu-id="e9f91-124">getTopMobileApps function</span></span>](../api/intune-apps-mobileapp-gettopmobileapps.md)|<span data-ttu-id="e9f91-125">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e9f91-125">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="e9f91-126">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e9f91-126">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e9f91-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9f91-127">Properties</span></span>
|<span data-ttu-id="e9f91-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9f91-128">Property</span></span>|<span data-ttu-id="e9f91-129">型</span><span class="sxs-lookup"><span data-stu-id="e9f91-129">Type</span></span>|<span data-ttu-id="e9f91-130">説明</span><span class="sxs-lookup"><span data-stu-id="e9f91-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9f91-131">id</span><span class="sxs-lookup"><span data-stu-id="e9f91-131">id</span></span>|<span data-ttu-id="e9f91-132">String</span><span class="sxs-lookup"><span data-stu-id="e9f91-132">String</span></span>|<span data-ttu-id="e9f91-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e9f91-133">Key of the entity.</span></span>|
|<span data-ttu-id="e9f91-134">displayName</span><span class="sxs-lookup"><span data-stu-id="e9f91-134">displayName</span></span>|<span data-ttu-id="e9f91-135">String</span><span class="sxs-lookup"><span data-stu-id="e9f91-135">String</span></span>|<span data-ttu-id="e9f91-136">管理者が提供またはインポートしたアプリのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="e9f91-136">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="e9f91-137">説明</span><span class="sxs-lookup"><span data-stu-id="e9f91-137">description</span></span>|<span data-ttu-id="e9f91-138">String</span><span class="sxs-lookup"><span data-stu-id="e9f91-138">String</span></span>|<span data-ttu-id="e9f91-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e9f91-139">The description of the app.</span></span>|
|<span data-ttu-id="e9f91-140">publisher</span><span class="sxs-lookup"><span data-stu-id="e9f91-140">publisher</span></span>|<span data-ttu-id="e9f91-141">String</span><span class="sxs-lookup"><span data-stu-id="e9f91-141">String</span></span>|<span data-ttu-id="e9f91-142">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e9f91-142">The publisher of the app.</span></span>|
|<span data-ttu-id="e9f91-143">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e9f91-143">largeIcon</span></span>|[<span data-ttu-id="e9f91-144">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e9f91-144">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e9f91-145">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="e9f91-145">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="e9f91-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9f91-146">createdDateTime</span></span>|<span data-ttu-id="e9f91-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9f91-147">DateTimeOffset</span></span>|<span data-ttu-id="e9f91-148">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e9f91-148">The date and time the app was created.</span></span>|
|<span data-ttu-id="e9f91-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9f91-149">lastModifiedDateTime</span></span>|<span data-ttu-id="e9f91-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9f91-150">DateTimeOffset</span></span>|<span data-ttu-id="e9f91-151">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e9f91-151">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="e9f91-152">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e9f91-152">isFeatured</span></span>|<span data-ttu-id="e9f91-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9f91-153">Boolean</span></span>|<span data-ttu-id="e9f91-154">アプリが管理者のおすすめとしてマークされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e9f91-154">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="e9f91-155">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e9f91-155">privacyInformationUrl</span></span>|<span data-ttu-id="e9f91-156">String</span><span class="sxs-lookup"><span data-stu-id="e9f91-156">String</span></span>|<span data-ttu-id="e9f91-157">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e9f91-157">The privacy statement Url.</span></span>|
|<span data-ttu-id="e9f91-158">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e9f91-158">informationUrl</span></span>|<span data-ttu-id="e9f91-159">String</span><span class="sxs-lookup"><span data-stu-id="e9f91-159">String</span></span>|<span data-ttu-id="e9f91-160">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e9f91-160">The more information Url.</span></span>|
|<span data-ttu-id="e9f91-161">owner</span><span class="sxs-lookup"><span data-stu-id="e9f91-161">owner</span></span>|<span data-ttu-id="e9f91-162">String</span><span class="sxs-lookup"><span data-stu-id="e9f91-162">String</span></span>|<span data-ttu-id="e9f91-163">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e9f91-163">The owner of the app.</span></span>|
|<span data-ttu-id="e9f91-164">developer</span><span class="sxs-lookup"><span data-stu-id="e9f91-164">developer</span></span>|<span data-ttu-id="e9f91-165">String</span><span class="sxs-lookup"><span data-stu-id="e9f91-165">String</span></span>|<span data-ttu-id="e9f91-166">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e9f91-166">The developer of the app.</span></span>|
|<span data-ttu-id="e9f91-167">notes</span><span class="sxs-lookup"><span data-stu-id="e9f91-167">notes</span></span>|<span data-ttu-id="e9f91-168">String</span><span class="sxs-lookup"><span data-stu-id="e9f91-168">String</span></span>|<span data-ttu-id="e9f91-169">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e9f91-169">Notes for the app.</span></span>|
|<span data-ttu-id="e9f91-170">uploadState</span><span class="sxs-lookup"><span data-stu-id="e9f91-170">uploadState</span></span>|<span data-ttu-id="e9f91-171">Int32</span><span class="sxs-lookup"><span data-stu-id="e9f91-171">Int32</span></span>|<span data-ttu-id="e9f91-172">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="e9f91-172">The upload state.</span></span>|
|<span data-ttu-id="e9f91-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="e9f91-173">publishingState</span></span>|[<span data-ttu-id="e9f91-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e9f91-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e9f91-175">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e9f91-175">The publishing state for the app.</span></span> <span data-ttu-id="e9f91-176">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e9f91-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e9f91-177">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e9f91-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e9f91-178">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e9f91-178">isAssigned</span></span>|<span data-ttu-id="e9f91-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9f91-179">Boolean</span></span>|<span data-ttu-id="e9f91-180">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="e9f91-180">The value indicating whether the app is assigned to at least one group.</span></span>|
|<span data-ttu-id="e9f91-181">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e9f91-181">roleScopeTagIds</span></span>|<span data-ttu-id="e9f91-182">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e9f91-182">String collection</span></span>|<span data-ttu-id="e9f91-183">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="e9f91-183">List of scope tag ids for this mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9f91-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e9f91-184">Relationships</span></span>
|<span data-ttu-id="e9f91-185">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e9f91-185">Relationship</span></span>|<span data-ttu-id="e9f91-186">型</span><span class="sxs-lookup"><span data-stu-id="e9f91-186">Type</span></span>|<span data-ttu-id="e9f91-187">説明</span><span class="sxs-lookup"><span data-stu-id="e9f91-187">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9f91-188">categories</span><span class="sxs-lookup"><span data-stu-id="e9f91-188">categories</span></span>|<span data-ttu-id="e9f91-189">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e9f91-189">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="e9f91-190">このアプリのカテゴリのリストです。</span><span class="sxs-lookup"><span data-stu-id="e9f91-190">The list of categories for this app.</span></span>|
|<span data-ttu-id="e9f91-191">assignments</span><span class="sxs-lookup"><span data-stu-id="e9f91-191">assignments</span></span>|<span data-ttu-id="e9f91-192">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e9f91-192">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="e9f91-193">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="e9f91-193">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="e9f91-194">installSummary</span><span class="sxs-lookup"><span data-stu-id="e9f91-194">installSummary</span></span>|[<span data-ttu-id="e9f91-195">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e9f91-195">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="e9f91-196">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="e9f91-196">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="e9f91-197">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="e9f91-197">deviceStatuses</span></span>|<span data-ttu-id="e9f91-198">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e9f91-198">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="e9f91-199">このモバイル アプリケーションのインストール状況の一覧です。</span><span class="sxs-lookup"><span data-stu-id="e9f91-199">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="e9f91-200">userStatuses</span><span class="sxs-lookup"><span data-stu-id="e9f91-200">userStatuses</span></span>|<span data-ttu-id="e9f91-201">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e9f91-201">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="e9f91-202">このモバイル アプリケーションのインストール状況の一覧です。</span><span class="sxs-lookup"><span data-stu-id="e9f91-202">The list of installation states for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9f91-203">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9f91-203">JSON Representation</span></span>
<span data-ttu-id="e9f91-204">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e9f91-204">Here is a JSON representation of the resource.</span></span>
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
  ]
}
```




