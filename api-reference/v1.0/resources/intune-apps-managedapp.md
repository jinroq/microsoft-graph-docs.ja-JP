---
title: managedApp リソースの種類
description: Intune アプリ保護ポリシーで管理できるアプリの、プロパティと継承済みプロパティを含む抽象クラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2ce11682142fccbf77890eda5f56c0cbe2325803
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029065"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="8700f-103">managedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8700f-103">managedApp resource type</span></span>

> <span data-ttu-id="8700f-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8700f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8700f-105">Intune アプリ保護ポリシーで管理できるアプリの、プロパティと継承済みプロパティを含む抽象クラス。</span><span class="sxs-lookup"><span data-stu-id="8700f-105">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="8700f-106">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8700f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8700f-107">Methods</span></span>
|<span data-ttu-id="8700f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8700f-108">Method</span></span>|<span data-ttu-id="8700f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8700f-109">Return Type</span></span>|<span data-ttu-id="8700f-110">説明</span><span class="sxs-lookup"><span data-stu-id="8700f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8700f-111">managedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="8700f-111">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="8700f-112">[managedApp](../resources/intune-apps-managedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8700f-112">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="8700f-113">[managedApp](../resources/intune-apps-managedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8700f-113">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="8700f-114">managedApp の取得</span><span class="sxs-lookup"><span data-stu-id="8700f-114">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="8700f-115">managedApp</span><span class="sxs-lookup"><span data-stu-id="8700f-115">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="8700f-116">[managedApp](../resources/intune-apps-managedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8700f-116">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8700f-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8700f-117">Properties</span></span>
|<span data-ttu-id="8700f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8700f-118">Property</span></span>|<span data-ttu-id="8700f-119">型</span><span class="sxs-lookup"><span data-stu-id="8700f-119">Type</span></span>|<span data-ttu-id="8700f-120">説明</span><span class="sxs-lookup"><span data-stu-id="8700f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8700f-121">id</span><span class="sxs-lookup"><span data-stu-id="8700f-121">id</span></span>|<span data-ttu-id="8700f-122">文字列</span><span class="sxs-lookup"><span data-stu-id="8700f-122">String</span></span>|<span data-ttu-id="8700f-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8700f-123">Key of the entity.</span></span> <span data-ttu-id="8700f-124">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-125">displayName</span><span class="sxs-lookup"><span data-stu-id="8700f-125">displayName</span></span>|<span data-ttu-id="8700f-126">文字列</span><span class="sxs-lookup"><span data-stu-id="8700f-126">String</span></span>|<span data-ttu-id="8700f-127">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="8700f-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8700f-128">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-129">description</span><span class="sxs-lookup"><span data-stu-id="8700f-129">description</span></span>|<span data-ttu-id="8700f-130">String</span><span class="sxs-lookup"><span data-stu-id="8700f-130">String</span></span>|<span data-ttu-id="8700f-131">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="8700f-131">The description of the app.</span></span> <span data-ttu-id="8700f-132">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-133">publisher</span><span class="sxs-lookup"><span data-stu-id="8700f-133">publisher</span></span>|<span data-ttu-id="8700f-134">String</span><span class="sxs-lookup"><span data-stu-id="8700f-134">String</span></span>|<span data-ttu-id="8700f-135">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="8700f-135">The publisher of the app.</span></span> <span data-ttu-id="8700f-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8700f-137">largeIcon</span></span>|[<span data-ttu-id="8700f-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8700f-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8700f-139">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="8700f-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8700f-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8700f-141">createdDateTime</span></span>|<span data-ttu-id="8700f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8700f-142">DateTimeOffset</span></span>|<span data-ttu-id="8700f-143">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="8700f-143">The date and time the app was created.</span></span> <span data-ttu-id="8700f-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8700f-145">lastModifiedDateTime</span></span>|<span data-ttu-id="8700f-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8700f-146">DateTimeOffset</span></span>|<span data-ttu-id="8700f-147">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8700f-147">The date and time the app was last modified.</span></span> <span data-ttu-id="8700f-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8700f-149">isFeatured</span></span>|<span data-ttu-id="8700f-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="8700f-150">Boolean</span></span>|<span data-ttu-id="8700f-151">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8700f-152">privacyInformationUrl</span></span>|<span data-ttu-id="8700f-153">String</span><span class="sxs-lookup"><span data-stu-id="8700f-153">String</span></span>|<span data-ttu-id="8700f-154">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="8700f-154">The privacy statement Url.</span></span> <span data-ttu-id="8700f-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8700f-156">informationUrl</span></span>|<span data-ttu-id="8700f-157">String</span><span class="sxs-lookup"><span data-stu-id="8700f-157">String</span></span>|<span data-ttu-id="8700f-158">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="8700f-158">The more information Url.</span></span> <span data-ttu-id="8700f-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-160">owner</span><span class="sxs-lookup"><span data-stu-id="8700f-160">owner</span></span>|<span data-ttu-id="8700f-161">String</span><span class="sxs-lookup"><span data-stu-id="8700f-161">String</span></span>|<span data-ttu-id="8700f-162">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="8700f-162">The owner of the app.</span></span> <span data-ttu-id="8700f-163">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-164">developer</span><span class="sxs-lookup"><span data-stu-id="8700f-164">developer</span></span>|<span data-ttu-id="8700f-165">String</span><span class="sxs-lookup"><span data-stu-id="8700f-165">String</span></span>|<span data-ttu-id="8700f-166">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="8700f-166">The developer of the app.</span></span> <span data-ttu-id="8700f-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-168">notes</span><span class="sxs-lookup"><span data-stu-id="8700f-168">notes</span></span>|<span data-ttu-id="8700f-169">String</span><span class="sxs-lookup"><span data-stu-id="8700f-169">String</span></span>|<span data-ttu-id="8700f-170">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="8700f-170">Notes for the app.</span></span> <span data-ttu-id="8700f-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="8700f-172">publishingState</span></span>|[<span data-ttu-id="8700f-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8700f-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8700f-174">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="8700f-174">The publishing state for the app.</span></span> <span data-ttu-id="8700f-175">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="8700f-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8700f-176">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8700f-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8700f-177">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="8700f-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8700f-178">appAvailability</span><span class="sxs-lookup"><span data-stu-id="8700f-178">appAvailability</span></span>|[<span data-ttu-id="8700f-179">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="8700f-179">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="8700f-180">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="8700f-180">The Application's availability.</span></span> <span data-ttu-id="8700f-181">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="8700f-181">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="8700f-182">version</span><span class="sxs-lookup"><span data-stu-id="8700f-182">version</span></span>|<span data-ttu-id="8700f-183">String</span><span class="sxs-lookup"><span data-stu-id="8700f-183">String</span></span>|<span data-ttu-id="8700f-184">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="8700f-184">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8700f-185">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8700f-185">Relationships</span></span>
|<span data-ttu-id="8700f-186">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8700f-186">Relationship</span></span>|<span data-ttu-id="8700f-187">型</span><span class="sxs-lookup"><span data-stu-id="8700f-187">Type</span></span>|<span data-ttu-id="8700f-188">説明</span><span class="sxs-lookup"><span data-stu-id="8700f-188">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8700f-189">categories</span><span class="sxs-lookup"><span data-stu-id="8700f-189">categories</span></span>|<span data-ttu-id="8700f-190">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8700f-190">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="8700f-191">このアプリのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="8700f-191">The list of categories for this app.</span></span> <span data-ttu-id="8700f-192">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8700f-193">assignments</span><span class="sxs-lookup"><span data-stu-id="8700f-193">assignments</span></span>|<span data-ttu-id="8700f-194">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8700f-194">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="8700f-195">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="8700f-195">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="8700f-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8700f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8700f-197">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8700f-197">JSON Representation</span></span>
<span data-ttu-id="8700f-198">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8700f-198">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedApp",
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
  "publishingState": "String",
  "appAvailability": "String",
  "version": "String"
}
```



