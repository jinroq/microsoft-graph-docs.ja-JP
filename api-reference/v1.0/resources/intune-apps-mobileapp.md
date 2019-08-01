---
title: mobileApp リソースの種類
description: Intune モバイル アプリの基本プロパティを含む抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08bc3cb0c6b1a7b815e30179aa79861b08ad3b15
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028953"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="d0176-103">mobileApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0176-103">mobileApp resource type</span></span>

> <span data-ttu-id="d0176-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0176-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0176-105">Intune モバイル アプリの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="d0176-105">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="d0176-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0176-106">Methods</span></span>
|<span data-ttu-id="d0176-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0176-107">Method</span></span>|<span data-ttu-id="d0176-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d0176-108">Return Type</span></span>|<span data-ttu-id="d0176-109">説明</span><span class="sxs-lookup"><span data-stu-id="d0176-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0176-110">mobileApps のリスト</span><span class="sxs-lookup"><span data-stu-id="d0176-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="d0176-111">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d0176-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="d0176-112">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d0176-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="d0176-113">MobileApp の取得</span><span class="sxs-lookup"><span data-stu-id="d0176-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="d0176-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="d0176-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="d0176-115">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d0176-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="d0176-116">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="d0176-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="d0176-117">なし</span><span class="sxs-lookup"><span data-stu-id="d0176-117">None</span></span>|<span data-ttu-id="d0176-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d0176-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d0176-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0176-119">Properties</span></span>
|<span data-ttu-id="d0176-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0176-120">Property</span></span>|<span data-ttu-id="d0176-121">型</span><span class="sxs-lookup"><span data-stu-id="d0176-121">Type</span></span>|<span data-ttu-id="d0176-122">説明</span><span class="sxs-lookup"><span data-stu-id="d0176-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0176-123">id</span><span class="sxs-lookup"><span data-stu-id="d0176-123">id</span></span>|<span data-ttu-id="d0176-124">文字列</span><span class="sxs-lookup"><span data-stu-id="d0176-124">String</span></span>|<span data-ttu-id="d0176-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d0176-125">Key of the entity.</span></span>|
|<span data-ttu-id="d0176-126">displayName</span><span class="sxs-lookup"><span data-stu-id="d0176-126">displayName</span></span>|<span data-ttu-id="d0176-127">文字列</span><span class="sxs-lookup"><span data-stu-id="d0176-127">String</span></span>|<span data-ttu-id="d0176-128">管理者が提供またはインポートしたアプリのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="d0176-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="d0176-129">description</span><span class="sxs-lookup"><span data-stu-id="d0176-129">description</span></span>|<span data-ttu-id="d0176-130">String</span><span class="sxs-lookup"><span data-stu-id="d0176-130">String</span></span>|<span data-ttu-id="d0176-131">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="d0176-131">The description of the app.</span></span>|
|<span data-ttu-id="d0176-132">publisher</span><span class="sxs-lookup"><span data-stu-id="d0176-132">publisher</span></span>|<span data-ttu-id="d0176-133">String</span><span class="sxs-lookup"><span data-stu-id="d0176-133">String</span></span>|<span data-ttu-id="d0176-134">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="d0176-134">The publisher of the app.</span></span>|
|<span data-ttu-id="d0176-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d0176-135">largeIcon</span></span>|[<span data-ttu-id="d0176-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d0176-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d0176-137">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="d0176-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="d0176-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0176-138">createdDateTime</span></span>|<span data-ttu-id="d0176-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0176-139">DateTimeOffset</span></span>|<span data-ttu-id="d0176-140">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d0176-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="d0176-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0176-141">lastModifiedDateTime</span></span>|<span data-ttu-id="d0176-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0176-142">DateTimeOffset</span></span>|<span data-ttu-id="d0176-143">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d0176-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="d0176-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d0176-144">isFeatured</span></span>|<span data-ttu-id="d0176-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="d0176-145">Boolean</span></span>|<span data-ttu-id="d0176-146">アプリが管理者のおすすめとしてマークされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="d0176-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="d0176-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d0176-147">privacyInformationUrl</span></span>|<span data-ttu-id="d0176-148">String</span><span class="sxs-lookup"><span data-stu-id="d0176-148">String</span></span>|<span data-ttu-id="d0176-149">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="d0176-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="d0176-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d0176-150">informationUrl</span></span>|<span data-ttu-id="d0176-151">String</span><span class="sxs-lookup"><span data-stu-id="d0176-151">String</span></span>|<span data-ttu-id="d0176-152">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="d0176-152">The more information Url.</span></span>|
|<span data-ttu-id="d0176-153">owner</span><span class="sxs-lookup"><span data-stu-id="d0176-153">owner</span></span>|<span data-ttu-id="d0176-154">String</span><span class="sxs-lookup"><span data-stu-id="d0176-154">String</span></span>|<span data-ttu-id="d0176-155">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="d0176-155">The owner of the app.</span></span>|
|<span data-ttu-id="d0176-156">developer</span><span class="sxs-lookup"><span data-stu-id="d0176-156">developer</span></span>|<span data-ttu-id="d0176-157">String</span><span class="sxs-lookup"><span data-stu-id="d0176-157">String</span></span>|<span data-ttu-id="d0176-158">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="d0176-158">The developer of the app.</span></span>|
|<span data-ttu-id="d0176-159">notes</span><span class="sxs-lookup"><span data-stu-id="d0176-159">notes</span></span>|<span data-ttu-id="d0176-160">String</span><span class="sxs-lookup"><span data-stu-id="d0176-160">String</span></span>|<span data-ttu-id="d0176-161">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="d0176-161">Notes for the app.</span></span>|
|<span data-ttu-id="d0176-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="d0176-162">publishingState</span></span>|[<span data-ttu-id="d0176-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d0176-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d0176-164">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="d0176-164">The publishing state for the app.</span></span> <span data-ttu-id="d0176-165">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="d0176-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d0176-166">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="d0176-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0176-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d0176-167">Relationships</span></span>
|<span data-ttu-id="d0176-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d0176-168">Relationship</span></span>|<span data-ttu-id="d0176-169">型</span><span class="sxs-lookup"><span data-stu-id="d0176-169">Type</span></span>|<span data-ttu-id="d0176-170">説明</span><span class="sxs-lookup"><span data-stu-id="d0176-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0176-171">categories</span><span class="sxs-lookup"><span data-stu-id="d0176-171">categories</span></span>|<span data-ttu-id="d0176-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d0176-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="d0176-173">このアプリのカテゴリのリストです。</span><span class="sxs-lookup"><span data-stu-id="d0176-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="d0176-174">assignments</span><span class="sxs-lookup"><span data-stu-id="d0176-174">assignments</span></span>|<span data-ttu-id="d0176-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d0176-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="d0176-176">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="d0176-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0176-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0176-177">JSON Representation</span></span>
<span data-ttu-id="d0176-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d0176-178">Here is a JSON representation of the resource.</span></span>
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
  "publishingState": "String"
}
```



