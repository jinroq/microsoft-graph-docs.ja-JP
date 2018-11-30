---
title: webApp リソースの種類
description: Web アプリのプロパティと継承されるプロパティを含みます。
ms.openlocfilehash: ff661063c0cdc5fe6c41b5e93d57487a1236ca03
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024214"
---
# <a name="webapp-resource-type"></a><span data-ttu-id="d37a8-103">webApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d37a8-103">webApp resource type</span></span>

> <span data-ttu-id="d37a8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d37a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d37a8-105">Web アプリのプロパティと継承されるプロパティを含みます。</span><span class="sxs-lookup"><span data-stu-id="d37a8-105">Contains properties and inherited properties for web apps.</span></span>

<span data-ttu-id="d37a8-106">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d37a8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d37a8-107">Methods</span></span>
|<span data-ttu-id="d37a8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d37a8-108">Method</span></span>|<span data-ttu-id="d37a8-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d37a8-109">Return Type</span></span>|<span data-ttu-id="d37a8-110">説明</span><span class="sxs-lookup"><span data-stu-id="d37a8-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d37a8-111">webApps のリスト</span><span class="sxs-lookup"><span data-stu-id="d37a8-111">List webApps</span></span>](../api/intune-apps-webapp-list.md)|<span data-ttu-id="d37a8-112">[webApp](../resources/intune-apps-webapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d37a8-112">[webApp](../resources/intune-apps-webapp.md) collection</span></span>|<span data-ttu-id="d37a8-113">[webApp](../resources/intune-apps-webapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d37a8-113">List properties and relationships of the [webApp](../resources/intune-apps-webapp.md) objects.</span></span>|
|[<span data-ttu-id="d37a8-114">webApp の取得</span><span class="sxs-lookup"><span data-stu-id="d37a8-114">Get webApp</span></span>](../api/intune-apps-webapp-get.md)|[<span data-ttu-id="d37a8-115">webApp</span><span class="sxs-lookup"><span data-stu-id="d37a8-115">webApp</span></span>](../resources/intune-apps-webapp.md)|<span data-ttu-id="d37a8-116">[webApp](../resources/intune-apps-webapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d37a8-116">Read properties and relationships of the [webApp](../resources/intune-apps-webapp.md) object.</span></span>|
|[<span data-ttu-id="d37a8-117">webApp の作成</span><span class="sxs-lookup"><span data-stu-id="d37a8-117">Create webApp</span></span>](../api/intune-apps-webapp-create.md)|[<span data-ttu-id="d37a8-118">webApp</span><span class="sxs-lookup"><span data-stu-id="d37a8-118">webApp</span></span>](../resources/intune-apps-webapp.md)|<span data-ttu-id="d37a8-119">新しい [webApp](../resources/intune-apps-webapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d37a8-119">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>|
|[<span data-ttu-id="d37a8-120">webApp の削除</span><span class="sxs-lookup"><span data-stu-id="d37a8-120">Delete webApp</span></span>](../api/intune-apps-webapp-delete.md)|<span data-ttu-id="d37a8-121">なし</span><span class="sxs-lookup"><span data-stu-id="d37a8-121">None</span></span>|<span data-ttu-id="d37a8-122">[webApp](../resources/intune-apps-webapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d37a8-122">Deletes a [webApp](../resources/intune-apps-webapp.md).</span></span>|
|[<span data-ttu-id="d37a8-123">webApp の更新</span><span class="sxs-lookup"><span data-stu-id="d37a8-123">Update webApp</span></span>](../api/intune-apps-webapp-update.md)|[<span data-ttu-id="d37a8-124">webApp</span><span class="sxs-lookup"><span data-stu-id="d37a8-124">webApp</span></span>](../resources/intune-apps-webapp.md)|<span data-ttu-id="d37a8-125">[webApp](../resources/intune-apps-webapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d37a8-125">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d37a8-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d37a8-126">Properties</span></span>
|<span data-ttu-id="d37a8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d37a8-127">Property</span></span>|<span data-ttu-id="d37a8-128">型</span><span class="sxs-lookup"><span data-stu-id="d37a8-128">Type</span></span>|<span data-ttu-id="d37a8-129">説明</span><span class="sxs-lookup"><span data-stu-id="d37a8-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d37a8-130">id</span><span class="sxs-lookup"><span data-stu-id="d37a8-130">id</span></span>|<span data-ttu-id="d37a8-131">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-131">String</span></span>|<span data-ttu-id="d37a8-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d37a8-132">Key of the entity.</span></span> <span data-ttu-id="d37a8-133">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-133">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="d37a8-134">displayName</span></span>|<span data-ttu-id="d37a8-135">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-135">String</span></span>|<span data-ttu-id="d37a8-136">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="d37a8-136">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d37a8-137">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-137">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-138">説明</span><span class="sxs-lookup"><span data-stu-id="d37a8-138">description</span></span>|<span data-ttu-id="d37a8-139">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-139">String</span></span>|<span data-ttu-id="d37a8-140">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="d37a8-140">The description of the app.</span></span> <span data-ttu-id="d37a8-141">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-141">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-142">publisher</span><span class="sxs-lookup"><span data-stu-id="d37a8-142">publisher</span></span>|<span data-ttu-id="d37a8-143">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-143">String</span></span>|<span data-ttu-id="d37a8-144">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="d37a8-144">The publisher of the app.</span></span> <span data-ttu-id="d37a8-145">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-145">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-146">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d37a8-146">largeIcon</span></span>|[<span data-ttu-id="d37a8-147">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d37a8-147">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d37a8-148">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="d37a8-148">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d37a8-149">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-149">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d37a8-150">createdDateTime</span></span>|<span data-ttu-id="d37a8-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37a8-151">DateTimeOffset</span></span>|<span data-ttu-id="d37a8-152">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d37a8-152">The date and time the app was created.</span></span> <span data-ttu-id="d37a8-153">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-153">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-154">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d37a8-154">lastModifiedDateTime</span></span>|<span data-ttu-id="d37a8-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d37a8-155">DateTimeOffset</span></span>|<span data-ttu-id="d37a8-156">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d37a8-156">The date and time the app was last modified.</span></span> <span data-ttu-id="d37a8-157">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-157">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-158">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d37a8-158">isFeatured</span></span>|<span data-ttu-id="d37a8-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="d37a8-159">Boolean</span></span>|<span data-ttu-id="d37a8-160">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-160">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-161">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d37a8-161">privacyInformationUrl</span></span>|<span data-ttu-id="d37a8-162">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-162">String</span></span>|<span data-ttu-id="d37a8-163">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="d37a8-163">The privacy statement Url.</span></span> <span data-ttu-id="d37a8-164">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d37a8-165">informationUrl</span></span>|<span data-ttu-id="d37a8-166">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-166">String</span></span>|<span data-ttu-id="d37a8-167">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="d37a8-167">The more information Url.</span></span> <span data-ttu-id="d37a8-168">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-169">owner</span><span class="sxs-lookup"><span data-stu-id="d37a8-169">owner</span></span>|<span data-ttu-id="d37a8-170">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-170">String</span></span>|<span data-ttu-id="d37a8-171">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="d37a8-171">The owner of the app.</span></span> <span data-ttu-id="d37a8-172">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-172">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-173">developer</span><span class="sxs-lookup"><span data-stu-id="d37a8-173">developer</span></span>|<span data-ttu-id="d37a8-174">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-174">String</span></span>|<span data-ttu-id="d37a8-175">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="d37a8-175">The developer of the app.</span></span> <span data-ttu-id="d37a8-176">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-177">notes</span><span class="sxs-lookup"><span data-stu-id="d37a8-177">notes</span></span>|<span data-ttu-id="d37a8-178">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-178">String</span></span>|<span data-ttu-id="d37a8-179">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="d37a8-179">Notes for the app.</span></span> <span data-ttu-id="d37a8-180">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-180">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-181">publishingState</span><span class="sxs-lookup"><span data-stu-id="d37a8-181">publishingState</span></span>|[<span data-ttu-id="d37a8-182">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d37a8-182">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d37a8-183">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="d37a8-183">The publishing state for the app.</span></span> <span data-ttu-id="d37a8-184">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="d37a8-184">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d37a8-185">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d37a8-185">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d37a8-186">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="d37a8-186">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d37a8-187">appUrl</span><span class="sxs-lookup"><span data-stu-id="d37a8-187">appUrl</span></span>|<span data-ttu-id="d37a8-188">String</span><span class="sxs-lookup"><span data-stu-id="d37a8-188">String</span></span>|<span data-ttu-id="d37a8-189">Web アプリの URL。</span><span class="sxs-lookup"><span data-stu-id="d37a8-189">The web app URL.</span></span>|
|<span data-ttu-id="d37a8-190">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="d37a8-190">useManagedBrowser</span></span>|<span data-ttu-id="d37a8-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="d37a8-191">Boolean</span></span>|<span data-ttu-id="d37a8-192">管理対象のブラウザーを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d37a8-192">Whether or not to use managed browser.</span></span> <span data-ttu-id="d37a8-193">このプロパティは、Android と iOS のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="d37a8-193">This property is only applicable for Android and IOS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d37a8-194">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d37a8-194">Relationships</span></span>
|<span data-ttu-id="d37a8-195">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d37a8-195">Relationship</span></span>|<span data-ttu-id="d37a8-196">型</span><span class="sxs-lookup"><span data-stu-id="d37a8-196">Type</span></span>|<span data-ttu-id="d37a8-197">説明</span><span class="sxs-lookup"><span data-stu-id="d37a8-197">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d37a8-198">categories</span><span class="sxs-lookup"><span data-stu-id="d37a8-198">categories</span></span>|<span data-ttu-id="d37a8-199">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d37a8-199">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="d37a8-200">このアプリのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="d37a8-200">The list of categories for this app.</span></span> <span data-ttu-id="d37a8-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d37a8-202">assignments</span><span class="sxs-lookup"><span data-stu-id="d37a8-202">assignments</span></span>|<span data-ttu-id="d37a8-203">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d37a8-203">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="d37a8-204">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="d37a8-204">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="d37a8-205">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d37a8-205">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d37a8-206">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d37a8-206">JSON Representation</span></span>
<span data-ttu-id="d37a8-207">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d37a8-207">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.webApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "String",
  "useManagedBrowser": true
}
```


