---
title: 契約のリソースの種類
description: テナントのカスタマイズ可能な使用許諾契約書が作成され、Azure Active Directory (AD の Azure) を使用して管理する条件を表します。 機能を管理、Azure Active Directory の使用条件に従って、シナリオを作成し、次のメソッドを使用できます。
ms.openlocfilehash: 2e5c9087cd809f9c067150654d420fda533ca61b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068805"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="d22f8-104">契約のリソースの種類</span><span class="sxs-lookup"><span data-stu-id="d22f8-104">agreement resource type</span></span>

> <span data-ttu-id="d22f8-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d22f8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d22f8-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d22f8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d22f8-107">テナントのカスタマイズ可能な使用許諾契約書が作成され、Azure Active Directory (AD の Azure) を使用して管理する条件を表します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-107">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="d22f8-108">作成し、シナリオに基づく[Azure Active Directory の使用条件の機能](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)を管理するのには、次のメソッドを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d22f8-108">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="d22f8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d22f8-109">Methods</span></span>

| <span data-ttu-id="d22f8-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="d22f8-110">Method</span></span>       | <span data-ttu-id="d22f8-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d22f8-111">Return Type</span></span> | <span data-ttu-id="d22f8-112">説明</span><span class="sxs-lookup"><span data-stu-id="d22f8-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d22f8-113">契約書を作成します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-113">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="d22f8-114">契約</span><span class="sxs-lookup"><span data-stu-id="d22f8-114">agreement</span></span>](agreement.md) | <span data-ttu-id="d22f8-115">契約コレクションへの投稿には、新しい契約を作成します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-115">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="d22f8-116">リスト契約</span><span class="sxs-lookup"><span data-stu-id="d22f8-116">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="d22f8-117">[契約](agreement.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d22f8-117">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="d22f8-118">契約オブジェクト コレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-118">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="d22f8-119">契約を取得します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-119">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="d22f8-120">契約</span><span class="sxs-lookup"><span data-stu-id="d22f8-120">agreement</span></span>](agreement.md) | <span data-ttu-id="d22f8-121">契約オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d22f8-121">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="d22f8-122">契約を更新します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-122">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="d22f8-123">契約</span><span class="sxs-lookup"><span data-stu-id="d22f8-123">agreement</span></span>](agreement.md) | <span data-ttu-id="d22f8-124">契約オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-124">Update an agreement object.</span></span> |
| [<span data-ttu-id="d22f8-125">契約を削除します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-125">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="d22f8-126">なし</span><span class="sxs-lookup"><span data-stu-id="d22f8-126">None</span></span> | <span data-ttu-id="d22f8-127">契約オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-127">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="d22f8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d22f8-128">Properties</span></span>
| <span data-ttu-id="d22f8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d22f8-129">Property</span></span>     | <span data-ttu-id="d22f8-130">型</span><span class="sxs-lookup"><span data-stu-id="d22f8-130">Type</span></span>        | <span data-ttu-id="d22f8-131">説明</span><span class="sxs-lookup"><span data-stu-id="d22f8-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d22f8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d22f8-132">displayName</span></span>|<span data-ttu-id="d22f8-133">String</span><span class="sxs-lookup"><span data-stu-id="d22f8-133">String</span></span>|<span data-ttu-id="d22f8-134">契約書の名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="d22f8-135">id</span><span class="sxs-lookup"><span data-stu-id="d22f8-135">id</span></span>|<span data-ttu-id="d22f8-136">String</span><span class="sxs-lookup"><span data-stu-id="d22f8-136">String</span></span>| <span data-ttu-id="d22f8-137">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d22f8-137">Read-only.</span></span>|
|<span data-ttu-id="d22f8-138">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="d22f8-138">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="d22f8-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="d22f8-139">Boolean</span></span>|<span data-ttu-id="d22f8-140">ユーザーを展開し、受け入れる前に契約書を表示するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-140">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d22f8-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d22f8-141">Relationships</span></span>
| <span data-ttu-id="d22f8-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d22f8-142">Relationship</span></span> | <span data-ttu-id="d22f8-143">型</span><span class="sxs-lookup"><span data-stu-id="d22f8-143">Type</span></span>        | <span data-ttu-id="d22f8-144">説明</span><span class="sxs-lookup"><span data-stu-id="d22f8-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d22f8-145">files</span><span class="sxs-lookup"><span data-stu-id="d22f8-145">files</span></span>|<span data-ttu-id="d22f8-146">[agreementFile](agreementfile.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d22f8-146">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="d22f8-147">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="d22f8-147">Read-only.</span></span> <span data-ttu-id="d22f8-148">Pdf は、本契約にリンクされています。</span><span class="sxs-lookup"><span data-stu-id="d22f8-148">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d22f8-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d22f8-149">JSON representation</span></span>

<span data-ttu-id="d22f8-150">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d22f8-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
