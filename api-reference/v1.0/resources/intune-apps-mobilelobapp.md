---
title: mobileLobApp リソースの種類
description: ビジネス アプリのすべての携帯電話回線のプロパティを含む抽象基本クラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc00842f3525f48fb172d6fd9616b18ac7085a91
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260754"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="97e76-103">mobileLobApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97e76-103">mobileLobApp resource type</span></span>

> <span data-ttu-id="97e76-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97e76-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97e76-105">ビジネス アプリのすべての携帯電話回線のプロパティを含む抽象基本クラス。</span><span class="sxs-lookup"><span data-stu-id="97e76-105">An abstract base class containing properties for all mobile line of business apps.</span></span>


<span data-ttu-id="97e76-106">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="97e76-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="97e76-107">Methods</span></span>
|<span data-ttu-id="97e76-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="97e76-108">Method</span></span>|<span data-ttu-id="97e76-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="97e76-109">Return Type</span></span>|<span data-ttu-id="97e76-110">説明</span><span class="sxs-lookup"><span data-stu-id="97e76-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="97e76-111">mobileLobApps のリスト</span><span class="sxs-lookup"><span data-stu-id="97e76-111">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="97e76-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="97e76-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="97e76-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="97e76-113">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="97e76-114">mobileLobApp の取得</span><span class="sxs-lookup"><span data-stu-id="97e76-114">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="97e76-115">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="97e76-115">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="97e76-116">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="97e76-116">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="97e76-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97e76-117">Properties</span></span>
|<span data-ttu-id="97e76-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97e76-118">Property</span></span>|<span data-ttu-id="97e76-119">型</span><span class="sxs-lookup"><span data-stu-id="97e76-119">Type</span></span>|<span data-ttu-id="97e76-120">説明</span><span class="sxs-lookup"><span data-stu-id="97e76-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97e76-121">id</span><span class="sxs-lookup"><span data-stu-id="97e76-121">id</span></span>|<span data-ttu-id="97e76-122">文字列</span><span class="sxs-lookup"><span data-stu-id="97e76-122">String</span></span>|<span data-ttu-id="97e76-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="97e76-123">Key of the entity.</span></span> <span data-ttu-id="97e76-124">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-125">displayName</span><span class="sxs-lookup"><span data-stu-id="97e76-125">displayName</span></span>|<span data-ttu-id="97e76-126">String</span><span class="sxs-lookup"><span data-stu-id="97e76-126">String</span></span>|<span data-ttu-id="97e76-127">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="97e76-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="97e76-128">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-129">説明</span><span class="sxs-lookup"><span data-stu-id="97e76-129">description</span></span>|<span data-ttu-id="97e76-130">文字列</span><span class="sxs-lookup"><span data-stu-id="97e76-130">String</span></span>|<span data-ttu-id="97e76-131">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="97e76-131">The description of the app.</span></span> <span data-ttu-id="97e76-132">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-133">publisher</span><span class="sxs-lookup"><span data-stu-id="97e76-133">publisher</span></span>|<span data-ttu-id="97e76-134">String</span><span class="sxs-lookup"><span data-stu-id="97e76-134">String</span></span>|<span data-ttu-id="97e76-135">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="97e76-135">The publisher of the app.</span></span> <span data-ttu-id="97e76-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="97e76-137">largeIcon</span></span>|[<span data-ttu-id="97e76-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="97e76-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="97e76-139">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="97e76-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="97e76-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="97e76-141">createdDateTime</span></span>|<span data-ttu-id="97e76-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e76-142">DateTimeOffset</span></span>|<span data-ttu-id="97e76-143">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="97e76-143">The date and time the app was created.</span></span> <span data-ttu-id="97e76-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="97e76-145">lastModifiedDateTime</span></span>|<span data-ttu-id="97e76-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e76-146">DateTimeOffset</span></span>|<span data-ttu-id="97e76-147">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="97e76-147">The date and time the app was last modified.</span></span> <span data-ttu-id="97e76-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="97e76-149">isFeatured</span></span>|<span data-ttu-id="97e76-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="97e76-150">Boolean</span></span>|<span data-ttu-id="97e76-151">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="97e76-152">privacyInformationUrl</span></span>|<span data-ttu-id="97e76-153">String</span><span class="sxs-lookup"><span data-stu-id="97e76-153">String</span></span>|<span data-ttu-id="97e76-154">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="97e76-154">The privacy statement Url.</span></span> <span data-ttu-id="97e76-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="97e76-156">informationUrl</span></span>|<span data-ttu-id="97e76-157">String</span><span class="sxs-lookup"><span data-stu-id="97e76-157">String</span></span>|<span data-ttu-id="97e76-158">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="97e76-158">The more information Url.</span></span> <span data-ttu-id="97e76-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-160">owner</span><span class="sxs-lookup"><span data-stu-id="97e76-160">owner</span></span>|<span data-ttu-id="97e76-161">String</span><span class="sxs-lookup"><span data-stu-id="97e76-161">String</span></span>|<span data-ttu-id="97e76-162">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="97e76-162">The owner of the app.</span></span> <span data-ttu-id="97e76-163">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-164">developer</span><span class="sxs-lookup"><span data-stu-id="97e76-164">developer</span></span>|<span data-ttu-id="97e76-165">String</span><span class="sxs-lookup"><span data-stu-id="97e76-165">String</span></span>|<span data-ttu-id="97e76-166">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="97e76-166">The developer of the app.</span></span> <span data-ttu-id="97e76-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-168">notes</span><span class="sxs-lookup"><span data-stu-id="97e76-168">notes</span></span>|<span data-ttu-id="97e76-169">String</span><span class="sxs-lookup"><span data-stu-id="97e76-169">String</span></span>|<span data-ttu-id="97e76-170">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="97e76-170">Notes for the app.</span></span> <span data-ttu-id="97e76-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="97e76-172">publishingState</span></span>|[<span data-ttu-id="97e76-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="97e76-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="97e76-174">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="97e76-174">The publishing state for the app.</span></span> <span data-ttu-id="97e76-175">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="97e76-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="97e76-176">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="97e76-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="97e76-177">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="97e76-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="97e76-178">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="97e76-178">committedContentVersion</span></span>|<span data-ttu-id="97e76-179">String</span><span class="sxs-lookup"><span data-stu-id="97e76-179">String</span></span>|<span data-ttu-id="97e76-180">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="97e76-180">The internal committed content version.</span></span>|
|<span data-ttu-id="97e76-181">fileName</span><span class="sxs-lookup"><span data-stu-id="97e76-181">fileName</span></span>|<span data-ttu-id="97e76-182">String</span><span class="sxs-lookup"><span data-stu-id="97e76-182">String</span></span>|<span data-ttu-id="97e76-183">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="97e76-183">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="97e76-184">size</span><span class="sxs-lookup"><span data-stu-id="97e76-184">size</span></span>|<span data-ttu-id="97e76-185">Int64</span><span class="sxs-lookup"><span data-stu-id="97e76-185">Int64</span></span>|<span data-ttu-id="97e76-186">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="97e76-186">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="97e76-187">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97e76-187">Relationships</span></span>
|<span data-ttu-id="97e76-188">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97e76-188">Relationship</span></span>|<span data-ttu-id="97e76-189">型</span><span class="sxs-lookup"><span data-stu-id="97e76-189">Type</span></span>|<span data-ttu-id="97e76-190">説明</span><span class="sxs-lookup"><span data-stu-id="97e76-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97e76-191">categories</span><span class="sxs-lookup"><span data-stu-id="97e76-191">categories</span></span>|<span data-ttu-id="97e76-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="97e76-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="97e76-193">このアプリのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="97e76-193">The list of categories for this app.</span></span> <span data-ttu-id="97e76-194">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-194">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-195">assignments</span><span class="sxs-lookup"><span data-stu-id="97e76-195">assignments</span></span>|<span data-ttu-id="97e76-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="97e76-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="97e76-197">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="97e76-197">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="97e76-198">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="97e76-198">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="97e76-199">contentVersions</span><span class="sxs-lookup"><span data-stu-id="97e76-199">contentVersions</span></span>|<span data-ttu-id="97e76-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="97e76-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="97e76-201">このアプリのコンテンツのバージョンのリスト。</span><span class="sxs-lookup"><span data-stu-id="97e76-201">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97e76-202">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="97e76-202">JSON Representation</span></span>
<span data-ttu-id="97e76-203">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="97e76-203">Here is a JSON representation of the resource.</span></span>
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



