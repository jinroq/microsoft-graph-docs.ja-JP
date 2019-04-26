---
title: mobileLobApp リソースの種類
description: ビジネス アプリのすべての携帯電話回線のプロパティを含む抽象基本クラス。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc00842f3525f48fb172d6fd9616b18ac7085a91
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557909"
---
# <a name="mobilelobapp-resource-type"></a><span data-ttu-id="c5e4c-103">mobileLobApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5e4c-103">mobileLobApp resource type</span></span>

> <span data-ttu-id="c5e4c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5e4c-105">ビジネス アプリのすべての携帯電話回線のプロパティを含む抽象基本クラス。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-105">An abstract base class containing properties for all mobile line of business apps.</span></span>


<span data-ttu-id="c5e4c-106">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-106">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c5e4c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c5e4c-107">Methods</span></span>
|<span data-ttu-id="c5e4c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c5e4c-108">Method</span></span>|<span data-ttu-id="c5e4c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c5e4c-109">Return Type</span></span>|<span data-ttu-id="c5e4c-110">説明</span><span class="sxs-lookup"><span data-stu-id="c5e4c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5e4c-111">mobileLobApps のリスト</span><span class="sxs-lookup"><span data-stu-id="c5e4c-111">List mobileLobApps</span></span>](../api/intune-apps-mobilelobapp-list.md)|<span data-ttu-id="c5e4c-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c5e4c-112">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) collection</span></span>|<span data-ttu-id="c5e4c-113">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-113">List properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) objects.</span></span>|
|[<span data-ttu-id="c5e4c-114">mobileLobApp の取得</span><span class="sxs-lookup"><span data-stu-id="c5e4c-114">Get mobileLobApp</span></span>](../api/intune-apps-mobilelobapp-get.md)|[<span data-ttu-id="c5e4c-115">mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="c5e4c-115">mobileLobApp</span></span>](../resources/intune-apps-mobilelobapp.md)|<span data-ttu-id="c5e4c-116">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-116">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5e4c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5e4c-117">Properties</span></span>
|<span data-ttu-id="c5e4c-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5e4c-118">Property</span></span>|<span data-ttu-id="c5e4c-119">型</span><span class="sxs-lookup"><span data-stu-id="c5e4c-119">Type</span></span>|<span data-ttu-id="c5e4c-120">説明</span><span class="sxs-lookup"><span data-stu-id="c5e4c-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5e4c-121">id</span><span class="sxs-lookup"><span data-stu-id="c5e4c-121">id</span></span>|<span data-ttu-id="c5e4c-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c5e4c-122">String</span></span>|<span data-ttu-id="c5e4c-123">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-123">Key of the entity.</span></span> <span data-ttu-id="c5e4c-124">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-124">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-125">displayName</span><span class="sxs-lookup"><span data-stu-id="c5e4c-125">displayName</span></span>|<span data-ttu-id="c5e4c-126">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-126">String</span></span>|<span data-ttu-id="c5e4c-127">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-127">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c5e4c-128">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-128">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-129">description</span><span class="sxs-lookup"><span data-stu-id="c5e4c-129">description</span></span>|<span data-ttu-id="c5e4c-130">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-130">String</span></span>|<span data-ttu-id="c5e4c-131">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-131">The description of the app.</span></span> <span data-ttu-id="c5e4c-132">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-132">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-133">publisher</span><span class="sxs-lookup"><span data-stu-id="c5e4c-133">publisher</span></span>|<span data-ttu-id="c5e4c-134">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-134">String</span></span>|<span data-ttu-id="c5e4c-135">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-135">The publisher of the app.</span></span> <span data-ttu-id="c5e4c-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-137">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c5e4c-137">largeIcon</span></span>|[<span data-ttu-id="c5e4c-138">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c5e4c-138">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c5e4c-139">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-139">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c5e4c-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5e4c-141">createdDateTime</span></span>|<span data-ttu-id="c5e4c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5e4c-142">DateTimeOffset</span></span>|<span data-ttu-id="c5e4c-143">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-143">The date and time the app was created.</span></span> <span data-ttu-id="c5e4c-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5e4c-145">lastModifiedDateTime</span></span>|<span data-ttu-id="c5e4c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5e4c-146">DateTimeOffset</span></span>|<span data-ttu-id="c5e4c-147">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-147">The date and time the app was last modified.</span></span> <span data-ttu-id="c5e4c-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-149">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c5e4c-149">isFeatured</span></span>|<span data-ttu-id="c5e4c-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="c5e4c-150">Boolean</span></span>|<span data-ttu-id="c5e4c-151">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-151">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c5e4c-152">privacyInformationUrl</span></span>|<span data-ttu-id="c5e4c-153">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-153">String</span></span>|<span data-ttu-id="c5e4c-154">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-154">The privacy statement Url.</span></span> <span data-ttu-id="c5e4c-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-156">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c5e4c-156">informationUrl</span></span>|<span data-ttu-id="c5e4c-157">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-157">String</span></span>|<span data-ttu-id="c5e4c-158">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-158">The more information Url.</span></span> <span data-ttu-id="c5e4c-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-160">owner</span><span class="sxs-lookup"><span data-stu-id="c5e4c-160">owner</span></span>|<span data-ttu-id="c5e4c-161">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-161">String</span></span>|<span data-ttu-id="c5e4c-162">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-162">The owner of the app.</span></span> <span data-ttu-id="c5e4c-163">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-163">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-164">developer</span><span class="sxs-lookup"><span data-stu-id="c5e4c-164">developer</span></span>|<span data-ttu-id="c5e4c-165">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-165">String</span></span>|<span data-ttu-id="c5e4c-166">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-166">The developer of the app.</span></span> <span data-ttu-id="c5e4c-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-168">notes</span><span class="sxs-lookup"><span data-stu-id="c5e4c-168">notes</span></span>|<span data-ttu-id="c5e4c-169">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-169">String</span></span>|<span data-ttu-id="c5e4c-170">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-170">Notes for the app.</span></span> <span data-ttu-id="c5e4c-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-172">publishingState</span><span class="sxs-lookup"><span data-stu-id="c5e4c-172">publishingState</span></span>|[<span data-ttu-id="c5e4c-173">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c5e4c-173">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c5e4c-174">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-174">The publishing state for the app.</span></span> <span data-ttu-id="c5e4c-175">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-175">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c5e4c-176">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-176">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c5e4c-177">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-177">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c5e4c-178">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="c5e4c-178">committedContentVersion</span></span>|<span data-ttu-id="c5e4c-179">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-179">String</span></span>|<span data-ttu-id="c5e4c-180">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-180">The internal committed content version.</span></span>|
|<span data-ttu-id="c5e4c-181">fileName</span><span class="sxs-lookup"><span data-stu-id="c5e4c-181">fileName</span></span>|<span data-ttu-id="c5e4c-182">String</span><span class="sxs-lookup"><span data-stu-id="c5e4c-182">String</span></span>|<span data-ttu-id="c5e4c-183">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-183">The name of the main Lob application file.</span></span>|
|<span data-ttu-id="c5e4c-184">size</span><span class="sxs-lookup"><span data-stu-id="c5e4c-184">size</span></span>|<span data-ttu-id="c5e4c-185">Int64</span><span class="sxs-lookup"><span data-stu-id="c5e4c-185">Int64</span></span>|<span data-ttu-id="c5e4c-186">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-186">The total size, including all uploaded files.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5e4c-187">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c5e4c-187">Relationships</span></span>
|<span data-ttu-id="c5e4c-188">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c5e4c-188">Relationship</span></span>|<span data-ttu-id="c5e4c-189">型</span><span class="sxs-lookup"><span data-stu-id="c5e4c-189">Type</span></span>|<span data-ttu-id="c5e4c-190">説明</span><span class="sxs-lookup"><span data-stu-id="c5e4c-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5e4c-191">categories</span><span class="sxs-lookup"><span data-stu-id="c5e4c-191">categories</span></span>|<span data-ttu-id="c5e4c-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c5e4c-192">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="c5e4c-193">このアプリのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-193">The list of categories for this app.</span></span> <span data-ttu-id="c5e4c-194">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-194">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-195">assignments</span><span class="sxs-lookup"><span data-stu-id="c5e4c-195">assignments</span></span>|<span data-ttu-id="c5e4c-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c5e4c-196">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="c5e4c-197">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-197">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="c5e4c-198">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c5e4c-198">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c5e4c-199">contentVersions</span><span class="sxs-lookup"><span data-stu-id="c5e4c-199">contentVersions</span></span>|<span data-ttu-id="c5e4c-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c5e4c-200">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) collection</span></span>|<span data-ttu-id="c5e4c-201">このアプリのコンテンツのバージョンのリスト。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-201">The list of content versions for this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5e4c-202">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5e4c-202">JSON Representation</span></span>
<span data-ttu-id="c5e4c-203">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c5e4c-203">Here is a JSON representation of the resource.</span></span>
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



