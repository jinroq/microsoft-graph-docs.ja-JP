---
title: mobileLobApp リソースの種類
description: ビジネス アプリのすべての携帯電話回線のプロパティを含む抽象基本クラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f07738bff5187cb209db5090c593a38684986ca5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028911"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="e1365-103">mobileLobApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1365-103">mobileLobApp resource type</span></span>

> <span data-ttu-id="e1365-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1365-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1365-105">ビジネス アプリのすべての携帯電話回線のプロパティを含む抽象基本クラス。</span><span class="sxs-lookup"><span data-stu-id="e1365-105">An abstract base class containing properties for all mobile line of business apps.</span></span>


<span data-ttu-id="e1365-106">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e1365-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1365-107">Methods</span></span>
|<span data-ttu-id="e1365-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1365-108">Method</span></span>|<span data-ttu-id="e1365-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e1365-109">Return Type</span></span>|<span data-ttu-id="e1365-110">説明</span><span class="sxs-lookup"><span data-stu-id="e1365-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e1365-111">mobileLobApps のリスト</span><span class="sxs-lookup"><span data-stu-id="e1365-111">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="e1365-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1365-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="e1365-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e1365-113">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="e1365-114">mobileLobApp の取得</span><span class="sxs-lookup"><span data-stu-id="e1365-114">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="e1365-115">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="e1365-115">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="e1365-116">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e1365-116">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1365-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1365-117">Properties</span></span>
|<span data-ttu-id="e1365-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1365-118">Property</span></span>|<span data-ttu-id="e1365-119">型</span><span class="sxs-lookup"><span data-stu-id="e1365-119">Type</span></span>|<span data-ttu-id="e1365-120">説明</span><span class="sxs-lookup"><span data-stu-id="e1365-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1365-121">id</span><span class="sxs-lookup"><span data-stu-id="e1365-121">id</span></span>|<span data-ttu-id="e1365-122">文字列</span><span class="sxs-lookup"><span data-stu-id="e1365-122">String</span></span>|<span data-ttu-id="e1365-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e1365-123">Key of the entity.</span></span> <span data-ttu-id="e1365-124">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-125">displayName</span><span class="sxs-lookup"><span data-stu-id="e1365-125">displayName</span></span>|<span data-ttu-id="e1365-126">文字列</span><span class="sxs-lookup"><span data-stu-id="e1365-126">String</span></span>|<span data-ttu-id="e1365-127">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e1365-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e1365-128">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-129">description</span><span class="sxs-lookup"><span data-stu-id="e1365-129">description</span></span>|<span data-ttu-id="e1365-130">String</span><span class="sxs-lookup"><span data-stu-id="e1365-130">String</span></span>|<span data-ttu-id="e1365-131">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e1365-131">The description of the app.</span></span> <span data-ttu-id="e1365-132">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-133">publisher</span><span class="sxs-lookup"><span data-stu-id="e1365-133">publisher</span></span>|<span data-ttu-id="e1365-134">String</span><span class="sxs-lookup"><span data-stu-id="e1365-134">String</span></span>|<span data-ttu-id="e1365-135">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e1365-135">The publisher of the app.</span></span> <span data-ttu-id="e1365-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e1365-137">largeIcon</span></span>|[<span data-ttu-id="e1365-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e1365-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e1365-139">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="e1365-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e1365-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1365-141">createdDateTime</span></span>|<span data-ttu-id="e1365-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1365-142">DateTimeOffset</span></span>|<span data-ttu-id="e1365-143">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e1365-143">The date and time the app was created.</span></span> <span data-ttu-id="e1365-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e1365-145">lastModifiedDateTime</span></span>|<span data-ttu-id="e1365-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1365-146">DateTimeOffset</span></span>|<span data-ttu-id="e1365-147">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e1365-147">The date and time the app was last modified.</span></span> <span data-ttu-id="e1365-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e1365-149">isFeatured</span></span>|<span data-ttu-id="e1365-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1365-150">Boolean</span></span>|<span data-ttu-id="e1365-151">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e1365-152">privacyInformationUrl</span></span>|<span data-ttu-id="e1365-153">String</span><span class="sxs-lookup"><span data-stu-id="e1365-153">String</span></span>|<span data-ttu-id="e1365-154">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e1365-154">The privacy statement Url.</span></span> <span data-ttu-id="e1365-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e1365-156">informationUrl</span></span>|<span data-ttu-id="e1365-157">String</span><span class="sxs-lookup"><span data-stu-id="e1365-157">String</span></span>|<span data-ttu-id="e1365-158">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e1365-158">The more information Url.</span></span> <span data-ttu-id="e1365-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-160">owner</span><span class="sxs-lookup"><span data-stu-id="e1365-160">owner</span></span>|<span data-ttu-id="e1365-161">String</span><span class="sxs-lookup"><span data-stu-id="e1365-161">String</span></span>|<span data-ttu-id="e1365-162">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e1365-162">The owner of the app.</span></span> <span data-ttu-id="e1365-163">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-164">developer</span><span class="sxs-lookup"><span data-stu-id="e1365-164">developer</span></span>|<span data-ttu-id="e1365-165">String</span><span class="sxs-lookup"><span data-stu-id="e1365-165">String</span></span>|<span data-ttu-id="e1365-166">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e1365-166">The developer of the app.</span></span> <span data-ttu-id="e1365-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-168">notes</span><span class="sxs-lookup"><span data-stu-id="e1365-168">notes</span></span>|<span data-ttu-id="e1365-169">String</span><span class="sxs-lookup"><span data-stu-id="e1365-169">String</span></span>|<span data-ttu-id="e1365-170">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e1365-170">Notes for the app.</span></span> <span data-ttu-id="e1365-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="e1365-172">publishingState</span></span>|[<span data-ttu-id="e1365-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e1365-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e1365-174">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e1365-174">The publishing state for the app.</span></span> <span data-ttu-id="e1365-175">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e1365-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e1365-176">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e1365-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e1365-177">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e1365-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e1365-178">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="e1365-178">committedContentVersion</span></span>|<span data-ttu-id="e1365-179">String</span><span class="sxs-lookup"><span data-stu-id="e1365-179">String</span></span>|<span data-ttu-id="e1365-180">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e1365-180">The internal committed content version.</span></span>|
|<span data-ttu-id="e1365-181">fileName</span><span class="sxs-lookup"><span data-stu-id="e1365-181">fileName</span></span>|<span data-ttu-id="e1365-182">String</span><span class="sxs-lookup"><span data-stu-id="e1365-182">String</span></span>|<span data-ttu-id="e1365-183">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="e1365-183">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="e1365-184">size</span><span class="sxs-lookup"><span data-stu-id="e1365-184">size</span></span>|<span data-ttu-id="e1365-185">Int64</span><span class="sxs-lookup"><span data-stu-id="e1365-185">Int64</span></span>|<span data-ttu-id="e1365-186">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="e1365-186">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1365-187">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1365-187">Relationships</span></span>
|<span data-ttu-id="e1365-188">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1365-188">Relationship</span></span>|<span data-ttu-id="e1365-189">型</span><span class="sxs-lookup"><span data-stu-id="e1365-189">Type</span></span>|<span data-ttu-id="e1365-190">説明</span><span class="sxs-lookup"><span data-stu-id="e1365-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1365-191">categories</span><span class="sxs-lookup"><span data-stu-id="e1365-191">categories</span></span>|<span data-ttu-id="e1365-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1365-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="e1365-193">このアプリのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="e1365-193">The list of categories for this app.</span></span> <span data-ttu-id="e1365-194">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-194">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-195">assignments</span><span class="sxs-lookup"><span data-stu-id="e1365-195">assignments</span></span>|<span data-ttu-id="e1365-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1365-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="e1365-197">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="e1365-197">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="e1365-198">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e1365-198">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e1365-199">contentVersions</span><span class="sxs-lookup"><span data-stu-id="e1365-199">contentVersions</span></span>|<span data-ttu-id="e1365-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e1365-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="e1365-201">このアプリのコンテンツのバージョンのリスト。</span><span class="sxs-lookup"><span data-stu-id="e1365-201">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1365-202">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1365-202">JSON Representation</span></span>
<span data-ttu-id="e1365-203">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e1365-203">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileLobApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileLobApp",
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
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024
}
```



