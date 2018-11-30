---
title: mobileApp リソースの種類
description: Intune モバイル アプリの基本プロパティを含む抽象クラスです。
ms.openlocfilehash: 1c3c573d0802cd937cdb44d9a2fdacf5cdbc6e56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073007"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="14cf8-103">mobileApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14cf8-103">mobileApp resource type</span></span>

> <span data-ttu-id="14cf8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14cf8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14cf8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14cf8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14cf8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="14cf8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14cf8-107">Intune モバイル アプリの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="14cf8-107">An abstract class containing the base properties for Intune mobile apps.</span></span>
## <a name="methods"></a><span data-ttu-id="14cf8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="14cf8-108">Methods</span></span>
|<span data-ttu-id="14cf8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="14cf8-109">Method</span></span>|<span data-ttu-id="14cf8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="14cf8-110">Return Type</span></span>|<span data-ttu-id="14cf8-111">説明</span><span class="sxs-lookup"><span data-stu-id="14cf8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="14cf8-112">mobileApps のリスト</span><span class="sxs-lookup"><span data-stu-id="14cf8-112">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="14cf8-113">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="14cf8-113">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="14cf8-114">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="14cf8-114">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="14cf8-115">MobileApp の取得</span><span class="sxs-lookup"><span data-stu-id="14cf8-115">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="14cf8-116">mobileApp</span><span class="sxs-lookup"><span data-stu-id="14cf8-116">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="14cf8-117">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="14cf8-117">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="14cf8-118">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="14cf8-118">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="14cf8-119">なし</span><span class="sxs-lookup"><span data-stu-id="14cf8-119">None</span></span>|<span data-ttu-id="14cf8-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="14cf8-120">Not yet documented</span></span>|
|[<span data-ttu-id="14cf8-121">getMobileAppCount 関数</span><span class="sxs-lookup"><span data-stu-id="14cf8-121">getMobileAppCount function</span></span>](../api/intune-apps-mobileapp-getmobileappcount.md)|<span data-ttu-id="14cf8-122">Int64</span><span class="sxs-lookup"><span data-stu-id="14cf8-122">Int64</span></span>|<span data-ttu-id="14cf8-123">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="14cf8-123">Not yet documented</span></span>|
|[<span data-ttu-id="14cf8-124">getTopMobileApps 関数</span><span class="sxs-lookup"><span data-stu-id="14cf8-124">getTopMobileApps function</span></span>](../api/intune-apps-mobileapp-gettopmobileapps.md)|<span data-ttu-id="14cf8-125">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="14cf8-125">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="14cf8-126">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="14cf8-126">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="14cf8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14cf8-127">Properties</span></span>
|<span data-ttu-id="14cf8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14cf8-128">Property</span></span>|<span data-ttu-id="14cf8-129">型</span><span class="sxs-lookup"><span data-stu-id="14cf8-129">Type</span></span>|<span data-ttu-id="14cf8-130">説明</span><span class="sxs-lookup"><span data-stu-id="14cf8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14cf8-131">id</span><span class="sxs-lookup"><span data-stu-id="14cf8-131">id</span></span>|<span data-ttu-id="14cf8-132">String</span><span class="sxs-lookup"><span data-stu-id="14cf8-132">String</span></span>|<span data-ttu-id="14cf8-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="14cf8-133">Key of the entity.</span></span>|
|<span data-ttu-id="14cf8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="14cf8-134">displayName</span></span>|<span data-ttu-id="14cf8-135">String</span><span class="sxs-lookup"><span data-stu-id="14cf8-135">String</span></span>|<span data-ttu-id="14cf8-136">管理者が提供またはインポートしたアプリのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="14cf8-136">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="14cf8-137">説明</span><span class="sxs-lookup"><span data-stu-id="14cf8-137">description</span></span>|<span data-ttu-id="14cf8-138">String</span><span class="sxs-lookup"><span data-stu-id="14cf8-138">String</span></span>|<span data-ttu-id="14cf8-139">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="14cf8-139">The description of the app.</span></span>|
|<span data-ttu-id="14cf8-140">publisher</span><span class="sxs-lookup"><span data-stu-id="14cf8-140">publisher</span></span>|<span data-ttu-id="14cf8-141">String</span><span class="sxs-lookup"><span data-stu-id="14cf8-141">String</span></span>|<span data-ttu-id="14cf8-142">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="14cf8-142">The publisher of the app.</span></span>|
|<span data-ttu-id="14cf8-143">largeIcon</span><span class="sxs-lookup"><span data-stu-id="14cf8-143">largeIcon</span></span>|[<span data-ttu-id="14cf8-144">mimeContent</span><span class="sxs-lookup"><span data-stu-id="14cf8-144">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="14cf8-145">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="14cf8-145">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="14cf8-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14cf8-146">createdDateTime</span></span>|<span data-ttu-id="14cf8-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14cf8-147">DateTimeOffset</span></span>|<span data-ttu-id="14cf8-148">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="14cf8-148">The date and time the app was created.</span></span>|
|<span data-ttu-id="14cf8-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14cf8-149">lastModifiedDateTime</span></span>|<span data-ttu-id="14cf8-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14cf8-150">DateTimeOffset</span></span>|<span data-ttu-id="14cf8-151">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="14cf8-151">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="14cf8-152">isFeatured</span><span class="sxs-lookup"><span data-stu-id="14cf8-152">isFeatured</span></span>|<span data-ttu-id="14cf8-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="14cf8-153">Boolean</span></span>|<span data-ttu-id="14cf8-154">アプリが管理者のおすすめとしてマークされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="14cf8-154">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="14cf8-155">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="14cf8-155">privacyInformationUrl</span></span>|<span data-ttu-id="14cf8-156">String</span><span class="sxs-lookup"><span data-stu-id="14cf8-156">String</span></span>|<span data-ttu-id="14cf8-157">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="14cf8-157">The privacy statement Url.</span></span>|
|<span data-ttu-id="14cf8-158">informationUrl</span><span class="sxs-lookup"><span data-stu-id="14cf8-158">informationUrl</span></span>|<span data-ttu-id="14cf8-159">String</span><span class="sxs-lookup"><span data-stu-id="14cf8-159">String</span></span>|<span data-ttu-id="14cf8-160">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="14cf8-160">The more information Url.</span></span>|
|<span data-ttu-id="14cf8-161">owner</span><span class="sxs-lookup"><span data-stu-id="14cf8-161">owner</span></span>|<span data-ttu-id="14cf8-162">String</span><span class="sxs-lookup"><span data-stu-id="14cf8-162">String</span></span>|<span data-ttu-id="14cf8-163">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="14cf8-163">The owner of the app.</span></span>|
|<span data-ttu-id="14cf8-164">developer</span><span class="sxs-lookup"><span data-stu-id="14cf8-164">developer</span></span>|<span data-ttu-id="14cf8-165">String</span><span class="sxs-lookup"><span data-stu-id="14cf8-165">String</span></span>|<span data-ttu-id="14cf8-166">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="14cf8-166">The developer of the app.</span></span>|
|<span data-ttu-id="14cf8-167">notes</span><span class="sxs-lookup"><span data-stu-id="14cf8-167">notes</span></span>|<span data-ttu-id="14cf8-168">String</span><span class="sxs-lookup"><span data-stu-id="14cf8-168">String</span></span>|<span data-ttu-id="14cf8-169">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="14cf8-169">Notes for the app.</span></span>|
|<span data-ttu-id="14cf8-170">uploadState</span><span class="sxs-lookup"><span data-stu-id="14cf8-170">uploadState</span></span>|<span data-ttu-id="14cf8-171">Int32</span><span class="sxs-lookup"><span data-stu-id="14cf8-171">Int32</span></span>|<span data-ttu-id="14cf8-172">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="14cf8-172">The upload state.</span></span>|
|<span data-ttu-id="14cf8-173">publishingState</span><span class="sxs-lookup"><span data-stu-id="14cf8-173">publishingState</span></span>|[<span data-ttu-id="14cf8-174">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="14cf8-174">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="14cf8-175">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="14cf8-175">The publishing state for the app.</span></span> <span data-ttu-id="14cf8-176">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="14cf8-176">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="14cf8-177">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="14cf8-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14cf8-178">関係</span><span class="sxs-lookup"><span data-stu-id="14cf8-178">Relationships</span></span>
|<span data-ttu-id="14cf8-179">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="14cf8-179">Relationship</span></span>|<span data-ttu-id="14cf8-180">型</span><span class="sxs-lookup"><span data-stu-id="14cf8-180">Type</span></span>|<span data-ttu-id="14cf8-181">説明</span><span class="sxs-lookup"><span data-stu-id="14cf8-181">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14cf8-182">categories</span><span class="sxs-lookup"><span data-stu-id="14cf8-182">categories</span></span>|<span data-ttu-id="14cf8-183">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="14cf8-183">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="14cf8-184">このアプリのカテゴリのリストです。</span><span class="sxs-lookup"><span data-stu-id="14cf8-184">The list of categories for this app.</span></span>|
|<span data-ttu-id="14cf8-185">assignments</span><span class="sxs-lookup"><span data-stu-id="14cf8-185">assignments</span></span>|<span data-ttu-id="14cf8-186">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="14cf8-186">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="14cf8-187">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="14cf8-187">The list of group assignments for this mobile app.</span></span>|
|<span data-ttu-id="14cf8-188">installSummary</span><span class="sxs-lookup"><span data-stu-id="14cf8-188">installSummary</span></span>|[<span data-ttu-id="14cf8-189">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="14cf8-189">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="14cf8-190">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="14cf8-190">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="14cf8-191">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="14cf8-191">deviceStatuses</span></span>|<span data-ttu-id="14cf8-192">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="14cf8-192">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="14cf8-193">このモバイル アプリケーションのインストール状況の一覧です。</span><span class="sxs-lookup"><span data-stu-id="14cf8-193">The list of installation states for this mobile app.</span></span>|
|<span data-ttu-id="14cf8-194">userStatuses</span><span class="sxs-lookup"><span data-stu-id="14cf8-194">userStatuses</span></span>|<span data-ttu-id="14cf8-195">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="14cf8-195">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="14cf8-196">このモバイル アプリケーションのインストール状況の一覧です。</span><span class="sxs-lookup"><span data-stu-id="14cf8-196">The list of installation states for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14cf8-197">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14cf8-197">JSON Representation</span></span>
<span data-ttu-id="14cf8-198">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="14cf8-198">Here is a JSON representation of the resource.</span></span>
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
  "publishingState": "String"
}
```





