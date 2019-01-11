---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 61a4098850f9b3b4a6b82f2fcee5d1ce89b0696d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830255"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="01e26-103">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="01e26-103">managedEBook resource type</span></span>

> <span data-ttu-id="01e26-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="01e26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01e26-105">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="01e26-105">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="01e26-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="01e26-106">Methods</span></span>
|<span data-ttu-id="01e26-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="01e26-107">Method</span></span>|<span data-ttu-id="01e26-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="01e26-108">Return Type</span></span>|<span data-ttu-id="01e26-109">説明</span><span class="sxs-lookup"><span data-stu-id="01e26-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="01e26-110">managedEBook のリスト</span><span class="sxs-lookup"><span data-stu-id="01e26-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="01e26-111">[managedEBook](../resources/intune-books-managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="01e26-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="01e26-112">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="01e26-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="01e26-113">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="01e26-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="01e26-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="01e26-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="01e26-115">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="01e26-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="01e26-116">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="01e26-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="01e26-117">なし</span><span class="sxs-lookup"><span data-stu-id="01e26-117">None</span></span>|<span data-ttu-id="01e26-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="01e26-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="01e26-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01e26-119">Properties</span></span>
|<span data-ttu-id="01e26-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01e26-120">Property</span></span>|<span data-ttu-id="01e26-121">種類</span><span class="sxs-lookup"><span data-stu-id="01e26-121">Type</span></span>|<span data-ttu-id="01e26-122">説明</span><span class="sxs-lookup"><span data-stu-id="01e26-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01e26-123">ID</span><span class="sxs-lookup"><span data-stu-id="01e26-123">id</span></span>|<span data-ttu-id="01e26-124">String</span><span class="sxs-lookup"><span data-stu-id="01e26-124">String</span></span>|<span data-ttu-id="01e26-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="01e26-125">Key of the entity.</span></span>|
|<span data-ttu-id="01e26-126">displayName</span><span class="sxs-lookup"><span data-stu-id="01e26-126">displayName</span></span>|<span data-ttu-id="01e26-127">String</span><span class="sxs-lookup"><span data-stu-id="01e26-127">String</span></span>|<span data-ttu-id="01e26-128">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="01e26-128">Name of the eBook.</span></span>|
|<span data-ttu-id="01e26-129">説明</span><span class="sxs-lookup"><span data-stu-id="01e26-129">description</span></span>|<span data-ttu-id="01e26-130">String</span><span class="sxs-lookup"><span data-stu-id="01e26-130">String</span></span>|<span data-ttu-id="01e26-131">説明。</span><span class="sxs-lookup"><span data-stu-id="01e26-131">Description.</span></span>|
|<span data-ttu-id="01e26-132">publisher</span><span class="sxs-lookup"><span data-stu-id="01e26-132">publisher</span></span>|<span data-ttu-id="01e26-133">String</span><span class="sxs-lookup"><span data-stu-id="01e26-133">String</span></span>|<span data-ttu-id="01e26-134">発行元です。</span><span class="sxs-lookup"><span data-stu-id="01e26-134">Publisher.</span></span>|
|<span data-ttu-id="01e26-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="01e26-135">publishedDateTime</span></span>|<span data-ttu-id="01e26-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01e26-136">DateTimeOffset</span></span>|<span data-ttu-id="01e26-137">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="01e26-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="01e26-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="01e26-138">largeCover</span></span>|[<span data-ttu-id="01e26-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="01e26-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="01e26-140">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="01e26-140">Book cover.</span></span>|
|<span data-ttu-id="01e26-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="01e26-141">createdDateTime</span></span>|<span data-ttu-id="01e26-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01e26-142">DateTimeOffset</span></span>|<span data-ttu-id="01e26-143">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="01e26-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="01e26-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="01e26-144">lastModifiedDateTime</span></span>|<span data-ttu-id="01e26-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="01e26-145">DateTimeOffset</span></span>|<span data-ttu-id="01e26-146">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="01e26-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="01e26-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="01e26-147">informationUrl</span></span>|<span data-ttu-id="01e26-148">String</span><span class="sxs-lookup"><span data-stu-id="01e26-148">String</span></span>|<span data-ttu-id="01e26-149">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="01e26-149">The more information Url.</span></span>|
|<span data-ttu-id="01e26-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="01e26-150">privacyInformationUrl</span></span>|<span data-ttu-id="01e26-151">String</span><span class="sxs-lookup"><span data-stu-id="01e26-151">String</span></span>|<span data-ttu-id="01e26-152">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="01e26-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01e26-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="01e26-153">Relationships</span></span>
|<span data-ttu-id="01e26-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="01e26-154">Relationship</span></span>|<span data-ttu-id="01e26-155">型</span><span class="sxs-lookup"><span data-stu-id="01e26-155">Type</span></span>|<span data-ttu-id="01e26-156">説明</span><span class="sxs-lookup"><span data-stu-id="01e26-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01e26-157">assignments</span><span class="sxs-lookup"><span data-stu-id="01e26-157">assignments</span></span>|<span data-ttu-id="01e26-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="01e26-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="01e26-159">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="01e26-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="01e26-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="01e26-160">installSummary</span></span>|[<span data-ttu-id="01e26-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="01e26-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="01e26-162">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="01e26-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="01e26-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="01e26-163">deviceStates</span></span>|<span data-ttu-id="01e26-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="01e26-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="01e26-165">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="01e26-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="01e26-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="01e26-166">userStateSummary</span></span>|<span data-ttu-id="01e26-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="01e26-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="01e26-168">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="01e26-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="01e26-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="01e26-169">JSON Representation</span></span>
<span data-ttu-id="01e26-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="01e26-170">Here is a JSON representation of the resource.</span></span>
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



