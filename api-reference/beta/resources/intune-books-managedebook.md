---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6fd4fd3caef3aab90257805a48e53bee9c6b8764
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962598"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="e531b-103">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e531b-103">managedEBook resource type</span></span>

> <span data-ttu-id="e531b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e531b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e531b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e531b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e531b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e531b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e531b-107">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="e531b-107">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="e531b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e531b-108">Methods</span></span>
|<span data-ttu-id="e531b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e531b-109">Method</span></span>|<span data-ttu-id="e531b-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e531b-110">Return Type</span></span>|<span data-ttu-id="e531b-111">説明</span><span class="sxs-lookup"><span data-stu-id="e531b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e531b-112">managedEBook のリスト</span><span class="sxs-lookup"><span data-stu-id="e531b-112">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="e531b-113">[managedEBook](../resources/intune-books-managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e531b-113">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="e531b-114">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e531b-114">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="e531b-115">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="e531b-115">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="e531b-116">managedEBook</span><span class="sxs-lookup"><span data-stu-id="e531b-116">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="e531b-117">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e531b-117">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="e531b-118">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="e531b-118">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="e531b-119">なし</span><span class="sxs-lookup"><span data-stu-id="e531b-119">None</span></span>|<span data-ttu-id="e531b-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e531b-120">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e531b-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e531b-121">Properties</span></span>
|<span data-ttu-id="e531b-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e531b-122">Property</span></span>|<span data-ttu-id="e531b-123">種類</span><span class="sxs-lookup"><span data-stu-id="e531b-123">Type</span></span>|<span data-ttu-id="e531b-124">説明</span><span class="sxs-lookup"><span data-stu-id="e531b-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e531b-125">ID</span><span class="sxs-lookup"><span data-stu-id="e531b-125">id</span></span>|<span data-ttu-id="e531b-126">String</span><span class="sxs-lookup"><span data-stu-id="e531b-126">String</span></span>|<span data-ttu-id="e531b-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e531b-127">Key of the entity.</span></span>|
|<span data-ttu-id="e531b-128">displayName</span><span class="sxs-lookup"><span data-stu-id="e531b-128">displayName</span></span>|<span data-ttu-id="e531b-129">String</span><span class="sxs-lookup"><span data-stu-id="e531b-129">String</span></span>|<span data-ttu-id="e531b-130">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="e531b-130">Name of the eBook.</span></span>|
|<span data-ttu-id="e531b-131">説明</span><span class="sxs-lookup"><span data-stu-id="e531b-131">description</span></span>|<span data-ttu-id="e531b-132">String</span><span class="sxs-lookup"><span data-stu-id="e531b-132">String</span></span>|<span data-ttu-id="e531b-133">説明。</span><span class="sxs-lookup"><span data-stu-id="e531b-133">Description.</span></span>|
|<span data-ttu-id="e531b-134">publisher</span><span class="sxs-lookup"><span data-stu-id="e531b-134">publisher</span></span>|<span data-ttu-id="e531b-135">String</span><span class="sxs-lookup"><span data-stu-id="e531b-135">String</span></span>|<span data-ttu-id="e531b-136">発行元です。</span><span class="sxs-lookup"><span data-stu-id="e531b-136">Publisher.</span></span>|
|<span data-ttu-id="e531b-137">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e531b-137">publishedDateTime</span></span>|<span data-ttu-id="e531b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e531b-138">DateTimeOffset</span></span>|<span data-ttu-id="e531b-139">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="e531b-139">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="e531b-140">largeCover</span><span class="sxs-lookup"><span data-stu-id="e531b-140">largeCover</span></span>|[<span data-ttu-id="e531b-141">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e531b-141">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e531b-142">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="e531b-142">Book cover.</span></span>|
|<span data-ttu-id="e531b-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e531b-143">createdDateTime</span></span>|<span data-ttu-id="e531b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e531b-144">DateTimeOffset</span></span>|<span data-ttu-id="e531b-145">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e531b-145">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="e531b-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e531b-146">lastModifiedDateTime</span></span>|<span data-ttu-id="e531b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e531b-147">DateTimeOffset</span></span>|<span data-ttu-id="e531b-148">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e531b-148">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="e531b-149">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e531b-149">informationUrl</span></span>|<span data-ttu-id="e531b-150">String</span><span class="sxs-lookup"><span data-stu-id="e531b-150">String</span></span>|<span data-ttu-id="e531b-151">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e531b-151">The more information Url.</span></span>|
|<span data-ttu-id="e531b-152">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e531b-152">privacyInformationUrl</span></span>|<span data-ttu-id="e531b-153">String</span><span class="sxs-lookup"><span data-stu-id="e531b-153">String</span></span>|<span data-ttu-id="e531b-154">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e531b-154">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e531b-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e531b-155">Relationships</span></span>
|<span data-ttu-id="e531b-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e531b-156">Relationship</span></span>|<span data-ttu-id="e531b-157">型</span><span class="sxs-lookup"><span data-stu-id="e531b-157">Type</span></span>|<span data-ttu-id="e531b-158">説明</span><span class="sxs-lookup"><span data-stu-id="e531b-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e531b-159">categories</span><span class="sxs-lookup"><span data-stu-id="e531b-159">categories</span></span>|<span data-ttu-id="e531b-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e531b-160">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="e531b-161">この eBook のカテゴリの一覧です。</span><span class="sxs-lookup"><span data-stu-id="e531b-161">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="e531b-162">assignments</span><span class="sxs-lookup"><span data-stu-id="e531b-162">assignments</span></span>|<span data-ttu-id="e531b-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e531b-163">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="e531b-164">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="e531b-164">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="e531b-165">installSummary</span><span class="sxs-lookup"><span data-stu-id="e531b-165">installSummary</span></span>|[<span data-ttu-id="e531b-166">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e531b-166">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="e531b-167">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="e531b-167">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="e531b-168">deviceStates</span><span class="sxs-lookup"><span data-stu-id="e531b-168">deviceStates</span></span>|<span data-ttu-id="e531b-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e531b-169">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="e531b-170">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="e531b-170">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="e531b-171">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="e531b-171">userStateSummary</span></span>|<span data-ttu-id="e531b-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e531b-172">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="e531b-173">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="e531b-173">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e531b-174">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e531b-174">JSON Representation</span></span>
<span data-ttu-id="e531b-175">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e531b-175">Here is a JSON representation of the resource.</span></span>
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





