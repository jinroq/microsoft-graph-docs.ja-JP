---
title: mobileApp リソースの種類
description: Intune モバイル アプリの基本プロパティを含む抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91167967a543ea4556c1704a2bba4ec9a10a4c3d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557895"
---
# <a name="mobileapp-resource-type"></a><span data-ttu-id="e9291-103">mobileApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9291-103">mobileApp resource type</span></span>

> <span data-ttu-id="e9291-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e9291-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9291-105">Intune モバイル アプリの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="e9291-105">An abstract class containing the base properties for Intune mobile apps.</span></span>

## <a name="methods"></a><span data-ttu-id="e9291-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="e9291-106">Methods</span></span>
|<span data-ttu-id="e9291-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e9291-107">Method</span></span>|<span data-ttu-id="e9291-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e9291-108">Return Type</span></span>|<span data-ttu-id="e9291-109">説明</span><span class="sxs-lookup"><span data-stu-id="e9291-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e9291-110">mobileApps のリスト</span><span class="sxs-lookup"><span data-stu-id="e9291-110">List mobileApps</span></span>](../api/intune-apps-mobileapp-list.md)|<span data-ttu-id="e9291-111">[mobileApp](../resources/intune-apps-mobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e9291-111">[mobileApp](../resources/intune-apps-mobileapp.md) collection</span></span>|<span data-ttu-id="e9291-112">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e9291-112">List properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) objects.</span></span>|
|[<span data-ttu-id="e9291-113">MobileApp の取得</span><span class="sxs-lookup"><span data-stu-id="e9291-113">Get mobileApp</span></span>](../api/intune-apps-mobileapp-get.md)|[<span data-ttu-id="e9291-114">mobileApp</span><span class="sxs-lookup"><span data-stu-id="e9291-114">mobileApp</span></span>](../resources/intune-apps-mobileapp.md)|<span data-ttu-id="e9291-115">[mobileApp](../resources/intune-apps-mobileapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e9291-115">Read properties and relationships of the [mobileApp](../resources/intune-apps-mobileapp.md) object.</span></span>|
|[<span data-ttu-id="e9291-116">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="e9291-116">assign action</span></span>](../api/intune-apps-mobileapp-assign.md)|<span data-ttu-id="e9291-117">なし</span><span class="sxs-lookup"><span data-stu-id="e9291-117">None</span></span>|<span data-ttu-id="e9291-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e9291-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e9291-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9291-119">Properties</span></span>
|<span data-ttu-id="e9291-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9291-120">Property</span></span>|<span data-ttu-id="e9291-121">型</span><span class="sxs-lookup"><span data-stu-id="e9291-121">Type</span></span>|<span data-ttu-id="e9291-122">説明</span><span class="sxs-lookup"><span data-stu-id="e9291-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9291-123">id</span><span class="sxs-lookup"><span data-stu-id="e9291-123">id</span></span>|<span data-ttu-id="e9291-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e9291-124">String</span></span>|<span data-ttu-id="e9291-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e9291-125">Key of the entity.</span></span>|
|<span data-ttu-id="e9291-126">displayName</span><span class="sxs-lookup"><span data-stu-id="e9291-126">displayName</span></span>|<span data-ttu-id="e9291-127">String</span><span class="sxs-lookup"><span data-stu-id="e9291-127">String</span></span>|<span data-ttu-id="e9291-128">管理者が提供またはインポートしたアプリのタイトルです。</span><span class="sxs-lookup"><span data-stu-id="e9291-128">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="e9291-129">description</span><span class="sxs-lookup"><span data-stu-id="e9291-129">description</span></span>|<span data-ttu-id="e9291-130">String</span><span class="sxs-lookup"><span data-stu-id="e9291-130">String</span></span>|<span data-ttu-id="e9291-131">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e9291-131">The description of the app.</span></span>|
|<span data-ttu-id="e9291-132">publisher</span><span class="sxs-lookup"><span data-stu-id="e9291-132">publisher</span></span>|<span data-ttu-id="e9291-133">String</span><span class="sxs-lookup"><span data-stu-id="e9291-133">String</span></span>|<span data-ttu-id="e9291-134">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e9291-134">The publisher of the app.</span></span>|
|<span data-ttu-id="e9291-135">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e9291-135">largeIcon</span></span>|[<span data-ttu-id="e9291-136">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e9291-136">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e9291-137">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="e9291-137">The large icon, to be displayed in the app details and used for upload of the icon.</span></span>|
|<span data-ttu-id="e9291-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e9291-138">createdDateTime</span></span>|<span data-ttu-id="e9291-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9291-139">DateTimeOffset</span></span>|<span data-ttu-id="e9291-140">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e9291-140">The date and time the app was created.</span></span>|
|<span data-ttu-id="e9291-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e9291-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e9291-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9291-142">DateTimeOffset</span></span>|<span data-ttu-id="e9291-143">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e9291-143">The date and time the app was last modified.</span></span>|
|<span data-ttu-id="e9291-144">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e9291-144">isFeatured</span></span>|<span data-ttu-id="e9291-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e9291-145">Boolean</span></span>|<span data-ttu-id="e9291-146">アプリが管理者のおすすめとしてマークされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e9291-146">The value indicating whether the app is marked as featured by the admin.</span></span>|
|<span data-ttu-id="e9291-147">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e9291-147">privacyInformationUrl</span></span>|<span data-ttu-id="e9291-148">String</span><span class="sxs-lookup"><span data-stu-id="e9291-148">String</span></span>|<span data-ttu-id="e9291-149">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e9291-149">The privacy statement Url.</span></span>|
|<span data-ttu-id="e9291-150">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e9291-150">informationUrl</span></span>|<span data-ttu-id="e9291-151">String</span><span class="sxs-lookup"><span data-stu-id="e9291-151">String</span></span>|<span data-ttu-id="e9291-152">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e9291-152">The more information Url.</span></span>|
|<span data-ttu-id="e9291-153">owner</span><span class="sxs-lookup"><span data-stu-id="e9291-153">owner</span></span>|<span data-ttu-id="e9291-154">String</span><span class="sxs-lookup"><span data-stu-id="e9291-154">String</span></span>|<span data-ttu-id="e9291-155">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e9291-155">The owner of the app.</span></span>|
|<span data-ttu-id="e9291-156">developer</span><span class="sxs-lookup"><span data-stu-id="e9291-156">developer</span></span>|<span data-ttu-id="e9291-157">String</span><span class="sxs-lookup"><span data-stu-id="e9291-157">String</span></span>|<span data-ttu-id="e9291-158">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e9291-158">The developer of the app.</span></span>|
|<span data-ttu-id="e9291-159">notes</span><span class="sxs-lookup"><span data-stu-id="e9291-159">notes</span></span>|<span data-ttu-id="e9291-160">String</span><span class="sxs-lookup"><span data-stu-id="e9291-160">String</span></span>|<span data-ttu-id="e9291-161">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e9291-161">Notes for the app.</span></span>|
|<span data-ttu-id="e9291-162">publishingState</span><span class="sxs-lookup"><span data-stu-id="e9291-162">publishingState</span></span>|[<span data-ttu-id="e9291-163">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e9291-163">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e9291-164">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e9291-164">The publishing state for the app.</span></span> <span data-ttu-id="e9291-165">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e9291-165">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e9291-166">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e9291-166">Possible values are: `notPublished`, `processing`, `published`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9291-167">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e9291-167">Relationships</span></span>
|<span data-ttu-id="e9291-168">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e9291-168">Relationship</span></span>|<span data-ttu-id="e9291-169">型</span><span class="sxs-lookup"><span data-stu-id="e9291-169">Type</span></span>|<span data-ttu-id="e9291-170">説明</span><span class="sxs-lookup"><span data-stu-id="e9291-170">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9291-171">categories</span><span class="sxs-lookup"><span data-stu-id="e9291-171">categories</span></span>|<span data-ttu-id="e9291-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e9291-172">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="e9291-173">このアプリのカテゴリのリストです。</span><span class="sxs-lookup"><span data-stu-id="e9291-173">The list of categories for this app.</span></span>|
|<span data-ttu-id="e9291-174">assignments</span><span class="sxs-lookup"><span data-stu-id="e9291-174">assignments</span></span>|<span data-ttu-id="e9291-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e9291-175">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="e9291-176">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="e9291-176">The list of group assignments for this mobile app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9291-177">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9291-177">JSON Representation</span></span>
<span data-ttu-id="e9291-178">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e9291-178">Here is a JSON representation of the resource.</span></span>
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



