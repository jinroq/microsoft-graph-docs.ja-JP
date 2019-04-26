---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 888df51e17ab45dcada3d69fad95315b26b4b20e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561181"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="49cdf-103">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49cdf-103">managedEBook resource type</span></span>

> <span data-ttu-id="49cdf-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49cdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49cdf-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="49cdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49cdf-106">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="49cdf-106">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="49cdf-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="49cdf-107">Methods</span></span>
|<span data-ttu-id="49cdf-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="49cdf-108">Method</span></span>|<span data-ttu-id="49cdf-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="49cdf-109">Return Type</span></span>|<span data-ttu-id="49cdf-110">説明</span><span class="sxs-lookup"><span data-stu-id="49cdf-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="49cdf-111">managedEBook のリスト</span><span class="sxs-lookup"><span data-stu-id="49cdf-111">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="49cdf-112">[managedEBook](../resources/intune-books-managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="49cdf-112">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="49cdf-113">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="49cdf-113">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="49cdf-114">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="49cdf-114">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="49cdf-115">managedEBook</span><span class="sxs-lookup"><span data-stu-id="49cdf-115">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="49cdf-116">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="49cdf-116">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="49cdf-117">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="49cdf-117">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="49cdf-118">なし</span><span class="sxs-lookup"><span data-stu-id="49cdf-118">None</span></span>|<span data-ttu-id="49cdf-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="49cdf-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="49cdf-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49cdf-120">Properties</span></span>
|<span data-ttu-id="49cdf-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49cdf-121">Property</span></span>|<span data-ttu-id="49cdf-122">型</span><span class="sxs-lookup"><span data-stu-id="49cdf-122">Type</span></span>|<span data-ttu-id="49cdf-123">説明</span><span class="sxs-lookup"><span data-stu-id="49cdf-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49cdf-124">id</span><span class="sxs-lookup"><span data-stu-id="49cdf-124">id</span></span>|<span data-ttu-id="49cdf-125">String</span><span class="sxs-lookup"><span data-stu-id="49cdf-125">String</span></span>|<span data-ttu-id="49cdf-126">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="49cdf-126">Key of the entity.</span></span>|
|<span data-ttu-id="49cdf-127">displayName</span><span class="sxs-lookup"><span data-stu-id="49cdf-127">displayName</span></span>|<span data-ttu-id="49cdf-128">String</span><span class="sxs-lookup"><span data-stu-id="49cdf-128">String</span></span>|<span data-ttu-id="49cdf-129">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="49cdf-129">Name of the eBook.</span></span>|
|<span data-ttu-id="49cdf-130">description</span><span class="sxs-lookup"><span data-stu-id="49cdf-130">description</span></span>|<span data-ttu-id="49cdf-131">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="49cdf-131">String</span></span>|<span data-ttu-id="49cdf-132">説明。</span><span class="sxs-lookup"><span data-stu-id="49cdf-132">Description.</span></span>|
|<span data-ttu-id="49cdf-133">publisher</span><span class="sxs-lookup"><span data-stu-id="49cdf-133">publisher</span></span>|<span data-ttu-id="49cdf-134">String</span><span class="sxs-lookup"><span data-stu-id="49cdf-134">String</span></span>|<span data-ttu-id="49cdf-135">発行元です。</span><span class="sxs-lookup"><span data-stu-id="49cdf-135">Publisher.</span></span>|
|<span data-ttu-id="49cdf-136">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="49cdf-136">publishedDateTime</span></span>|<span data-ttu-id="49cdf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49cdf-137">DateTimeOffset</span></span>|<span data-ttu-id="49cdf-138">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="49cdf-138">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="49cdf-139">largeCover</span><span class="sxs-lookup"><span data-stu-id="49cdf-139">largeCover</span></span>|[<span data-ttu-id="49cdf-140">mimeContent</span><span class="sxs-lookup"><span data-stu-id="49cdf-140">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="49cdf-141">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="49cdf-141">Book cover.</span></span>|
|<span data-ttu-id="49cdf-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="49cdf-142">createdDateTime</span></span>|<span data-ttu-id="49cdf-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49cdf-143">DateTimeOffset</span></span>|<span data-ttu-id="49cdf-144">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="49cdf-144">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="49cdf-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="49cdf-145">lastModifiedDateTime</span></span>|<span data-ttu-id="49cdf-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="49cdf-146">DateTimeOffset</span></span>|<span data-ttu-id="49cdf-147">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="49cdf-147">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="49cdf-148">informationUrl</span><span class="sxs-lookup"><span data-stu-id="49cdf-148">informationUrl</span></span>|<span data-ttu-id="49cdf-149">String</span><span class="sxs-lookup"><span data-stu-id="49cdf-149">String</span></span>|<span data-ttu-id="49cdf-150">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="49cdf-150">The more information Url.</span></span>|
|<span data-ttu-id="49cdf-151">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="49cdf-151">privacyInformationUrl</span></span>|<span data-ttu-id="49cdf-152">String</span><span class="sxs-lookup"><span data-stu-id="49cdf-152">String</span></span>|<span data-ttu-id="49cdf-153">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="49cdf-153">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49cdf-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49cdf-154">Relationships</span></span>
|<span data-ttu-id="49cdf-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="49cdf-155">Relationship</span></span>|<span data-ttu-id="49cdf-156">型</span><span class="sxs-lookup"><span data-stu-id="49cdf-156">Type</span></span>|<span data-ttu-id="49cdf-157">説明</span><span class="sxs-lookup"><span data-stu-id="49cdf-157">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49cdf-158">categories</span><span class="sxs-lookup"><span data-stu-id="49cdf-158">categories</span></span>|<span data-ttu-id="49cdf-159">[managedebookcategory](../resources/intune-books-managedebookcategory.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="49cdf-159">[managedEBookCategory](../resources/intune-books-managedebookcategory.md) collection</span></span>|<span data-ttu-id="49cdf-160">この電子ブックのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="49cdf-160">The list of categories for this eBook.</span></span>|
|<span data-ttu-id="49cdf-161">assignments</span><span class="sxs-lookup"><span data-stu-id="49cdf-161">assignments</span></span>|<span data-ttu-id="49cdf-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="49cdf-162">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="49cdf-163">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="49cdf-163">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="49cdf-164">installSummary</span><span class="sxs-lookup"><span data-stu-id="49cdf-164">installSummary</span></span>|[<span data-ttu-id="49cdf-165">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="49cdf-165">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="49cdf-166">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="49cdf-166">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="49cdf-167">deviceStates</span><span class="sxs-lookup"><span data-stu-id="49cdf-167">deviceStates</span></span>|<span data-ttu-id="49cdf-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="49cdf-168">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="49cdf-169">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="49cdf-169">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="49cdf-170">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="49cdf-170">userStateSummary</span></span>|<span data-ttu-id="49cdf-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="49cdf-171">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="49cdf-172">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="49cdf-172">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49cdf-173">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49cdf-173">JSON Representation</span></span>
<span data-ttu-id="49cdf-174">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="49cdf-174">Here is a JSON representation of the resource.</span></span>
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





