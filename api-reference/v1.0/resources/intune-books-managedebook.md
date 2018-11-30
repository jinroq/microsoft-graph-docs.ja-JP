---
title: managedEBook リソースの種類
description: 管理対象電子ブックの基本プロパティを含む抽象クラスです。
ms.openlocfilehash: 427582977558254561b219dff2392f01ced4f53d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023486"
---
# <a name="managedebook-resource-type"></a><span data-ttu-id="a1e9e-103">managedEBook リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a1e9e-103">managedEBook resource type</span></span>

> <span data-ttu-id="a1e9e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1e9e-105">管理対象電子ブックの基本プロパティを含む抽象クラスです。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-105">An abstract class containing the base properties for Managed eBook.</span></span>
## <a name="methods"></a><span data-ttu-id="a1e9e-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1e9e-106">Methods</span></span>
|<span data-ttu-id="a1e9e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a1e9e-107">Method</span></span>|<span data-ttu-id="a1e9e-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a1e9e-108">Return Type</span></span>|<span data-ttu-id="a1e9e-109">説明</span><span class="sxs-lookup"><span data-stu-id="a1e9e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a1e9e-110">managedEBook のリスト</span><span class="sxs-lookup"><span data-stu-id="a1e9e-110">List managedEBooks</span></span>](../api/intune-books-managedebook-list.md)|<span data-ttu-id="a1e9e-111">[managedEBook](../resources/intune-books-managedebook.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1e9e-111">[managedEBook](../resources/intune-books-managedebook.md) collection</span></span>|<span data-ttu-id="a1e9e-112">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-112">List properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) objects.</span></span>|
|[<span data-ttu-id="a1e9e-113">managedEBook の取得</span><span class="sxs-lookup"><span data-stu-id="a1e9e-113">Get managedEBook</span></span>](../api/intune-books-managedebook-get.md)|[<span data-ttu-id="a1e9e-114">managedEBook</span><span class="sxs-lookup"><span data-stu-id="a1e9e-114">managedEBook</span></span>](../resources/intune-books-managedebook.md)|<span data-ttu-id="a1e9e-115">[managedEBook](../resources/intune-books-managedebook.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-115">Read properties and relationships of the [managedEBook](../resources/intune-books-managedebook.md) object.</span></span>|
|[<span data-ttu-id="a1e9e-116">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="a1e9e-116">assign action</span></span>](../api/intune-books-managedebook-assign.md)|<span data-ttu-id="a1e9e-117">なし</span><span class="sxs-lookup"><span data-stu-id="a1e9e-117">None</span></span>|<span data-ttu-id="a1e9e-118">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a1e9e-118">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="a1e9e-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1e9e-119">Properties</span></span>
|<span data-ttu-id="a1e9e-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a1e9e-120">Property</span></span>|<span data-ttu-id="a1e9e-121">型</span><span class="sxs-lookup"><span data-stu-id="a1e9e-121">Type</span></span>|<span data-ttu-id="a1e9e-122">説明</span><span class="sxs-lookup"><span data-stu-id="a1e9e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1e9e-123">id</span><span class="sxs-lookup"><span data-stu-id="a1e9e-123">id</span></span>|<span data-ttu-id="a1e9e-124">String</span><span class="sxs-lookup"><span data-stu-id="a1e9e-124">String</span></span>|<span data-ttu-id="a1e9e-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-125">Key of the entity.</span></span>|
|<span data-ttu-id="a1e9e-126">displayName</span><span class="sxs-lookup"><span data-stu-id="a1e9e-126">displayName</span></span>|<span data-ttu-id="a1e9e-127">String</span><span class="sxs-lookup"><span data-stu-id="a1e9e-127">String</span></span>|<span data-ttu-id="a1e9e-128">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-128">Name of the eBook.</span></span>|
|<span data-ttu-id="a1e9e-129">説明</span><span class="sxs-lookup"><span data-stu-id="a1e9e-129">description</span></span>|<span data-ttu-id="a1e9e-130">String</span><span class="sxs-lookup"><span data-stu-id="a1e9e-130">String</span></span>|<span data-ttu-id="a1e9e-131">説明。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-131">Description.</span></span>|
|<span data-ttu-id="a1e9e-132">publisher</span><span class="sxs-lookup"><span data-stu-id="a1e9e-132">publisher</span></span>|<span data-ttu-id="a1e9e-133">String</span><span class="sxs-lookup"><span data-stu-id="a1e9e-133">String</span></span>|<span data-ttu-id="a1e9e-134">発行元です。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-134">Publisher.</span></span>|
|<span data-ttu-id="a1e9e-135">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e9e-135">publishedDateTime</span></span>|<span data-ttu-id="a1e9e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e9e-136">DateTimeOffset</span></span>|<span data-ttu-id="a1e9e-137">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-137">The date and time when the eBook was published.</span></span>|
|<span data-ttu-id="a1e9e-138">largeCover</span><span class="sxs-lookup"><span data-stu-id="a1e9e-138">largeCover</span></span>|[<span data-ttu-id="a1e9e-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a1e9e-139">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a1e9e-140">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-140">Book cover.</span></span>|
|<span data-ttu-id="a1e9e-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e9e-141">createdDateTime</span></span>|<span data-ttu-id="a1e9e-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e9e-142">DateTimeOffset</span></span>|<span data-ttu-id="a1e9e-143">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-143">The date and time when the eBook file was created.</span></span>|
|<span data-ttu-id="a1e9e-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e9e-144">lastModifiedDateTime</span></span>|<span data-ttu-id="a1e9e-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e9e-145">DateTimeOffset</span></span>|<span data-ttu-id="a1e9e-146">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-146">The date and time when the eBook was last modified.</span></span>|
|<span data-ttu-id="a1e9e-147">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a1e9e-147">informationUrl</span></span>|<span data-ttu-id="a1e9e-148">String</span><span class="sxs-lookup"><span data-stu-id="a1e9e-148">String</span></span>|<span data-ttu-id="a1e9e-149">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-149">The more information Url.</span></span>|
|<span data-ttu-id="a1e9e-150">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a1e9e-150">privacyInformationUrl</span></span>|<span data-ttu-id="a1e9e-151">String</span><span class="sxs-lookup"><span data-stu-id="a1e9e-151">String</span></span>|<span data-ttu-id="a1e9e-152">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-152">The privacy statement Url.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1e9e-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1e9e-153">Relationships</span></span>
|<span data-ttu-id="a1e9e-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a1e9e-154">Relationship</span></span>|<span data-ttu-id="a1e9e-155">型</span><span class="sxs-lookup"><span data-stu-id="a1e9e-155">Type</span></span>|<span data-ttu-id="a1e9e-156">説明</span><span class="sxs-lookup"><span data-stu-id="a1e9e-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1e9e-157">assignments</span><span class="sxs-lookup"><span data-stu-id="a1e9e-157">assignments</span></span>|<span data-ttu-id="a1e9e-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1e9e-158">[managedEBookAssignment](../resources/intune-books-managedebookassignment.md) collection</span></span>|<span data-ttu-id="a1e9e-159">この電子ブックの割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-159">The list of assignments for this eBook.</span></span>|
|<span data-ttu-id="a1e9e-160">installSummary</span><span class="sxs-lookup"><span data-stu-id="a1e9e-160">installSummary</span></span>|[<span data-ttu-id="a1e9e-161">eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="a1e9e-161">eBookInstallSummary</span></span>](../resources/intune-books-ebookinstallsummary.md)|<span data-ttu-id="a1e9e-162">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-162">Mobile App Install Summary.</span></span>|
|<span data-ttu-id="a1e9e-163">deviceStates</span><span class="sxs-lookup"><span data-stu-id="a1e9e-163">deviceStates</span></span>|<span data-ttu-id="a1e9e-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1e9e-164">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) collection</span></span>|<span data-ttu-id="a1e9e-165">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-165">The list of installation states for this eBook.</span></span>|
|<span data-ttu-id="a1e9e-166">userStateSummary</span><span class="sxs-lookup"><span data-stu-id="a1e9e-166">userStateSummary</span></span>|<span data-ttu-id="a1e9e-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a1e9e-167">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) collection</span></span>|<span data-ttu-id="a1e9e-168">この電子ブックのインストール状態のリストです。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-168">The list of installation states for this eBook.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1e9e-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a1e9e-169">JSON Representation</span></span>
<span data-ttu-id="a1e9e-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a1e9e-170">Here is a JSON representation of the resource.</span></span>
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



