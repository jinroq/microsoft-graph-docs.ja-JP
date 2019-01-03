---
title: mailSearchFolder リソースの種類
description: MailSearchFolder は、指定した検索条件に一致するすべてのメール アイテムが含まれているユーザーのメールボックス内の仮想フォルダーです。 mailSearchFolder は、mailFolder から継承します。
ms.openlocfilehash: abce7c86e44fcee98042aecf753f0fdf4172365e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071542"
---
# <a name="mailsearchfolder-resource-type"></a><span data-ttu-id="abb91-104">mailSearchFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="abb91-104">mailSearchFolder resource type</span></span>

> <span data-ttu-id="abb91-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="abb91-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abb91-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abb91-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="abb91-107">MailSearchFolder は、指定した検索条件に一致するすべてのメール アイテムが含まれているユーザーのメールボックス内の仮想フォルダーです。</span><span class="sxs-lookup"><span data-stu-id="abb91-107">A mailSearchFolder is a virtual folder in the user's mailbox that contains all the email items matching specified search criteria.</span></span> <span data-ttu-id="abb91-108">mailSearchFolder は、 [mailFolder](mailfolder.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="abb91-108">mailSearchFolder inherits from [mailFolder](mailfolder.md).</span></span>

## <a name="methods"></a><span data-ttu-id="abb91-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="abb91-109">Methods</span></span>

| <span data-ttu-id="abb91-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="abb91-110">Method</span></span> | <span data-ttu-id="abb91-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="abb91-111">Return Type</span></span>  | <span data-ttu-id="abb91-112">説明</span><span class="sxs-lookup"><span data-stu-id="abb91-112">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="abb91-113">検索フォルダーを作成する</span><span class="sxs-lookup"><span data-stu-id="abb91-113">Create a search folder</span></span>](../api/mailsearchfolder-post.md) | [<span data-ttu-id="abb91-114">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="abb91-114">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="abb91-115">このユーザーのメールボックスで検索フォルダーを作成します。</span><span class="sxs-lookup"><span data-stu-id="abb91-115">Create a search folder in this user's mailbox.</span></span> |
| [<span data-ttu-id="abb91-116">検索フォルダーの一覧</span><span class="sxs-lookup"><span data-stu-id="abb91-116">List search folders</span></span>](../api/mailfolder-list-childfolders.md) | <span data-ttu-id="abb91-117">[mailFolder](mailfolder.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="abb91-117">[mailFolder](mailfolder.md) collection</span></span> | <span data-ttu-id="abb91-118">検索フォルダーを含む、このユーザーのメールボックス内のすべてのフォルダーを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="abb91-118">List all the folders in this user's mailbox, including search folders.</span></span> |
| [<span data-ttu-id="abb91-119">検索フォルダ―を取得する</span><span class="sxs-lookup"><span data-stu-id="abb91-119">Get a search folder</span></span>](../api/mailfolder-get.md) | [<span data-ttu-id="abb91-120">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="abb91-120">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="abb91-121">指定した検索フォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="abb91-121">Get the specified search folder.</span></span> |
| [<span data-ttu-id="abb91-122">検索フォルダーを更新する</span><span class="sxs-lookup"><span data-stu-id="abb91-122">Update a search folder</span></span>](../api/mailsearchfolder-update.md) | [<span data-ttu-id="abb91-123">mailSearchFolder</span><span class="sxs-lookup"><span data-stu-id="abb91-123">mailSearchFolder</span></span>](mailsearchfolder.md) | <span data-ttu-id="abb91-124">指定した検索フォルダーを更新します。</span><span class="sxs-lookup"><span data-stu-id="abb91-124">Update the specified search folder.</span></span> |
| [<span data-ttu-id="abb91-125">検索フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="abb91-125">Delete a search folder</span></span>](../api/mailfolder-delete.md) | <span data-ttu-id="abb91-126">なし</span><span class="sxs-lookup"><span data-stu-id="abb91-126">None</span></span> | <span data-ttu-id="abb91-127">指定した検索フォルダーを削除します。</span><span class="sxs-lookup"><span data-stu-id="abb91-127">Delete the specified search folder.</span></span> |
| [<span data-ttu-id="abb91-128">検索フォルダー内のすべてのメッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="abb91-128">List all messages in a search folder</span></span>](../api/mailfolder-list-messages.md) | <span data-ttu-id="abb91-129">[message](message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="abb91-129">[message](message.md) collection</span></span> | <span data-ttu-id="abb91-130">指定した検索フォルダー内のすべてのメッセージを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="abb91-130">List all the messages in the specified search folder.</span></span> |

## <a name="properties"></a><span data-ttu-id="abb91-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abb91-131">Properties</span></span>

| <span data-ttu-id="abb91-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abb91-132">Property</span></span> | <span data-ttu-id="abb91-133">型</span><span class="sxs-lookup"><span data-stu-id="abb91-133">Type</span></span> | <span data-ttu-id="abb91-134">説明</span><span class="sxs-lookup"><span data-stu-id="abb91-134">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="abb91-135">参照して</span><span class="sxs-lookup"><span data-stu-id="abb91-135">isSupported</span></span> | <span data-ttu-id="abb91-136">ブール値</span><span class="sxs-lookup"><span data-stu-id="abb91-136">Boolean</span></span> | <span data-ttu-id="abb91-137">検索フォルダーは、REST Api を使用して編集可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="abb91-137">Indicates whether a search folder is editable using REST APIs.</span></span> |
| <span data-ttu-id="abb91-138">includeNestedFolders</span><span class="sxs-lookup"><span data-stu-id="abb91-138">includeNestedFolders</span></span> | <span data-ttu-id="abb91-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="abb91-139">Boolean</span></span> | <span data-ttu-id="abb91-140">メールボックス フォルダー階層を走査する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="abb91-140">Indicates how the mailbox folder hierarchy should be traversed.</span></span> <span data-ttu-id="abb91-141">`true`詳細検索をする必要があることを意味時に`false`簡易検索を代わりに行う必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="abb91-141">`true` means that a deep search should be done while `false` means a shallow search should be done instead.</span></span> |
| <span data-ttu-id="abb91-142">sourceFolderIDs</span><span class="sxs-lookup"><span data-stu-id="abb91-142">sourceFolderIDs</span></span> | <span data-ttu-id="abb91-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="abb91-143">String collection</span></span> | <span data-ttu-id="abb91-144">メールボックス フォルダーをマイニングする必要があります。</span><span class="sxs-lookup"><span data-stu-id="abb91-144">The mailbox folders that should be mined.</span></span> |
| <span data-ttu-id="abb91-145">filterQuery</span><span class="sxs-lookup"><span data-stu-id="abb91-145">filterQuery</span></span> | <span data-ttu-id="abb91-146">String</span><span class="sxs-lookup"><span data-stu-id="abb91-146">String</span></span> | <span data-ttu-id="abb91-147">メッセージをフィルタ リングする OData クエリです。</span><span class="sxs-lookup"><span data-stu-id="abb91-147">The OData query to filter the messages.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="abb91-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="abb91-148">JSON representation</span></span>

<span data-ttu-id="abb91-149">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="abb91-149">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mailSearchFolder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->