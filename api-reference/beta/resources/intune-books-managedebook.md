---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a9248a2bca56188deb913159d9ff664ce8d9b48
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949298"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="e8e3a-103">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8e3a-103">managedEBook resource type</span></span>

> <span data-ttu-id="e8e3a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8e3a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8e3a-106">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="e8e3a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8e3a-107">Methods</span></span>
|<span data-ttu-id="e8e3a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e8e3a-108">Method</span></span>|<span data-ttu-id="e8e3a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e8e3a-109">Return Type</span></span>|<span data-ttu-id="e8e3a-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8e3a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e8e3a-111">managedEBook のリスト</span><span class="sxs-lookup"><span data-stu-id="e8e3a-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="e8e3a-112">[managedEBook](../resources/intune-books-managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e8e3a-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="e8e3a-113">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="e8e3a-114">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="e8e3a-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="e8e3a-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="e8e3a-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="e8e3a-116">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="e8e3a-117">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="e8e3a-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="e8e3a-118">なし</span><span class="sxs-lookup"><span data-stu-id="e8e3a-118">None</span></span>|<span data-ttu-id="e8e3a-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e8e3a-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="e8e3a-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8e3a-120">Properties</span></span>
|<span data-ttu-id="e8e3a-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8e3a-121">Property</span></span>|<span data-ttu-id="e8e3a-122">種類</span><span class="sxs-lookup"><span data-stu-id="e8e3a-122">Type</span></span>|<span data-ttu-id="e8e3a-123">説明</span><span class="sxs-lookup"><span data-stu-id="e8e3a-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8e3a-124">id</span><span class="sxs-lookup"><span data-stu-id="e8e3a-124">id</span></span>|<span data-ttu-id="e8e3a-125">文字列</span><span class="sxs-lookup"><span data-stu-id="e8e3a-125">String</span></span>|<span data-ttu-id="e8e3a-126">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-126">Key of the entity.</span></span>|
|<span data-ttu-id="e8e3a-127">displayName</span><span class="sxs-lookup"><span data-stu-id="e8e3a-127">displayName</span></span>|<span data-ttu-id="e8e3a-128">String</span><span class="sxs-lookup"><span data-stu-id="e8e3a-128">String</span></span>|<span data-ttu-id="e8e3a-129">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-129">Name of the eBook.</span></span>|
|<span data-ttu-id="e8e3a-130">description</span><span class="sxs-lookup"><span data-stu-id="e8e3a-130">description</span></span>|<span data-ttu-id="e8e3a-131">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e8e3a-131">String</span></span>|<span data-ttu-id="e8e3a-132">説明。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-132">Description.</span></span>|
|<span data-ttu-id="e8e3a-133">publisher</span><span class="sxs-lookup"><span data-stu-id="e8e3a-133">publisher</span></span>|<span data-ttu-id="e8e3a-134">String</span><span class="sxs-lookup"><span data-stu-id="e8e3a-134">String</span></span>|<span data-ttu-id="e8e3a-135">発行元です。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-135">Publisher.</span></span>|
|<span data-ttu-id="e8e3a-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8e3a-136">publishedDateTime</span></span>|<span data-ttu-id="e8e3a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8e3a-137">DateTimeOffset</span></span>|<span data-ttu-id="e8e3a-138">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="e8e3a-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="e8e3a-139">largeCover</span></span>|[<span data-ttu-id="e8e3a-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e8e3a-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e8e3a-141">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-141">Book cover.</span></span>|
|<span data-ttu-id="e8e3a-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e8e3a-142">createdDateTime</span></span>|<span data-ttu-id="e8e3a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8e3a-143">DateTimeOffset</span></span>|<span data-ttu-id="e8e3a-144">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="e8e3a-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e8e3a-145">lastModifiedDateTime</span></span>|<span data-ttu-id="e8e3a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e8e3a-146">DateTimeOffset</span></span>|<span data-ttu-id="e8e3a-147">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="e8e3a-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e8e3a-148">informationUrl</span></span>|<span data-ttu-id="e8e3a-149">String</span><span class="sxs-lookup"><span data-stu-id="e8e3a-149">String</span></span>|<span data-ttu-id="e8e3a-150">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-150">The more information Url.</span></span>|
|<span data-ttu-id="e8e3a-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e8e3a-151">privacyInformationUrl</span></span>|<span data-ttu-id="e8e3a-152">String</span><span class="sxs-lookup"><span data-stu-id="e8e3a-152">String</span></span>|<span data-ttu-id="e8e3a-153">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8e3a-154">関係</span><span class="sxs-lookup"><span data-stu-id="e8e3a-154">Relationships</span></span>
|<span data-ttu-id="e8e3a-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e8e3a-155">Relationship</span></span>|<span data-ttu-id="e8e3a-156">型</span><span class="sxs-lookup"><span data-stu-id="e8e3a-156">Type</span></span>|<span data-ttu-id="e8e3a-157">説明</span><span class="sxs-lookup"><span data-stu-id="e8e3a-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8e3a-158">categories</span><span class="sxs-lookup"><span data-stu-id="e8e3a-158">categories</span></span>|<span data-ttu-id="e8e3a-159">[Managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e8e3a-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="e8e3a-160">この電子ブックのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="e8e3a-161">assignments</span><span class="sxs-lookup"><span data-stu-id="e8e3a-161">assignments</span></span>|<span data-ttu-id="e8e3a-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e8e3a-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="e8e3a-163">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="e8e3a-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="e8e3a-164">installSummary</span></span>|[<span data-ttu-id="e8e3a-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e8e3a-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="e8e3a-166">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="e8e3a-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="e8e3a-167">deviceStates</span></span>|<span data-ttu-id="e8e3a-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e8e3a-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="e8e3a-169">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="e8e3a-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="e8e3a-170">userStateSummary</span></span>|<span data-ttu-id="e8e3a-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e8e3a-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="e8e3a-172">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e8e3a-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8e3a-173">JSON Representation</span></span>
<span data-ttu-id="e8e3a-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e8e3a-174">Here is a JSON representation of the resource.</span></span>
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




