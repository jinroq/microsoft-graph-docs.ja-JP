---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08bd5cc6f5630aca0ff5b35c5590875d259ad294
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422048"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="467b1-103">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="467b1-103">managedEBook resource type</span></span>

> <span data-ttu-id="467b1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="467b1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="467b1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="467b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="467b1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="467b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="467b1-107">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="467b1-107">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="467b1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="467b1-108">Methods</span></span>
|<span data-ttu-id="467b1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="467b1-109">Method</span></span>|<span data-ttu-id="467b1-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="467b1-110">Return Type</span></span>|<span data-ttu-id="467b1-111">説明</span><span class="sxs-lookup"><span data-stu-id="467b1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="467b1-112">managedEBook のリスト</span><span class="sxs-lookup"><span data-stu-id="467b1-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="467b1-113">[managedEBook](../resources/intune-books-managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="467b1-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="467b1-114">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="467b1-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="467b1-115">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="467b1-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="467b1-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="467b1-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="467b1-117">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="467b1-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="467b1-118">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="467b1-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="467b1-119">なし</span><span class="sxs-lookup"><span data-stu-id="467b1-119">None</span></span>|<span data-ttu-id="467b1-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="467b1-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="467b1-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="467b1-121">Properties</span></span>
|<span data-ttu-id="467b1-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="467b1-122">Property</span></span>|<span data-ttu-id="467b1-123">型</span><span class="sxs-lookup"><span data-stu-id="467b1-123">Type</span></span>|<span data-ttu-id="467b1-124">説明</span><span class="sxs-lookup"><span data-stu-id="467b1-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="467b1-125">id</span><span class="sxs-lookup"><span data-stu-id="467b1-125">id</span></span>|<span data-ttu-id="467b1-126">String</span><span class="sxs-lookup"><span data-stu-id="467b1-126">String</span></span>|<span data-ttu-id="467b1-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="467b1-127">Key of the entity.</span></span>|
|<span data-ttu-id="467b1-128">displayName</span><span class="sxs-lookup"><span data-stu-id="467b1-128">displayName</span></span>|<span data-ttu-id="467b1-129">String</span><span class="sxs-lookup"><span data-stu-id="467b1-129">String</span></span>|<span data-ttu-id="467b1-130">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="467b1-130">Name of the eBook.</span></span>|
|<span data-ttu-id="467b1-131">説明</span><span class="sxs-lookup"><span data-stu-id="467b1-131">description</span></span>|<span data-ttu-id="467b1-132">String</span><span class="sxs-lookup"><span data-stu-id="467b1-132">String</span></span>|<span data-ttu-id="467b1-133">説明。</span><span class="sxs-lookup"><span data-stu-id="467b1-133">Description.</span></span>|
|<span data-ttu-id="467b1-134">publisher</span><span class="sxs-lookup"><span data-stu-id="467b1-134">publisher</span></span>|<span data-ttu-id="467b1-135">String</span><span class="sxs-lookup"><span data-stu-id="467b1-135">String</span></span>|<span data-ttu-id="467b1-136">発行元です。</span><span class="sxs-lookup"><span data-stu-id="467b1-136">Publisher.</span></span>|
|<span data-ttu-id="467b1-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="467b1-137">publishedDateTime</span></span>|<span data-ttu-id="467b1-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="467b1-138">DateTimeOffset</span></span>|<span data-ttu-id="467b1-139">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="467b1-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="467b1-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="467b1-140">largeCover</span></span>|[<span data-ttu-id="467b1-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="467b1-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="467b1-142">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="467b1-142">Book cover.</span></span>|
|<span data-ttu-id="467b1-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="467b1-143">createdDateTime</span></span>|<span data-ttu-id="467b1-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="467b1-144">DateTimeOffset</span></span>|<span data-ttu-id="467b1-145">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="467b1-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="467b1-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="467b1-146">lastModifiedDateTime</span></span>|<span data-ttu-id="467b1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="467b1-147">DateTimeOffset</span></span>|<span data-ttu-id="467b1-148">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="467b1-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="467b1-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="467b1-149">informationUrl</span></span>|<span data-ttu-id="467b1-150">String</span><span class="sxs-lookup"><span data-stu-id="467b1-150">String</span></span>|<span data-ttu-id="467b1-151">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="467b1-151">The more information Url.</span></span>|
|<span data-ttu-id="467b1-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="467b1-152">privacyInformationUrl</span></span>|<span data-ttu-id="467b1-153">String</span><span class="sxs-lookup"><span data-stu-id="467b1-153">String</span></span>|<span data-ttu-id="467b1-154">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="467b1-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="467b1-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="467b1-155">Relationships</span></span>
|<span data-ttu-id="467b1-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="467b1-156">Relationship</span></span>|<span data-ttu-id="467b1-157">型</span><span class="sxs-lookup"><span data-stu-id="467b1-157">Type</span></span>|<span data-ttu-id="467b1-158">説明</span><span class="sxs-lookup"><span data-stu-id="467b1-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="467b1-159">categories</span><span class="sxs-lookup"><span data-stu-id="467b1-159">categories</span></span>|<span data-ttu-id="467b1-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="467b1-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="467b1-161">この eBook のカテゴリの一覧です。</span><span class="sxs-lookup"><span data-stu-id="467b1-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="467b1-162">assignments</span><span class="sxs-lookup"><span data-stu-id="467b1-162">assignments</span></span>|<span data-ttu-id="467b1-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="467b1-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="467b1-164">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="467b1-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="467b1-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="467b1-165">installSummary</span></span>|[<span data-ttu-id="467b1-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="467b1-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="467b1-167">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="467b1-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="467b1-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="467b1-168">deviceStates</span></span>|<span data-ttu-id="467b1-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="467b1-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="467b1-170">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="467b1-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="467b1-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="467b1-171">userStateSummary</span></span>|<span data-ttu-id="467b1-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="467b1-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="467b1-173">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="467b1-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="467b1-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="467b1-174">JSON Representation</span></span>
<span data-ttu-id="467b1-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="467b1-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBook"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String"
}
```




