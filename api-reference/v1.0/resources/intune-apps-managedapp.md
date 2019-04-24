---
title: managedApp リソースの種類
description: Intune アプリ保護ポリシーで管理できるアプリの、プロパティと継承済みプロパティを含む抽象クラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9260766a41920794c3842bdb0898c14cbd12357a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585434"
---
# <a name="managedapp-resource-type"></a><span data-ttu-id="f3834-103">managedApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3834-103">managedApp resource type</span></span>

> <span data-ttu-id="f3834-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3834-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3834-105">Intune アプリ保護ポリシーで管理できるアプリの、プロパティと継承済みプロパティを含む抽象クラス。</span><span class="sxs-lookup"><span data-stu-id="f3834-105">Abstract class that contains properties and inherited properties for apps that you can manage with an Intune app protection policy.</span></span>


<span data-ttu-id="f3834-106">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f3834-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f3834-107">Methods</span></span>
|<span data-ttu-id="f3834-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f3834-108">Method</span></span>|<span data-ttu-id="f3834-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f3834-109">Return Type</span></span>|<span data-ttu-id="f3834-110">説明</span><span class="sxs-lookup"><span data-stu-id="f3834-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3834-111">managedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="f3834-111">List managedApps</span></span>](../api/intune-apps-managedapp-list.md)|<span data-ttu-id="f3834-112">[managedApp](../resources/intune-apps-managedapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f3834-112">[managedApp](../resources/intune-apps-managedapp.md) collection</span></span>|<span data-ttu-id="f3834-113">[managedApp](../resources/intune-apps-managedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f3834-113">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>|
|[<span data-ttu-id="f3834-114">managedApp の取得</span><span class="sxs-lookup"><span data-stu-id="f3834-114">Get managedApp</span></span>](../api/intune-apps-managedapp-get.md)|[<span data-ttu-id="f3834-115">managedApp</span><span class="sxs-lookup"><span data-stu-id="f3834-115">managedApp</span></span>](../resources/intune-apps-managedapp.md)|<span data-ttu-id="f3834-116">[managedApp](../resources/intune-apps-managedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f3834-116">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3834-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3834-117">Properties</span></span>
|<span data-ttu-id="f3834-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3834-118">Property</span></span>|<span data-ttu-id="f3834-119">型</span><span class="sxs-lookup"><span data-stu-id="f3834-119">Type</span></span>|<span data-ttu-id="f3834-120">説明</span><span class="sxs-lookup"><span data-stu-id="f3834-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3834-121">id</span><span class="sxs-lookup"><span data-stu-id="f3834-121">id</span></span>|<span data-ttu-id="f3834-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f3834-122">String</span></span>|<span data-ttu-id="f3834-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f3834-123">Key of the entity.</span></span> <span data-ttu-id="f3834-124">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-125">displayName</span><span class="sxs-lookup"><span data-stu-id="f3834-125">displayName</span></span>|<span data-ttu-id="f3834-126">String</span><span class="sxs-lookup"><span data-stu-id="f3834-126">String</span></span>|<span data-ttu-id="f3834-127">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f3834-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f3834-128">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-129">説明</span><span class="sxs-lookup"><span data-stu-id="f3834-129">description</span></span>|<span data-ttu-id="f3834-130">String</span><span class="sxs-lookup"><span data-stu-id="f3834-130">String</span></span>|<span data-ttu-id="f3834-131">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f3834-131">The description of the app.</span></span> <span data-ttu-id="f3834-132">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-133">publisher</span><span class="sxs-lookup"><span data-stu-id="f3834-133">publisher</span></span>|<span data-ttu-id="f3834-134">String</span><span class="sxs-lookup"><span data-stu-id="f3834-134">String</span></span>|<span data-ttu-id="f3834-135">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f3834-135">The publisher of the app.</span></span> <span data-ttu-id="f3834-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f3834-137">largeIcon</span></span>|[<span data-ttu-id="f3834-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f3834-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f3834-139">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="f3834-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f3834-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3834-141">createdDateTime</span></span>|<span data-ttu-id="f3834-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3834-142">DateTimeOffset</span></span>|<span data-ttu-id="f3834-143">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f3834-143">The date and time the app was created.</span></span> <span data-ttu-id="f3834-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3834-145">lastModifiedDateTime</span></span>|<span data-ttu-id="f3834-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3834-146">DateTimeOffset</span></span>|<span data-ttu-id="f3834-147">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f3834-147">The date and time the app was last modified.</span></span> <span data-ttu-id="f3834-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f3834-149">isFeatured</span></span>|<span data-ttu-id="f3834-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3834-150">Boolean</span></span>|<span data-ttu-id="f3834-151">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f3834-152">privacyInformationUrl</span></span>|<span data-ttu-id="f3834-153">String</span><span class="sxs-lookup"><span data-stu-id="f3834-153">String</span></span>|<span data-ttu-id="f3834-154">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f3834-154">The privacy statement Url.</span></span> <span data-ttu-id="f3834-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f3834-156">informationUrl</span></span>|<span data-ttu-id="f3834-157">String</span><span class="sxs-lookup"><span data-stu-id="f3834-157">String</span></span>|<span data-ttu-id="f3834-158">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f3834-158">The more information Url.</span></span> <span data-ttu-id="f3834-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-160">owner</span><span class="sxs-lookup"><span data-stu-id="f3834-160">owner</span></span>|<span data-ttu-id="f3834-161">String</span><span class="sxs-lookup"><span data-stu-id="f3834-161">String</span></span>|<span data-ttu-id="f3834-162">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f3834-162">The owner of the app.</span></span> <span data-ttu-id="f3834-163">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-164">developer</span><span class="sxs-lookup"><span data-stu-id="f3834-164">developer</span></span>|<span data-ttu-id="f3834-165">String</span><span class="sxs-lookup"><span data-stu-id="f3834-165">String</span></span>|<span data-ttu-id="f3834-166">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f3834-166">The developer of the app.</span></span> <span data-ttu-id="f3834-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-168">notes</span><span class="sxs-lookup"><span data-stu-id="f3834-168">notes</span></span>|<span data-ttu-id="f3834-169">String</span><span class="sxs-lookup"><span data-stu-id="f3834-169">String</span></span>|<span data-ttu-id="f3834-170">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f3834-170">Notes for the app.</span></span> <span data-ttu-id="f3834-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="f3834-172">publishingState</span></span>|[<span data-ttu-id="f3834-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f3834-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f3834-174">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f3834-174">The publishing state for the app.</span></span> <span data-ttu-id="f3834-175">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f3834-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f3834-176">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f3834-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f3834-177">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f3834-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f3834-178">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f3834-178">appAvailability</span></span>|[<span data-ttu-id="f3834-179">managedappavailability</span><span class="sxs-lookup"><span data-stu-id="f3834-179">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f3834-180">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="f3834-180">The Application's availability.</span></span> <span data-ttu-id="f3834-181">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="f3834-181">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f3834-182">version</span><span class="sxs-lookup"><span data-stu-id="f3834-182">version</span></span>|<span data-ttu-id="f3834-183">String</span><span class="sxs-lookup"><span data-stu-id="f3834-183">String</span></span>|<span data-ttu-id="f3834-184">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f3834-184">The Application's version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3834-185">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3834-185">Relationships</span></span>
|<span data-ttu-id="f3834-186">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3834-186">Relationship</span></span>|<span data-ttu-id="f3834-187">型</span><span class="sxs-lookup"><span data-stu-id="f3834-187">Type</span></span>|<span data-ttu-id="f3834-188">説明</span><span class="sxs-lookup"><span data-stu-id="f3834-188">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3834-189">categories</span><span class="sxs-lookup"><span data-stu-id="f3834-189">categories</span></span>|<span data-ttu-id="f3834-190">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f3834-190">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="f3834-191">このアプリのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="f3834-191">The list of categories for this app.</span></span> <span data-ttu-id="f3834-192">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f3834-193">assignments</span><span class="sxs-lookup"><span data-stu-id="f3834-193">assignments</span></span>|<span data-ttu-id="f3834-194">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f3834-194">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="f3834-195">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="f3834-195">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="f3834-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f3834-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f3834-197">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3834-197">JSON Representation</span></span>
<span data-ttu-id="f3834-198">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3834-198">Here is a JSON representation of the resource.</span></span>
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



