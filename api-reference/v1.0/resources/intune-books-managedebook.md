---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ae6151c23bf05b076ade441f908a2810c80f45ed
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253464"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="d5e54-103">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d5e54-103">managedEBook resource type</span></span>

> <span data-ttu-id="d5e54-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5e54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5e54-105">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="d5e54-105">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="d5e54-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d5e54-106">Methods</span></span>
|<span data-ttu-id="d5e54-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d5e54-107">Method</span></span>|<span data-ttu-id="d5e54-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d5e54-108">Return Type</span></span>|<span data-ttu-id="d5e54-109">説明</span><span class="sxs-lookup"><span data-stu-id="d5e54-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d5e54-110">managedEBook のリスト</span><span class="sxs-lookup"><span data-stu-id="d5e54-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="d5e54-111">[managedEBook](../resources/intune-books-managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d5e54-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="d5e54-112">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d5e54-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="d5e54-113">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="d5e54-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="d5e54-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="d5e54-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="d5e54-115">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d5e54-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="d5e54-116">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="d5e54-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="d5e54-117">なし</span><span class="sxs-lookup"><span data-stu-id="d5e54-117">None</span></span>|<span data-ttu-id="d5e54-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d5e54-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d5e54-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5e54-119">Properties</span></span>
|<span data-ttu-id="d5e54-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d5e54-120">Property</span></span>|<span data-ttu-id="d5e54-121">型</span><span class="sxs-lookup"><span data-stu-id="d5e54-121">Type</span></span>|<span data-ttu-id="d5e54-122">説明</span><span class="sxs-lookup"><span data-stu-id="d5e54-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5e54-123">id</span><span class="sxs-lookup"><span data-stu-id="d5e54-123">id</span></span>|<span data-ttu-id="d5e54-124">文字列</span><span class="sxs-lookup"><span data-stu-id="d5e54-124">String</span></span>|<span data-ttu-id="d5e54-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d5e54-125">Key of the entity.</span></span>|
|<span data-ttu-id="d5e54-126">displayName</span><span class="sxs-lookup"><span data-stu-id="d5e54-126">displayName</span></span>|<span data-ttu-id="d5e54-127">String</span><span class="sxs-lookup"><span data-stu-id="d5e54-127">String</span></span>|<span data-ttu-id="d5e54-128">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="d5e54-128">Name of the eBook.</span></span>|
|<span data-ttu-id="d5e54-129">説明</span><span class="sxs-lookup"><span data-stu-id="d5e54-129">description</span></span>|<span data-ttu-id="d5e54-130">文字列</span><span class="sxs-lookup"><span data-stu-id="d5e54-130">String</span></span>|<span data-ttu-id="d5e54-131">説明。</span><span class="sxs-lookup"><span data-stu-id="d5e54-131">Description.</span></span>|
|<span data-ttu-id="d5e54-132">publisher</span><span class="sxs-lookup"><span data-stu-id="d5e54-132">publisher</span></span>|<span data-ttu-id="d5e54-133">String</span><span class="sxs-lookup"><span data-stu-id="d5e54-133">String</span></span>|<span data-ttu-id="d5e54-134">発行元です。</span><span class="sxs-lookup"><span data-stu-id="d5e54-134">Publisher.</span></span>|
|<span data-ttu-id="d5e54-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5e54-135">publishedDateTime</span></span>|<span data-ttu-id="d5e54-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5e54-136">DateTimeOffset</span></span>|<span data-ttu-id="d5e54-137">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="d5e54-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="d5e54-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="d5e54-138">largeCover</span></span>|[<span data-ttu-id="d5e54-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d5e54-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d5e54-140">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="d5e54-140">Book cover.</span></span>|
|<span data-ttu-id="d5e54-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d5e54-141">createdDateTime</span></span>|<span data-ttu-id="d5e54-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5e54-142">DateTimeOffset</span></span>|<span data-ttu-id="d5e54-143">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d5e54-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="d5e54-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d5e54-144">lastModifiedDateTime</span></span>|<span data-ttu-id="d5e54-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d5e54-145">DateTimeOffset</span></span>|<span data-ttu-id="d5e54-146">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d5e54-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="d5e54-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d5e54-147">informationUrl</span></span>|<span data-ttu-id="d5e54-148">String</span><span class="sxs-lookup"><span data-stu-id="d5e54-148">String</span></span>|<span data-ttu-id="d5e54-149">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="d5e54-149">The more information Url.</span></span>|
|<span data-ttu-id="d5e54-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d5e54-150">privacyInformationUrl</span></span>|<span data-ttu-id="d5e54-151">String</span><span class="sxs-lookup"><span data-stu-id="d5e54-151">String</span></span>|<span data-ttu-id="d5e54-152">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="d5e54-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d5e54-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d5e54-153">Relationships</span></span>
|<span data-ttu-id="d5e54-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d5e54-154">Relationship</span></span>|<span data-ttu-id="d5e54-155">型</span><span class="sxs-lookup"><span data-stu-id="d5e54-155">Type</span></span>|<span data-ttu-id="d5e54-156">説明</span><span class="sxs-lookup"><span data-stu-id="d5e54-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5e54-157">assignments</span><span class="sxs-lookup"><span data-stu-id="d5e54-157">assignments</span></span>|<span data-ttu-id="d5e54-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d5e54-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="d5e54-159">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="d5e54-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="d5e54-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="d5e54-160">installSummary</span></span>|[<span data-ttu-id="d5e54-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="d5e54-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="d5e54-162">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="d5e54-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="d5e54-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="d5e54-163">deviceStates</span></span>|<span data-ttu-id="d5e54-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d5e54-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="d5e54-165">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="d5e54-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="d5e54-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="d5e54-166">userStateSummary</span></span>|<span data-ttu-id="d5e54-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d5e54-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="d5e54-168">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="d5e54-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d5e54-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d5e54-169">JSON Representation</span></span>
<span data-ttu-id="d5e54-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d5e54-170">Here is a JSON representation of the resource.</span></span>
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



