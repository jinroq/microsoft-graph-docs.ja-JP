---
title: mailsearchfolder リソースの種類
description: mailsearchfolder は、指定した検索条件に一致するすべての電子メールアイテムを含む、ユーザーのメールボックス内の仮想フォルダーです。 mailsearchfolder は mailfolder から継承します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 15f334f2910c962c367242965bd2104c8f3edb79
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342756"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="0a9b6-104">mailsearchfolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a9b6-104">mailSearchFolder resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a9b6-105">mailsearchfolder は、指定した検索条件に一致するすべての電子メールアイテムを含む、ユーザーのメールボックス内の仮想フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-105">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="0a9b6-106">mailsearchfolder は[mailfolder](mailfolder.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-106">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0a9b6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a9b6-107">Methods</span></span>

| <span data-ttu-id="0a9b6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a9b6-108">Method</span></span> | <span data-ttu-id="0a9b6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0a9b6-109">Return Type</span></span>  | <span data-ttu-id="0a9b6-110">説明</span><span class="sxs-lookup"><span data-stu-id="0a9b6-110">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="0a9b6-111">検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="0a9b6-111">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="0a9b6-112">mailsearchfolder</span><span class="sxs-lookup"><span data-stu-id="0a9b6-112">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="0a9b6-113">このユーザーのメールボックスに検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-113">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="0a9b6-114">検索フォルダーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0a9b6-114">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="0a9b6-115">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a9b6-115">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="0a9b6-116">このユーザーのメールボックス内のすべてのフォルダー (検索フォルダーを含む) を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-116">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="0a9b6-117">検索フォルダ―を取得する</span><span class="sxs-lookup"><span data-stu-id="0a9b6-117">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="0a9b6-118">mailsearchfolder</span><span class="sxs-lookup"><span data-stu-id="0a9b6-118">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="0a9b6-119">指定した検索フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-119">Get the specified search folder.</span></span> |
| [<span data-ttu-id="0a9b6-120">検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="0a9b6-120">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="0a9b6-121">mailsearchfolder</span><span class="sxs-lookup"><span data-stu-id="0a9b6-121">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="0a9b6-122">指定した検索フォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-122">Update the specified search folder.</span></span> |
| [<span data-ttu-id="0a9b6-123">検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="0a9b6-123">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="0a9b6-124">なし</span><span class="sxs-lookup"><span data-stu-id="0a9b6-124">None</span></span> | <span data-ttu-id="0a9b6-125">指定した検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-125">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="0a9b6-126">検索フォルダー内のすべてのメッセージを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0a9b6-126">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="0a9b6-127">[message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a9b6-127">[message](message.md) collection</span></span> | <span data-ttu-id="0a9b6-128">指定した検索フォルダー内のすべてのメッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-128">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="0a9b6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a9b6-129">Properties</span></span>

| <span data-ttu-id="0a9b6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a9b6-130">Property</span></span> | <span data-ttu-id="0a9b6-131">型</span><span class="sxs-lookup"><span data-stu-id="0a9b6-131">Type</span></span> | <span data-ttu-id="0a9b6-132">説明</span><span class="sxs-lookup"><span data-stu-id="0a9b6-132">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="0a9b6-133">issupported</span><span class="sxs-lookup"><span data-stu-id="0a9b6-133">isSupported</span></span> | <span data-ttu-id="0a9b6-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a9b6-134">Boolean</span></span> | <span data-ttu-id="0a9b6-135">検索フォルダーが REST api を使用して編集可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-135">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="0a9b6-136">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="0a9b6-136">includeNestedFolders</span></span> | <span data-ttu-id="0a9b6-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a9b6-137">Boolean</span></span> | <span data-ttu-id="0a9b6-138">メールボックスフォルダー階層をスキャンする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-138">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="0a9b6-139">`true`詳細検索を実行`false`する必要がある場合は、その代わりに浅い検索を実行する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-139">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="0a9b6-140">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="0a9b6-140">sourceFolderIDs</span></span> | <span data-ttu-id="0a9b6-141">String collection</span><span class="sxs-lookup"><span data-stu-id="0a9b6-141">String collection</span></span> | <span data-ttu-id="0a9b6-142">マイニングするメールボックスフォルダー。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-142">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="0a9b6-143">filterquery</span><span class="sxs-lookup"><span data-stu-id="0a9b6-143">filterQuery</span></span> | <span data-ttu-id="0a9b6-144">String</span><span class="sxs-lookup"><span data-stu-id="0a9b6-144">String</span></span> | <span data-ttu-id="0a9b6-145">メッセージをフィルター処理するための OData クエリ。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-145">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0a9b6-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a9b6-146">JSON representation</span></span>

<span data-ttu-id="0a9b6-147">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0a9b6-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailSearchFolder"
}-->

```json
{
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIDs": ["string"],
  "filterQuery": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2018-01-23 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
