---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 42d14dbd1c2afa6eb316bcb46cf3fe76bd0669e0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028813"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="1e309-103">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1e309-103">managedEBook resource type</span></span>

> <span data-ttu-id="1e309-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e309-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e309-105">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="1e309-105">An abstract class containing the base properties for Managed eBook.</span></span>

## <a name="methods"></a><span data-ttu-id="1e309-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e309-106">Methods</span></span>
|<span data-ttu-id="1e309-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1e309-107">Method</span></span>|<span data-ttu-id="1e309-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1e309-108">Return Type</span></span>|<span data-ttu-id="1e309-109">説明</span><span class="sxs-lookup"><span data-stu-id="1e309-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1e309-110">managedEBook のリスト</span><span class="sxs-lookup"><span data-stu-id="1e309-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="1e309-111">[managedEBook](../resources/intune-books-managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1e309-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="1e309-112">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1e309-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="1e309-113">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="1e309-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="1e309-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="1e309-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="1e309-115">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1e309-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="1e309-116">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="1e309-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="1e309-117">なし</span><span class="sxs-lookup"><span data-stu-id="1e309-117">None</span></span>|<span data-ttu-id="1e309-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1e309-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1e309-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e309-119">Properties</span></span>
|<span data-ttu-id="1e309-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e309-120">Property</span></span>|<span data-ttu-id="1e309-121">型</span><span class="sxs-lookup"><span data-stu-id="1e309-121">Type</span></span>|<span data-ttu-id="1e309-122">説明</span><span class="sxs-lookup"><span data-stu-id="1e309-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e309-123">id</span><span class="sxs-lookup"><span data-stu-id="1e309-123">id</span></span>|<span data-ttu-id="1e309-124">文字列</span><span class="sxs-lookup"><span data-stu-id="1e309-124">String</span></span>|<span data-ttu-id="1e309-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1e309-125">Key of the entity.</span></span>|
|<span data-ttu-id="1e309-126">displayName</span><span class="sxs-lookup"><span data-stu-id="1e309-126">displayName</span></span>|<span data-ttu-id="1e309-127">String</span><span class="sxs-lookup"><span data-stu-id="1e309-127">String</span></span>|<span data-ttu-id="1e309-128">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="1e309-128">Name of the eBook.</span></span>|
|<span data-ttu-id="1e309-129">description</span><span class="sxs-lookup"><span data-stu-id="1e309-129">description</span></span>|<span data-ttu-id="1e309-130">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1e309-130">String</span></span>|<span data-ttu-id="1e309-131">説明。</span><span class="sxs-lookup"><span data-stu-id="1e309-131">Description.</span></span>|
|<span data-ttu-id="1e309-132">publisher</span><span class="sxs-lookup"><span data-stu-id="1e309-132">publisher</span></span>|<span data-ttu-id="1e309-133">String</span><span class="sxs-lookup"><span data-stu-id="1e309-133">String</span></span>|<span data-ttu-id="1e309-134">発行元です。</span><span class="sxs-lookup"><span data-stu-id="1e309-134">Publisher.</span></span>|
|<span data-ttu-id="1e309-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e309-135">publishedDateTime</span></span>|<span data-ttu-id="1e309-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e309-136">DateTimeOffset</span></span>|<span data-ttu-id="1e309-137">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="1e309-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="1e309-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="1e309-138">largeCover</span></span>|[<span data-ttu-id="1e309-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1e309-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1e309-140">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="1e309-140">Book cover.</span></span>|
|<span data-ttu-id="1e309-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e309-141">createdDateTime</span></span>|<span data-ttu-id="1e309-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e309-142">DateTimeOffset</span></span>|<span data-ttu-id="1e309-143">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1e309-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="1e309-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e309-144">lastModifiedDateTime</span></span>|<span data-ttu-id="1e309-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e309-145">DateTimeOffset</span></span>|<span data-ttu-id="1e309-146">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="1e309-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="1e309-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1e309-147">informationUrl</span></span>|<span data-ttu-id="1e309-148">String</span><span class="sxs-lookup"><span data-stu-id="1e309-148">String</span></span>|<span data-ttu-id="1e309-149">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="1e309-149">The more information Url.</span></span>|
|<span data-ttu-id="1e309-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1e309-150">privacyInformationUrl</span></span>|<span data-ttu-id="1e309-151">String</span><span class="sxs-lookup"><span data-stu-id="1e309-151">String</span></span>|<span data-ttu-id="1e309-152">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="1e309-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e309-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e309-153">Relationships</span></span>
|<span data-ttu-id="1e309-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1e309-154">Relationship</span></span>|<span data-ttu-id="1e309-155">型</span><span class="sxs-lookup"><span data-stu-id="1e309-155">Type</span></span>|<span data-ttu-id="1e309-156">説明</span><span class="sxs-lookup"><span data-stu-id="1e309-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e309-157">assignments</span><span class="sxs-lookup"><span data-stu-id="1e309-157">assignments</span></span>|<span data-ttu-id="1e309-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1e309-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="1e309-159">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="1e309-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="1e309-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="1e309-160">installSummary</span></span>|[<span data-ttu-id="1e309-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="1e309-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="1e309-162">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="1e309-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="1e309-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="1e309-163">deviceStates</span></span>|<span data-ttu-id="1e309-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1e309-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="1e309-165">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="1e309-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="1e309-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="1e309-166">userStateSummary</span></span>|<span data-ttu-id="1e309-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1e309-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="1e309-168">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="1e309-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e309-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1e309-169">JSON Representation</span></span>
<span data-ttu-id="1e309-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1e309-170">Here is a JSON representation of the resource.</span></span>
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



